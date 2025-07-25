---
lab:
  title: تحليل الصور في مدخل Azure AI Foundry
---

# تحليل الصور في مدخل Azure AI Foundry

تتضمن **Azure AI Vision** العديد من القدرات لفهم محتوى الصورة والسياق واستخراج المعلومات من الصور. في هذا التمرين، ستستخدم Azure AI Vision في مدخل Azure AI Foundry، وهي منصة Microsoft لإنشاء التطبيقات الذكية، لتحليل الصور باستخدام التجارب المدمجة. 

افترض أن بائع التجزئة الوهمي *Northwind Traders* قرر تنفيذ "متجر ذكي"، حيث تراقب خدمات الذكاء الاصطناعي المتجر لتحديد العملاء الذين يحتاجون إلى المساعدة، وتوجيه الموظفين لمساعدتهم. باستخدام Azure AI Vision، يمكن تحليل الصور التي التقطتها الكاميرات في جميع أنحاء المتجر لتقديم أوصاف ذات مغزى لما تصوره.

## إنشاء مشروع في مدخل Azure AI Foundry

1. في متصفح الويب، افتح [مدخل Azure AI Foundry](https://ai.azure.com) على `https://ai.azure.com` وسجّل الدخول باستخدام بيانات اعتماد Azure الخاصة بك. أغلق أي تلميحات أو نوافذ تشغيل سريع التي يتم فتحها عند تسجيل الدخول لأول مرة. 

1. في المتصفح، انتقل إلى `https://ai.azure.com/managementCenter/allResources` وحدد **إنشاء**. ثم حدد خيار إنشاء *مورد مركز ذكاء اصطناعي* جديد.

1. في معالج *إنشاء مشروع*، أدخل اسمًا صالحًا لمشروعك، وإذا تم اقتراح مركز موجود، فحدد الخيار لإنشاء مركز *جديد*. 

1. وسّع *خيارات متقدمة* لتحديد الإعدادات التالية لمشروعك:
    - **اشتراك**: اشتراكك في Azure
    - **مجموعة الموارد**: أنشئ أو حدد مجموعة موارد
    - **المنطقة**: حدد أحد المواقع التالية:
        * شرق الولايات المتحدة
        * وسط فرنسا
        * وسط كوريا
        * أوروبا الغربية
        * غرب الولايات المتحدة

    انتظر حتى يتم إنشاء مشروعك ومركزك.

1. عند إنشاء المشروع، سيتم نقلك إلى صفحة *نظرة عامة* التي تحتوي على تفاصيل المشروع. حدد **خدمات الذكاء الاصطناعي** في القائمة اليسرى (قد تحتاج إلى توسيع القائمة بالنقر على الرمز العلوي لقراءة محتوياتها). 

1. في صفحة *خدمات الذكاء الاصطناعي*، حدد لوحة *الرؤية + المستند* لتجربة إمكانات المستندات والرؤية من الذكاء الاصطناعي في Azure

    ![لقطة شاشة للوحة Vision + Document في Azure AI Foundry.](./media/vision-document-tile.png)

## إنشاء تسميات توضيحية لصورة

دعنا نستخدم وظيفة تسمية الصور في Azure AI Vision لتحليل الصور الملتقطة بواسطة كاميرا في متجر *Northwind Traders*. تتوفر التسميات التوضيحية للصور من خلال ميزات **التسمية التوضيحية** و**التسميات التوضيحية الكثيفة** .

1. في صفحة *الرؤية + المستند*، مرّر لأسفل وحدد **الصورة** ضمن *عرض كل إمكانات الرؤية الأخرى*. ثم حدد لوحة **تسمية الصورة**.

    ![لقطة شاشة للوحة تسمية الصورة في قسم الصور في صفحة "الرؤية" و"المستندات".](./media/vision-image-captioning-tile.png)

1. في صفحة **إضافة تعليقات إلى الصور**، حدد المورد *خدمات الذكاء الاصطناعي في Azure* الذي قمت بإنشائه. 

1. في صفحة **إضافة تسميات توضيحية للصور**، راجع المورد الذي تتصل به والمدرج ضمن العنوان الفرعي **جرّبه**. يجب ألا تضطر إلى إجراء تغييرات. (*ملاحظة*: إذا لم تقم بتخصيص موقع مورد صالح في وقت سابق أثناء إنشاء المورد، فقد يُطلب منك إنشاء مورد جديد لخدمات الذكاء الاصطناعي في Azure موجود في منطقة صالحة. ستحتاج إلى إنشاء المورد الجديد لمواصلة النشاط العملي.)  

1. حدد [**https://aka.ms/mslearn-images-for-analysis**](https://aka.ms/mslearn-images-for-analysis) لتنزيل **image-analysis.zip**. افتح المجلد على الكمبيوتر وحدد موقع الملف المسمى **store-camera-1.jpg**؛ الذي يحتوي على الصورة التالية:

    ![صورة لأحد الوالدين باستخدام كاميرا الهاتف المحمول لالتقاط صورة لطفل في متجر](./media/analyze-images-vision/store-camera-1.jpg)

1. قم بتحميل صورة **store-camera-1.jpg** عن طريق سحبها إلى مربع **سحب الملفات وإفلاتها هنا**، أو عن طريق استعراضها على نظام الملفات.

1. لاحظ نص التسمية التوضيحية الذي تم إنشاؤها، مرئي في لوحة **السمات المكتشفة** على يمين الصورة.

    توفر وظيفة **التسمية التوضيحية** جملة إنجليزية واحدة يمكن للبشر قراءتها تصف محتوى الصورة.

1. بعد ذلك، استخدم الصورة نفسها لإجراء **تسمية توضيحية كثيفة**. عُد إلى صفحة **الرؤية + المستند** عن طريق تحديد سهم *الرجوع* في أعلى الصفحة. في صفحة *الرؤية + المستند*، حدد علامة التبويب **الصورة**، ثم حدد لوحة **التسميات التوضيحية الكثيفة**.

    تختلف ميزة **التسميات التوضيحية الكثيفة** عن إمكانية **التسمية التوضيحية** من حيث أنها توفر العديد من التسميات التوضيحية القابلة للقراءة من قبل الإنسان للصورة، واحدة تصف محتوى الصورة والأخرى، كل منها يغطي العناصر الأساسية المكتشفة في الصورة. يتضمن كل كائن تم اكتشافه مربع إحاطة، والذي يحدد إحداثيات البكسل داخل الصورة المقترنة بالعنصر.

1. مرر مؤشر الماوس فوق أحد التسميات التوضيحية في قائمة السمات **المكتشفة** ولاحظ ما يحدث داخل الصورة.

    ![يتم عرض الصورة والتسميات التوضيحية الخاصة بها.](./media/analyze-images-vision/dense-captioning.png)

    حرك مؤشر الماوس فوق التسميات التوضيحية الأخرى في القائمة، ولاحظ كيف ينتقل المربع المحيط في الصورة لتمييز جزء الصورة المستخدم لإنشاء التسمية التوضيحية.

## وضع علامات على الصور 

الميزة التالية التي ستجربها هي وظيفة *استخراج العلامات* . تستند علامات الاستخراج إلى آلاف الكائنات التي يمكن التعرف عليها، بما في ذلك الكائنات الحية والمناظر الطبيعية والإجراءات.

1. عُد إلى صفحة *الرؤية + المستند* في Azure AI Foundry، ثم حدد علامة التبويب **الصورة**، ثم حدد لوحة **استخراج العلامة الشائعة**.

1. افتح المجلد الذي يحتوي على الصور التي قمت بتنزيلها وحدد موقع الملف المسمى **store-image-2.jpg**، والذي يبدو كما يلي:

    ![صورة لشخص مع سلة تسوق في سوبر ماركت](./media/analyze-images-vision/store-camera-2.jpg)

1. قم بتحميل ملف **store-camera-2.jpg**.

1. راجع قائمة العلامات المستخرجة من الصورة ودرجة الثقة لكل منها في لوحة السمات المكتشفة. هنا درجة الثقة هي احتمال أن يصف نص السمة المكتشفة ما هو في الواقع في الصورة. لاحظ في قائمة العلامات أنه لا يتضمن الكائنات فقط، ولكن الإجراءات، مثل *التسوق* و*البيع* و*الوقوف*.

    ![لقطة شاشة للوحة كشف السمات في Vision Studio مع عرض النص ودرجات الثقة بجوار الصورة الأصلية.](./media/analyze-images-vision/detect-attributes.png)

## كشف الكائنات

في هذه المهمة، يمكنك استخدام ميزة **الكشف عن الكائنات** لتحليل الصور. الكشف عن الكائنات يكتشف ويستخرج مربعات الإحاطة استناداً إلى آلاف الكائنات التي يمكن التعرف عليها والكائنات الحية.

1. عُد إلى صفحة *الرؤية + المستند* في Azure AI Foundry، ثم حدد علامة التبويب **الصورة**، واختر لوحة **اكتشاف الكائنات الشائعة**.

1. افتح المجلد الذي يحتوي على الصور التي قمت بتنزيلها وحدد موقع الملف المسمى **store-camera-3.jpg**، والذي يبدو كما يلي:

    ![صورة لشخص يحمل عربة تسوق](./media/analyze-images-vision/store-camera-3.jpg)

1. قم بتحميل ملف **store-camera-3.jpg**.

1. في مربع **السمات المكتشفة**، لاحظ قائمة الكائنات المكتشفة ودرجات الثقة الخاصة بها.

1. مرر مؤشر الماوس فوق الكائنات في قائمة **السمات المكتشفة** لتمييز مربع إحاطة العنصر في الصورة.

1. حرك شريط تمرير **قيمة الحد** حتى يتم عرض قيمة 70 إلى يمين شريط التمرير. لاحظ ما يحدث للكائنات في القائمة. يحدد شريط تمرير الحد أنه يجب عرض الكائنات المحددة بدرجة ثقة أو احتمال أكبر من الحد فقط.

## تنظيف

إذا كنت لا تنوي إجراء المزيد من التدريبات، فاحذف أي موارد لم تعد بحاجة إليها. وهذا يتجنب تكبد أي تكاليف غير ضرورية.

1.  افتح [بوابة Azure]( https://portal.azure.com) وحدد مجموعة الموارد التي تحتوي على الموارد التي قمت بإنشائها. 
1.  حدد المورد وحدد **حذف** ثم **نعم** للتأكيد. من ثم يتم حذف المورد.

## معرفة المزيد

لمعرفة المزيد حول ما يمكنك القيام به بهذه الخدمة، راجع [صفحة Azure AI Vision](https://learn.microsoft.com/azure/ai-services/computer-vision/overview).
