---
lab:
  title: تحليل النص في مدخل Azure AI Foundry
---

# تحليل النص في مدخل Azure AI Foundry

معالجة اللغات الطبيعية (NLP) هي فرع من فروع الذكاء الاصطناعي الذي يتعامل مع اللغة المكتوبة والمنطوقة. يمكنك استخدام البرمجة اللغوية العصبية لبناء حلول تستخرج المعنى الدلالي من النص أو الكلام، أو تصوغ استجابات ذات معنى باللغة الطبيعية.

تتضمن خدمة Azure AI Language تحليلات النصوص، مع إمكانيات مثل التعرف على الكيان، واستخراج العبارات الرئيسية، والتلخيص، وتحليل المشاعر. على سبيل المثال، لنفترض أن وكيل السفر الوهمي Margie's Travel يشجع العملاء على إرسال تقييمات للإقامات في الفنادق. بإمكانك استخدام خدمة "اللغة" لاستخراج الكيانات المسماة، وتحديد العبارات الرئيسية، وتلخيص النص، والمزيد.

في هذا التمرين، ستستخدم Azure AI Language في مدخل Azure AI Foundry، وهي منصة Microsoft لإنشاء التطبيقات الذكية، لتحليل مراجعات الفنادق. 

يستغرق هذا التدريب حوالي **20** دقيقة.

## إنشاء مشروع في مدخل Azure AI Foundry

