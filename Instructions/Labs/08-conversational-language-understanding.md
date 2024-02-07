---
lab:
  title: استخدام فهم لغة المحادثة مع Language Studio
---

# استخدام فهم لغة المحادثة مع Language Studio

بشكل متزايد، نتوقع أن تكون أجهزة الكمبيوتر قادرة على استخدام الذكاء الاصطناعي لفهم أوامر اللغة الطبيعية، إما منطوقة أو مكتوبة. على سبيل المثال، قد ترغب في أن يتحكم نظام أتمتة المنزل في الأجهزة في منزلك باستخدام الأوامر الصوتية مثل "تشغيل الضوء" أو "تشغيل المروحة". يمكن للأجهزة التي تعمل بالطاقة الذكاء الاصطناعي فهم هذه الأوامر واتخاذ الإجراء المناسب.

في هذا التمرين، ستستخدم Language Studio لإنشاء واختبار مشروع يرسل إرشادات إلى أجهزة مثل الأضواء أو المشجعين. ستستخدم قدرات خدمة Conversational Language Understanding لتكوين مشروعك. 

## إنشاء مورد *Language*

يمكنك استخدام العديد من ميزات Azure الذكاء الاصطناعي Language مع مورد **خدمات** Language** أو **Azure الذكاء الاصطناعي. هناك بعض المثيلات التي يمكن فيها استخدام مورد Language فقط. للتمرين أدناه، سنستخدم **مورد Language** . إذا لم تكن قد فعلت ذلك بالفعل، بادر بإنشاء مورد **Language** في اشتراك Azure خاصتك.

