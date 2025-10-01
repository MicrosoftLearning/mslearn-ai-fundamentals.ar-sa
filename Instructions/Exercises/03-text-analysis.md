---
lab:
  title: تحليل النص في مدخل Azure AI Foundry
---

# تحليل النص في مدخل Azure AI Foundry

تتضمن خدمة Azure AI Language تحليلات النصوص، مع إمكانيات مثل التعرّف على الكيان، واستخراج العبارات الرئيسية، والتلخيص، وتحليل المشاعر. على سبيل المثال، لنفترض أن وكيل السفر الوهمي Margie's Travel يشجع العملاء على إرسال تقييمات للإقامات في الفنادق. بإمكانك استخدام خدمة "اللغة" لاستخراج الكيانات المسماة، وتحديد العبارات الرئيسية، وتلخيص النص، والمزيد.

في هذا التمرين، ستستخدم Azure AI Language في مدخل Azure AI Foundry، وهي منصة Microsoft لإنشاء التطبيقات الذكية، لتحليل مراجعات الفنادق. 

يستغرق هذا التدريب حوالي **20** دقيقة.

## إنشاء مشروع في مدخل Azure AI Foundry

1. في متصفح الويب، افتح [مدخل Azure AI Foundry](https://ai.azure.com) على `https://ai.azure.com` وسجّل الدخول باستخدام بيانات اعتماد Azure الخاصة بك. أغلق أي تلميحات أو أجزاء التشغيل السريع يتم فتحه عندما تقوم بتسجيل الدخول لأول مرة، وإذا لزم الأمر،استخدم شعار **Azure AI Foundry** في أعلى اليسار للانتقال إلى الصفحة الرئيسية، والتي تبدو مشابهة للصورة التالية (أغلق جزء **المساعدة** إذا كان مفتوحًا):

    ![لقطة شاشة للصفحة الرئيسية في بوابة Azure AI Foundry.](./media/ai-foundry-portal.png)

1. مرّر إلى أسفل الصفحة، وحدّد مربع **استكشاف خدمات Azure AI**.

    ![لقطة شاشة لمربع استكشاف خدمات Azure AI.](./media/ai-services.png)

1. في صفحة خدمات Azure AI، حدّد مربع **Language + Translator**.

    ![لقطة شاشة لمربع Language + Translator.](./media/language-tile.png)

1. في صفحة **Language + Translator**، حدّد **تجربة مساحة اختبار اللغة**. بعد ذلك، عند المطالبة، قُم بإنشاء مشروع جديد باستخدام الإعدادات التالية:
    - **اسم المشروع**: *أدخِل اسمًا صالحًا لمشروعك.*
    - **الإعدادات المتقدمة**:
        - **Subscription**: *اشتراكك في Azure*
        - **Resource group**: *إنشاء مجموعة موارد أو تحديدها*
        - **المنطقة**: *حدّد أيًّا من مناطق **AI Foundry الموصى بها***
        - **AI Foundry أو Azure OpenAI** *أنشئ موردًا جديدًا في Azure AI Foundry باستخدام اسم صالح*

1. حدد **إنشاء**. انتظر حتى يتم إنشاء مشروعك. قد يستغرق ذلك بضع دقائق.

1. عند إنشاء المشروع، سيتم نقلك إلى مساحة اختبار **اللغة** (وإذا لم يتم ذلك تلقائيًا، فحدّد **مساحات الاختبار** في جزء المهام على اليسار، ثم افتح منها مساحة اختبار "اللغة").

    تُعدّ مساحة اختبار اللغة واجهة مستخدم تتيح لك تجربة بعض إمكانيات Azure AI Language.  

## استخدام Azure AI Language لتحليل النص

توفر خدمة Azure AI Language مجموعة متنوعه من أدوات تحليل النصوص.

### استخراج الكيانات المسماة باستخدام Azure AI Language في مدخل Azure AI Foundry

*الكيانات المسماة* هي كلمات تصف الأشخاص والأماكن والأشياء بأسماء مناسبة. دعنا نستخدم إمكانية استخراج الكيان المسمى في Azure AI Language لتحديد أنواع المعلومات في المراجعة.

1. في بيئة اللغة، حدد **استخراج المعلومات**. ثم حدد لوحة **استخراج الكيانات المسماة**. 

1. ضمن خانة *النموذج*، أدخِل التقييم التالي:

    ```
    Tired hotel with poor service
    The Royal Hotel, London, United Kingdom
    5/6/2018
    This is an old hotel (has been around since 1950's) and the room furnishings are average - becoming a bit old now and require changing. The internet didn't work and had to come to one of their office rooms to check in for my flight home. The website says it's close to the British Museum, but it's too far to walk.
    ```

1. حدد **تشغيل**. راجع الإخراج.

    ![لقطة شاشة لواجهة استخراج الكيانات المسماة في مساحة اختبار "اللغة".](./media/entity-extraction.png)

    لاحظ في قسم *التفاصيل* كيف تأتي الكيانات المستخرجة مع معلومات إضافية مثل النوع ودرجات الثقة. تمثل درجة الثقة احتمالية أن ينتمي النوع الذي تم تحديده بالفعل إلى هذه الفئة.

### استخراج العبارات الرئيسية باستخدام Azure AI Language في مدخل Azure AI Foundry

*العبارات الرئيسية* هي أهم قطع المعلومات في النص. دعنا نستخدم قدرة استخراج العبارات الرئيسية في Azure AI Language لاستخراج معلومات مهمة من مراجعة.

1. في بيئة اللغة، حدد **استخراج المعلومات**. ثم حدد لوحة **استخراج العبارات الرئيسية**. 

1. ضمن خانة *النموذج*، أدخِل التقييم التالي:

    ```
    Good Hotel and staff
    The Royal Hotel, London, UK
    3/2/2018
    Clean rooms, good service, great location near Buckingham Palace and Westminster Abbey, and so on. We thoroughly enjoyed our stay. The courtyard is very peaceful and we went to a restaurant which is part of the same group and is Indian ( West coast so plenty of fish) with a Michelin Star. We had the taster menu which was fabulous. The rooms were very well appointed with a kitchen, lounge, bedroom and enormous bathroom. Thoroughly recommended.
    ```

1. حدد **تشغيل**. راجع الإخراج.

    ![لقطة شاشة لواجهة استخراج العبارات الرئيسية في مساحة اختبار "اللغة".](./media/key-phrases.png)

    لاحظ العبارات المختلفة المستخرجة في قسم *التفاصيل*. ينبغي أن تساهم هذه العبارات بشكل أكبر في معنى النص.

### تلخيص النص باستخدام Azure AI Language في مدخل Azure AI Foundry
 
دعونا نلقي نظرة على قدرات التلخيص الخاصة بـ Azure AI Language.

1. في بيئة اللغة، حدد **تلخيص المعلومات**، ثم حدد لوحة **تلخيص النص**.

1. ضمن خانة *النموذج*، أدخِل التقييم التالي:
    
    ```
    Very noisy and rooms are tiny
    The Lombard Hotel, San Francisco, USA
    9/5/2018
    Hotel is located on Lombard street which is a very busy SIX lane street directly off the Golden Gate Bridge. Traffic from early morning until late at night especially on weekends. Noise would not be so bad if rooms were better insulated but they are not. Had to put cotton balls in my ears to be able to sleep--was too tired to enjoy the city the next day. Rooms are TINY. I picked the room because it had two queen size beds--but the room barely had space to fit them. With family of four in the room it was tight. With all that said, rooms are clean and they've made an effort to update them. The hotel is in Marina district with lots of good places to eat, within walking distance to Presidio. May be good hotel for young stay-up-late adults on a budget
    ```

1. حدد **تشغيل**. راجع الإخراج.

    ![لقطة شاشة لواجهة تلخيص النصوص في مساحة اختبار "اللغة".](./media/summarize-text.png)

    لاحظ أن *الملخّص الاستخراجي* في *التفاصيل* يوفّر درجات تصنيف لأكثر الجُمل أهمية.

### تحليل التوجه في النص

يُعدّ تحليل التوجه مهمة شائعة عند تحليل النص مثل تقييمات الفنادق.

1. في مساحة اختبار "اللغة"، حدّد **تصنيف النص**. بعد ذلك، حدّد مربع **تحليل التوجه**.

1. ضمن خانة *النموذج*، أدخِل التقييم التالي:
    
    ```
    Disappointing Stay at The City Hotel
    The City Hotel, London
    9/5/2018
    My experience at The City Hotel in London was far from pleasant. The constant noise from nearby train tracks made it nearly impossible to sleep, with vibrations felt throughout the building. The rooms were outdated, dusty, and poorly maintained—dripping faucets, squeaky beds, and broken fixtures were just the beginning. Sound insulation was nonexistent, so every conversation from neighboring rooms was clearly audible. While the location near public transport was convenient and the staff were friendly, these positives couldn't make up for the overall discomfort and lack of value. I wouldn’t recommend this hotel to anyone seeking a restful or enjoyable stay.
    ```

1. حدد **تشغيل**. راجع الإخراج.

    ![لقطة شاشة لواجهة تحليل التوجه في مساحة اختبار "اللغة".](./media/sentiment-analysis.png)

    لاحظ أن التحليل يولّد تقييمًا عامًا للتوجه، فضلًا عن تقييمات منفصلة لكل جملة.

## الكشف عن اللغة وترجمة النص

تتيح خدمة Azure AI Language إمكانية كشف اللغة التي كُتب بها النص. بالإضافة إلى ذلك، تمكّنك خدمة Azure AI Translator من ترجمة النصوص بسهولة من لغة إلى أخرى.

### اكتشاف اللغة

لنبدأ بالكشف عن اللغة التي تتم كتابة التقييم بها.

1. في جزء **تصنيف النص**، حدّد مربع **الكشف عن اللغة**.

1. ضمن خانة *النموذج*، أدخِل التقييم التالي:
    
    ```
    Un séjour mémorable à l’Hôtel d’Ville
    l’Hôtel d’Ville, Paris
    9/5/2018
    J’ai passé un excellent séjour à l’Hôtel d’Ville à Paris. L’emplacement est idéal, en plein cœur de la ville, ce qui permet de découvrir facilement les principaux sites touristiques. Le personnel était chaleureux, professionnel et toujours prêt à aider. La chambre était propre, confortable et bien équipée, avec une vue charmante sur les rues parisiennes. Le petit-déjeuner était varié et délicieux, parfait pour commencer la journée. Je recommande vivement cet hôtel à tous ceux qui recherchent une expérience parisienne authentique et agréable.
    ```

1. حدد **تشغيل**. راجع الإخراج.

    ![لقطة شاشة لواجهة الكشف عن اللغة في مساحة اختبار "اللغة".](./media/detect-language.png)

    لاحظ أن اللغة المكتشفة هي الفرنسية. 

### ترجمة النص

دعونا نترجم الآن التقييم المكتوب بالفرنسية إلى اللغة الإنجليزية.

1. في أعلى الصفحة، اضغط على رابط **&larr;** (رجوع) بجوار عنوان صفحة **مساحة اختبار "اللغة"** لعرض جميع مساحات الاختبار المتوفرة.
1. في قائمة مساحات الاختبار، افتح **مساحة اختبار "المترجم"**.
1. في مساحة اختبار "المترجم"، حدّد **ترجمة النص**.
1. في جزء **التكوين**، حدّد خيارات اللغة التالية:
    - **ترجمة من اللغة**: الفرنسية
    - **ترجمة إلى اللغة**: الإنجليزية
1. ضمن خانة *نموذج*، أدخِل التقييم المكتوب باللغة الفرنسية:
    
    ```
    Un séjour mémorable à l’Hôtel d’Ville
    l’Hôtel d’Ville, Paris
    9/5/2018
    J’ai passé un excellent séjour à l’Hôtel d’Ville à Paris. L’emplacement est idéal, en plein cœur de la ville, ce qui permet de découvrir facilement les principaux sites touristiques. Le personnel était chaleureux, professionnel et toujours prêt à aider. La chambre était propre, confortable et bien équipée, avec une vue charmante sur les rues parisiennes. Le petit-déjeuner était varié et délicieux, parfait pour commencer la journée. Je recommande vivement cet hôtel à tous ceux qui recherchent une expérience parisienne authentique et agréable.
    ```

1. حدّد **ترجمة**. راجع الإخراج.

    ![لقطة شاشة لواجهة ترجمة النص في مساحة اختبار "المترجم".](./media/text-translation.png)

    لاحظ أن التقييم المكتوب بالفرنسية تم تحويله إلى الإنجليزية.

## تنظيف

إذا كنت لا تنوي إجراء المزيد من التدريبات، فاحذف أي موارد لم تعد بحاجة إليها. وهذا يتجنب تكبد أي تكاليف غير ضرورية.

1. افتح **بوابة Azure** في [https://portal.azure.com](https://portal.azure.com) وحدد مجموعة الموارد التي تحتوي على الموارد التي قمت بإنشائها.
1. حدّد **حذف مجموعة الموارد** ثم **أدخِل اسم مجموعة الموارد** للتأكيد. ثم يتم حذف مجموعة الموارد.

## معرفة المزيد

لمعرفة المزيد حول ما يمكنك القيام به مع هذه الخدمة، يرجى مراجعة[صفحة خدمة Language](https://learn.microsoft.com/azure/ai-services/language-service/overview).