1. في متصفح الويب، افتح [مدخل Azure AI Foundry](https://ai.azure.com) على `https://ai.azure.com` وسجّل الدخول باستخدام بيانات اعتماد Azure الخاصة بك. أغلق أي تلميحات أو نوافذ تشغيل سريع التي يتم فتحها عند تسجيل الدخول لأول مرة. 

1. في المتصفح، انتقل إلى `https://ai.azure.com/managementCenter/allResources` وحدد **إنشاء جديد**. بعد ذلك، حدّد خيار إنشاء **مورد Azure AI Foundry**.

1. في المعالج *إنشاء مشروع*، أدخل اسمًا صالحًا لمشروعك.

1. وسّع *خيارات متقدمة* لتحديد الإعدادات التالية لمشروعك:
    - **اشتراك**: اشتراكك في Azure
    - **مجموعة الموارد**: أنشئ أو حدد مجموعة موارد
    - **المنطقة**: حدد أحد المواقع التالية:
        * شرق الولايات المتحدة
        * وسط فرنسا
        * وسط كوريا
        * أوروبا الغربية
        * غرب الولايات المتحدة

    حدد **إنشاء**. انتظر حتى يتم إنشاء مشروعك. قد يستغرق ذلك بضع دقائق.

1. عند إنشاء المشروع، سيتم نقلك إلى صفحة *نظرة عامة* التي تحتوي على تفاصيل المشروع.

1. في القائمة الموجودة على الجانب الأيسر من الشاشة، حدد **البيئات**. 

    >*ملاحظة*: قُم بتوسيع القائمة لقراءة محتوياتها من خلال النقر على أيقونة "توسيع" في الأعلى.

1. في صفحة مساحات الاختبار الخاصة بـ Azure AI Foundry، حدّد **تجربة مساحة اختبار اللغة**. تُعدّ مساحة اختبار اللغة واجهة مستخدم تتيح لك تجربة بعض إمكانيات Azure AI Language.  

## استخراج الكيانات المسماة باستخدام Azure AI Language في مدخل Azure AI Foundry

*الكيانات المسماة* هي كلمات تصف الأشخاص والأماكن والأشياء بأسماء مناسبة. دعنا نستخدم إمكانية استخراج الكيان المسمى في Azure AI Language لتحديد أنواع المعلومات في المراجعة.

1. في بيئة اللغة، حدد **استخراج المعلومات**. ثم حدد لوحة **استخراج الكيانات المسماة**. 

1. تحت *العينة*، انسخ والصق المراجعة التالية:

    ```
    Tired hotel with poor service
    The Royal Hotel, London, United Kingdom
    5/6/2018
    This is an old hotel (has been around since 1950's) and the room furnishings are average - becoming a bit old now and require changing. The internet didn't work and had to come to one of their office rooms to check in for my flight home. The website says it's close to the British Museum, but it's too far to walk.
    ```

1. حدد **تشغيل**. راجع الإخراج. لاحظ في قسم *التفاصيل* كيف تأتي الكيانات المستخرجة مع معلومات إضافية مثل النوع ودرجات الثقة. تمثل درجة الثقة احتمالية أن ينتمي النوع الذي تم تحديده بالفعل إلى هذه الفئة.

## استخراج العبارات الرئيسية باستخدام Azure AI Language في مدخل Azure AI Foundry

*العبارات الرئيسية* هي أهم قطع المعلومات في النص. دعنا نستخدم قدرة استخراج العبارات الرئيسية في Azure AI Language لاستخراج معلومات مهمة من مراجعة.

1. في بيئة اللغة، حدد **استخراج المعلومات**. ثم حدد لوحة **استخراج العبارات الرئيسية**. 

1. تحت *العينة*، انسخ والصق المراجعة التالية:

    ```
    Good Hotel and staff
    The Royal Hotel, London, UK
    3/2/2018
    Clean rooms, good service, great location near Buckingham Palace and Westminster Abbey, and so on. We thoroughly enjoyed our stay. The courtyard is very peaceful and we went to a restaurant which is part of the same group and is Indian ( West coast so plenty of fish) with a Michelin Star. We had the taster menu which was fabulous. The rooms were very well appointed with a kitchen, lounge, bedroom and enormous bathroom. Thoroughly recommended.
    ```

1. حدد **تشغيل**. راجع الإخراج. لاحظ العبارات المختلفة المستخرجة في قسم *التفاصيل*. ينبغي أن تساهم هذه العبارات بشكل أكبر في معنى النص.

## تلخيص النص باستخدام Azure AI Language في مدخل Azure AI Foundry
 
1. دعونا نلقي نظرة على قدرات التلخيص الخاصة بـ Azure AI Language. في بيئة اللغة، حدد *تلخيص المعلومات*، ثم حدد لوحة **تلخيص النص**.

1. تحت *العينة*، انسخ والصق المراجعة التالية:
    
    ```
    Very noisy and rooms are tiny
    The Lombard Hotel, San Francisco, USA
    9/5/2018
    Hotel is located on Lombard street which is a very busy SIX lane street directly off the Golden Gate Bridge. Traffic from early morning until late at night especially on weekends. Noise would not be so bad if rooms were better insulated but they are not. Had to put cotton balls in my ears to be able to sleep--was too tired to enjoy the city the next day. Rooms are TINY. I picked the room because it had two queen size beds--but the room barely had space to fit them. With family of four in the room it was tight. With all that said, rooms are clean and they've made an effort to update them. The hotel is in Marina district with lots of good places to eat, within walking distance to Presidio. May be good hotel for young stay-up-late adults on a budget
    ```

1. حدد **تشغيل**. راجع الإخراج. لاحظ أن *الملخّص الاستخراجي* في *التفاصيل* يوفّر درجات تصنيف لأكثر الجُمل أهمية.   

## تنظيف

إذا كنت لا تنوي إجراء المزيد من التدريبات، فاحذف أي موارد لم تعد بحاجة إليها. وهذا يتجنب تكبد أي تكاليف غير ضرورية.

1. افتح **بوابة Azure** في [https://portal.azure.com](https://portal.azure.com) وحدد مجموعة الموارد التي تحتوي على الموارد التي قمت بإنشائها.

1. حدد الموارد ثم حدد **حذف** ثم **نعم** للتأكيد. سيتم بعد ذلك حذف الموارد.

## معرفة المزيد

لمعرفة المزيد حول ما يمكنك القيام به مع هذه الخدمة، يرجى مراجعة[صفحة خدمة Language](https://learn.microsoft.com/azure/ai-services/language-service/overview).