1. في علامة تبويب مستعرض أخرى، افتح مدخل Microsoft Azure في [https://portal.azure.com](https://portal.azure.com?azure-portal=true)، وقم بتسجيل الدخول باستخدام حساب Microsoft المقترن باشتراك Azure الخاص بك.

1. **انقر فوق &65291; أنشئ زر مورد** وابحث عن *خدمة* Language. حدد **create** a **Language service** plan. سيتم نقلك إلى صفحة إلى *Select additional features**. احتفظ بالتحديد الافتراضي وانقر فوق **متابعة لإنشاء المورد** الخاص بك. 

1. في الصفحة **إنشاء لغة**، قم بتكوينها بالإعدادات التالية:
    - **الاشتراك**: *اشتراك Azure الخاص بك*.
    - **مجموعة الموارد**: *أنشئ مجموعة موارد جديدة ذات اسم فريد*.
    - **المنطقة**: شرق الولايات المتحدة.
    - **الاسم**: *أدخل اسمًا مميزًا*.
    - **مستوى** التسعير: *F0 أو S مجاني إذا لم يكن F0 مجانيا متوفرا*
    - **من خلال تحديد هذا المربع، أقر بأنني قرأت وفهمت جميع المصطلحات أدناه**: *محددة*.

1. حدد **Review + create** ثم **Create** وانتظر حتى يكتمل النشر.


### إنشاء تطبيق Conversational Language Understanding

لفهم اللغة الطبيعية باستخدام تطبيق Conversational Language Understanding، يمكنك إنشاء التطبيق، ثم إضافة الكيانات والأهداف والألفاظ لتحديد الأوامر التي تريد التطبيق.

1. في علامة تبويب مستعرض جديدة، افتح مدخل Language Studio في [https://language.azure.com](https://language.azure.com?azure-portal=true)، ثم سجل الدخول باستخدام حساب Microsoft المقترن باشتراك Azure.

1. إذا طلب منك اختيار مورد Language، حدد الإعدادات التالية:
    - **دليل** Azure: *دليل Azure الذي يحتوي على اشتراكك*.
    - **اشتراك** Azure: *اشتراك* Azure الخاص بك.
    - **مورد** اللغة: *مورد اللغة الذي قمت بإنشائه مسبقا.*

   إذا ***لم*** تتم مطالبتك باختيار مورد language، فقد يرجع ذلك إلى وجود موارد Language متعددة في اشتراكك؛ وفي هذه الحالة:
    1. في الشريط في الجزء العلوي إذا كانت الصفحة، حدد **الإعدادات (&9881;)**.
    2. في الصفحة **Settings** اعرض علامة التبويب **Resources**.
    3. حدد مورد اللغة الذي أنشأته للتو، وحدد **تبديل المورد**.
    4. في أعلى الصفحة، حدد **Language Studio** للعودة إلى الصفحة الرئيسية ل Language Studio.

1. في الجزء العلوي من المدخل، في قائمة **Create new**، حدد **Conversational Language Understanding**.

1. في **مربع الحوار إنشاء مشروع** ، في **صفحة إدخال المعلومات** الأساسية، أدخل التفاصيل التالية وحدد **التالي**:
    - **الاسم**: *إنشاء اسم فريد*
    - **الألفاظ اللغة** الأساسية: *الإنجليزية*
    - **Enable multiple languages in project**: *Do not select*
    - **الوصف**: `Simple home automation`

    > **تلميح**: دون اسم* مشروعك*، ستستخدمه لاحقا.

1. في صفحة Review **and finish** ، حدد **Create**.

### إنشاء المقاصد والأقوال والكيانات

يعد *الهدف* عبارة عن إجراء تريد تنفيذه، على سبيل المثال، قد ترغب في تشغيل مصباح أو إيقاف تشغيل مروحة. في هذه الحالة، ستحدد هدفين: أحدهما لتشغيل الجهاز والآخر لإيقاف تشغيل الجهاز. لكل قصد، عليك تحديد نماذج التعبيرات التي تشير إلى *الأقوال* المستخدمة للإشارة إلى تحقيق النية.

1. في جزء تعريف** المخطط، تأكد من **تحديد Intents** ثم حدد **Add**، وأضف هدفا بالاسم `switch_on` (في حالة صغيرة) وحدد **Add intent**.**

    ![حدد add ضمن Intents في جزء Build Schema.](media/conversational-language-understanding/build-schema.png)

    ![أضف الهدف switch_on ثم حدد Add intent.](media/conversational-language-understanding/add-intent.png)

1. انقر فوق الهدف **switch_on**. سينقلك إلى صفحة **Data labeling**. في القائمة المنسدلة **Intent**، حدد **switch_on**. بجوار **الهدف switch_on** ، اكتب التعبير `turn the light on` واضغط **على Enter** لإرسال هذا التعبير إلى القائمة.

    ![أضف تعبيرًا إلى مجموعة التدريب عن طريق الكتابة في "turn the light on" ضمن Utterance.](media/conversational-language-understanding/add-utterance-on.png)

1. تحتاج خدمة Language إلى خمسة أمثلة ألفاظ مختلفة على الأقل لكل هدف لتدريب نموذج اللغة بشكل كافٍ. أضف أربعة أمثلة لفظية أخرى إلى هدف **switch_on**:  
    - `switch on the fan`
    - `put the fan on`
    - `put the light on`
    - `switch on the light`
    - `turn the fan on`

1. في جزء **Labeling entities for training** على الجانب الأيمن من الشاشة، حدد **Labels**، ثم حدد **Add entity**. اكتب `device` (في حالة صغيرة)، وحدد **قائمة** وحدد **إضافة كيان**.

    ![أضف كيانًا عن طريق تحديد Tags على Tagging entities for training panel، ثم حدد Add entity.](media/conversational-language-understanding/add-entity.png)

    ![اكتب device ضمن Entity name وحدد List، ثم حدد Add entity.](media/conversational-language-understanding/add-entity-device.png)

1. عند نطق ***turn the fan on*** ميز الكلمة "fan". ثم في القائمة التي تظهر، في المربع *Search for an entity* حدد **device**.

    ![ميّز الكلمة fan في utterance وحدد device.](media/conversational-language-understanding/switch-on-entity.png)

1. افعل الشيء نفسه مع جميع الأقوال. ضع علامة على بقية *fan* أو العبارات *الخفيفة* باستخدام كيان **device**. عند الانتهاء، تحقق من أن لديك الألفاظ التالية وانقر فوق **Save changes**:

    | **intent** | **utterance** | **كيان** |
    | --------------- | ------------------ | ------------------ |
    | switch_on   | وضع المروحة في حالة التشغيل      | الجهاز - *select fan* |
    | switch_on   | إشعال المصباح    | الجهاز - *select light* |
    | switch_on   | تشغيل المصباح | الجهاز - *select light* |
    | switch_on   | تشغيل المروحة     | الجهاز - *select fan* |
    | switch_on   | تشغيل المروحة   | الجهاز - *select fan* |
    | switch_on   | إضاءة المصباح   | الجهاز - *select light* |

    ![بعد الانتهاء، حدد Save changes.](media/conversational-language-understanding/save-changes.png) 

1. في الجزء الموجود على اليسار، حدد **تعريف** المخطط وتحقق من **إدراج هدف switch_on** . ثم حدد **إضافة** وإضافة هدف جديد بالاسم `switch_off` (بأحرف صغيرة).

    ![ارجع إلى شاشة Build Schema وأضف الهدف switch_off.](media/conversational-language-understanding/add-switch-off.png) 

1. **حدد الهدف switch_off**. سينقلك إلى صفحة **Data labeling**. في القائمة المنسدلة **Intent**، حدد **switch_off**. بجوار **الهدف switch_off** ، أضف التعبير `turn the light off`.

1. أضف خمسة أمثلة لفظية أخرى إلى هدف **switch_off**.
    - `switch off the fan`
    - `put the fan off`
    - `put the light off`
    - `turn off the light`
    - `switch the fan off`

1. ضع علامة على الكلمات *الخفيفة* أو *fan* باستخدام كيان **device**. عند الانتهاء، تحقق من أن لديك الألفاظ التالية وانقر فوق **Save changes**:  

    | **intent** | **utterance** | **كيان** | 
    | --------------- | ------------------ | ------------------ |
    | switch_off   | وضع المروحة في حالة إيقاف التشغيل    | الجهاز - *select fan* | 
    | switch_off   | إطفاء المصباح  | الجهاز - *select light* |
    | switch_off   | إيقاف تشغيل المصباح | الجهاز - *select light* |
    | switch_off   | إيقاف المروحة | الجهاز - *select fan* |
    | switch_off   | إيقاف تشغيل المروحة | الجهاز - *select fan* |
    | switch_off   | إيقاف إضاءة المصباح | الجهاز - *select light* |

### التدريب على النموذج

الآن أنت مستعد لاستخدام المقاصد والكيانات التي حددتها لتدريب نموذج لغة المحادثة لتطبيقك.

1. على الجانب الأيسر من Language Studio، حدد **Training jobs**، ثم حدد **Start a training job**. استخدم الإعدادات التالية:
    - **Train a new model**: *Selected and choose a model name*
    - **وضع التدريب**: تدريب قياسي (مجاني)
    - **تقسيم البيانات**: *حدد تقسيم مجموعة الاختبارات تلقائياً من بيانات التدريب، واحتفظ بالنسب المئوية الافتراضية*
    - حدد **تدريب** في أسفل الصفحة.

1. انتظر حتى يكتمل التدريب.

### نشر النموذج واختباره

لاستخدام النموذج المدرَّب في تطبيق العميل، يجب عليك نشره كنقطة نهاية يمكن لتطبيقات العميل أن ترسل إليها ألفاظ جديدة؛ من خلالها سيتم توقع الأهداف والكيانات.

1. على الجانب الأيسر من Language Studio، حدد **Deploying a model**.

1. حدد اسم النموذج الخاص بك ثم **أضف التوزيع**. استخدم الإعدادات التالية:
    - **Create or select an existing deployment name**: *حدد create a new deployment name. أضف اسم فريد*.
    - **Assign trained model to your deployment name**: * حدد اسم النموذج المدرب*.
    - حدد **Deploy**

    > **تلميح**: لاحظ اسم* النشر الخاص بك*، ستستخدمه لاحقا. 

1. عند نشر النموذج، حدد **Testing deployments** على الجانب الأيسر من الصفحة، ثم حدد النموذج المنشور ضمن **Deployment name**.

1. أدخل النص التالي، ثم حدد **Run the test**:

    `switch the light on`

    ![اختبر النموذج الخاص بك عن طريق تحديد النموذج الموزع، ثم أدخل النص وحدد Run the test.](media/conversational-language-understanding/test-model.png) 

    راجع النتيجة التي تم إرجاعها، مع ملاحظة أنها تتضمن الهدف المتوقع (الذي يجب أن يكون **switch_on**) والكيان المتوقع (**device**) مع درجات الثقة التي تشير إلى احتمال احتساب النموذج لـ الهدف والكيان المتوقعين. تُظهر علامة التبويب JSON الثقة النسبية لكل هدف محتمل (الهدف الذي يتمتع بأعلى درجة ثقة هو الهدف المتوقع)

1. امسح مربع النص واختبر النموذج من خلال الألفاظ التالية ضمن *Enter your own text, or upload a text document*:
    - `turn off the fan`
    - `put the light on`
    - `put the fan off`

لقد قمت الآن بتكوين مشروع لغة محادثة بنجاح، وكيانات محددة، والأهداف، والألفاظ. لقد رأيت كيفية تدريب نموذج ونشره في Language Studio. وقد جربت ذلك بكلا التعبيرين اللذين حددتهما، وبعض الكلمات التي لم تحددها صراحة ولكن النموذج كان قادرا على تحديدها.

> **ملاحظة**: يوفر فهم لغة المحادثة التحليل الذكي لتفسير هدف الإدخال؛ ولا يقوم بأي إجراءات مثل تشغيل الضوء أو المروحة. سيحتاج المطور إلى إنشاء تطبيق يستخدم نموذج Conversational Language Understanding لتحديد هدف المستخدم، ثم أتمتة الإجراء المناسب.

## تنظيف

إذا كنت لا تنوي إجراء المزيد من التدريبات، فاحذف أي موارد لم تعد بحاجة إليها. وهذا يتجنب تراكم أي تكاليف غير ضرورية.

1.افتح مدخل []( https://portal.azure.com) Microsoft Azure وحدد مجموعة الموارد التي تحتوي على المورد الذي أنشأته. 1.حدد المورد وحدد **حذف** ثم **نعم** للتأكيد. ثم يتم حذف المورد.

## معرفة المزيد

لا يعرض هذا التطبيق سوى بعض إمكانات ميزة Conversational Language Understanding في خدمة Language. لمعرفة المزيد حول ما يمكنك القيام به مع هذه الخدمة، راجع [صفحة Conversational Language Understanding](https://docs.microsoft.com/azure/cognitive-services/language-service/conversational-language-understanding/overview).
