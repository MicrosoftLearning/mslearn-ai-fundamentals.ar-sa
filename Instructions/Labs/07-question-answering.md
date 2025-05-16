<div class="Box-sc-g0xbh4-0 eoaCFS js-snippet-clipboard-copy-unpositioned undefined" data-hpc="true"><article class="markdown-body entry-content container-lg" itemprop="text"><div dir="rtl"><markdown-accessiblity-table data-catalyst=""><table>
  <thead>
  <tr>
  <th>lab</th>
  </tr>
  </thead>
  <tbody>
  <tr>
  <td><div dir="rtl"><table>
  <thead>
  <tr>
  <th>title</th>
  </tr>
  </thead>
  <tbody>
  <tr>
  <td><div dir="rtl">استخدم الإجابة على الأسئلة مع Language Studio</div></td>
  </tr>
  </tbody>
</table>
</div></td>
  </tr>
  </tbody>
</table></markdown-accessiblity-table>

<div class="markdown-heading" dir="rtl"><h1 tabindex="-1" class="heading-element" dir="rtl">استخدم الإجابة على الأسئلة مع Language Studio</h1><a id="user-content-استخدم-الإجابة-على-الأسئلة-مع-language-studio" class="anchor" aria-label="Permalink: استخدم الإجابة على الأسئلة مع Language Studio" href="#استخدم-الإجابة-على-الأسئلة-مع-language-studio"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="rtl">في هذا التمرين، ستستخدم Language Studio لإنشاء قاعدة معرفية من الأسئلة والأجوبة وتدريبها. سيأتي محتوى قاعدة المعرفة من صفحة الأسئلة المتداولة الحالية من موقع Margie’s Travel على الويب، وهي وكالة سفر وهمية. ثم ستستخدم Language Studio لمعرفة كيفية عملها عند استخدامها بواسطة العملاء.</p>
<p dir="rtl">تشتمل خدمة Azure AI Language على إمكانات <em>الإجابة على الأسئلة</em>، والتي ستستخدمها لإنشاء قاعدة معرفية. يمكن إنشاء قواعد المعرفة إما من خلال إدخال أزواج الأسئلة والأجوبة يدويًا، أو من مستند أو صفحة ويب موجودة. تريد Margie's Travel استخدام مستند الأسئلة المتداولة الموجود لديهم.</p>
<p dir="rtl">تتيح لك ميزة الإجابة على الأسئلة من خدمة اللغة إنشاء قاعدة معارف بسرعة، إما بإدخال أزواج الأسئلة والأجوبة أو من مستند موجود أو صفحة ويب. ويمكن بعد ذلك استخدام بعض قدرات معالجة اللغة الطبيعية المدمجة لتفسير الأسئلة والعثور على إجابات مناسبة.</p>
<div class="markdown-heading" dir="rtl"><h2 tabindex="-1" class="heading-element" dir="rtl">إنشاء مورد <em>Language</em></h2><a id="user-content-إنشاء-مورد-language" class="anchor" aria-label="Permalink: إنشاء مورد Language" href="#إنشاء-مورد-language"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="rtl">لاستخدام الإجابة على الأسئلة، تحتاج إلى مورد <strong>لغة</strong>.</p>
<ol dir="rtl">
<li>
<p dir="rtl">في علامة تبويب المستعرض، افتح مدخل Azure على <a href="https://portal.azure.com?azure-portal=true" rel="nofollow">https://portal.azure.com</a>، وسجل الدخول باستخدام حساب Microsoft المرتبط باشتراكك في Azure.</p>
</li>
<li>
<p dir="rtl">انقر فوق زر <strong>＋إنشاء مورد</strong> وابحث عن <em>خدمة اللغة</em>. حدد <strong>إنشاء</strong> خطة <strong>خدمة اللغة</strong>. سيتم نقلك إلى صفحة <strong>لتحديد ميزات إضافية</strong>. استخدم الإعدادات التالية:</p>
<ul dir="rtl">
<li><strong>تحديد ميزات إضافية</strong>:
<ul dir="rtl">
<li><strong>Default features</strong>: <em>احتفظ بالميزات الافتراضية</em>.</li>
<li><strong>Custom features</strong>: <em>حدد custom question answering</em>.</li>
</ul>
</li>
<li>حدد <strong>متابعة لإنشاء المورد الخاص بك</strong>
</li>
<a target="_blank" rel="noopener noreferrer" href="https://github.com/MicrosoftLearning/mslearn-ai-fundamentals/blob/main/Instructions/Labs/media/create-a-bot/create-language-service-resource.png"><img src="https://github.com/MicrosoftLearning/mslearn-ai-fundamentals/blob/main/Instructions/Labs/media/create-a-bot/create-language-service-resource.png" alt="إنشاء مورد خدمة اللغة مع تمكين الإجابة المخصصة على الأسئلة." style="max-width: 100%;"></a></li>
</ul>
</li>
<li>
<p dir="rtl">في الصفحة <strong>Create Language</strong>، حدد الإعدادات التالية:</p>
<ul dir="rtl">
<li><strong>تفاصيل المشروع</strong>
<ul dir="rtl">
<li><strong>الاشتراك</strong>: <em>اشتراك Azure الخاص بك</em>.</li>
<li><strong>مجموعة الموارد</strong>: <em>حدد مجموعة موارد موجودة أو أنشئ مجموعة موارد جديدة</em>.</li>
</ul>
</li>
<li><strong>تفاصيل المثيل</strong>
<ul dir="rtl">
<li><strong>المنطقة</strong>: <em>حدد منطقة. إذا كنت في شرق الولايات المتحدة، فاستخدم "شرق الولايات المتحدة 2"</em></li>
<li><strong>Name</strong>: <em>اسم فريد لمورد Language الخاص بك</em>.</li>
<li><strong>Pricing tier</strong>: S (1000 مكالمة في الدقيقة)</li>
</ul>
</li>
<li><strong>الإجابة عن السؤال المخصص</strong>
<ul dir="rtl">
<li><strong>Azure search region</strong>: <em>اختر أي موقع متوفر</em>.</li>
<li><strong>مستوى الأسعار الخاص ببحث Azure</strong>: F مجاني (3 فهارس) - (<em>إذا لم يكن هذا المستوى متاحًا، فاختَر Basic</em>)</li>
</ul>
</li>
<li><strong>إشعار الذكاء الاصطناعي المسؤول</strong>
<ul dir="rtl">
<li><strong>By checking this box I certify that I have reviewed and acknowledge the terms in the Responsible AI Notice</strong>: <em>محدد</em>.</li>
</ul>
</li>
</ul>
</li>
<li>
<p dir="rtl">حدد <strong>مراجعة وإنشاء</strong>، ثم حدد <strong>إنشاء</strong>. انتظر توزيع خدمة Language التي ستدعم قاعدة المعارف المخصصة للإجابة على الأسئلة.</p>
<blockquote>
<p dir="rtl"><strong>ملاحظة</strong> إذا وفرت بالفعل موارد <strong>Azure Cognitive Search</strong> في المستوى المجاني، فقد لا تسمح لك حصة الاستخدام بإنشاء مورد آخر. وفي هذه الحالة، حدد مستوى آخر غير <strong>Free F</strong>.</p>
</blockquote>
</li>
</ol>
<div class="markdown-heading" dir="rtl"><h2 tabindex="-1" class="heading-element" dir="rtl">إنشاء مشروع جديد</h2><a id="user-content-إنشاء-مشروع-جديد" class="anchor" aria-label="Permalink: إنشاء مشروع جديد" href="#إنشاء-مشروع-جديد"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<ol dir="rtl">
<li>
<p dir="rtl">في علامة تبويب مستعرض جديدة، افتح مدخل Language Studio في <a href="https://language.azure.com?azure-portal=true" rel="nofollow">https://language.azure.com</a>، ثم سجل الدخول باستخدام حساب Microsoft المقترن باشتراك Azure.</p>
</li>
<li>
<p dir="rtl">إذا طلب منك اختيار مورد Language، حدد الإعدادات التالية:</p>
<ul dir="rtl">
<li><strong>دليل Azure</strong>: <em>دليل Azure الذي يحتوي على اشتراكك</em>.</li>
<li><strong>اشتراك Azure</strong>: <em>اشتراكك في Azure</em>.</li>
<li><strong>مورد اللغة</strong>: <em>مورد اللغة الذي قمتَ بإنشائه مسبقًا</em>.</li>
</ul>
<p dir="rtl">إذا <em><strong>لم</strong></em> تتم مطالبتك باختيار مورد language، فقد يرجع ذلك إلى وجود موارد Language متعددة في اشتراكك؛ وفي هذه الحالة:</p>
<ol dir="rtl">
<li>في الشريط في الجزء العلوي إذا كانت الصفحة، حدد <strong>الإعدادات (⚙)</strong>.</li>
<li>في الصفحة <strong>Settings</strong> اعرض علامة التبويب <strong>Resources</strong>.</li>
<li>حدد مورد اللغة الذي أنشأته للتو، وانقر فوق <strong>مورد الانتقال</strong>.</li>
<li>في أعلى الصفحة، انقر فوق <strong>Language Studio</strong> للعودة إلى الصفحة الرئيسية في Language Studio.</li>
</ol>
</li>
<li>
<p dir="rtl">في أعلى مدخل Language Studio، في القائمة <strong>Create new</strong>، حدد <strong>Custom question answering</strong>.</p>
</li>
<p dir="auto"><a target="_blank" rel="noopener noreferrer" href="https://github.com/MicrosoftLearning/mslearn-ai-fundamentals/blob/main/Instructions/Labs/media/create-a-bot/create-custom-question-answering.png"><img src="https://github.com/MicrosoftLearning/mslearn-ai-fundamentals/blob/main/Instructions/Labs/media/create-a-bot/create-custom-question-answering.png" alt="الإجابة عن السؤال المخصص" style="max-width: 100%;"></a></p>
</li>
<li>
<p dir="rtl">في صفحة <strong>Choose language setting for resource <em>your resource</em></strong>، حدد <strong>I want to select the language when I create a project in this resource</strong> وانقر فوق <strong>Next</strong>.
</li>
<a target="_blank" rel="noopener noreferrer" href="https://github.com/MicrosoftLearning/mslearn-ai-fundamentals/blob/main/Instructions/Labs/media/create-a-bot/create-project.png"><img src="https://github.com/MicrosoftLearning/mslearn-ai-fundamentals/blob/main/Instructions/Labs/media/create-a-bot/create-project.png" alt="أريد تحديد اللغة" style="max-width: 100%;"></a></p>
</li>
<li>
<p dir="rtl">في الصفحة <strong>Enter basic information</strong> أدخل التفاصيل التالية وانقر فوق <strong>Next</strong>:</p>
<ul dir="rtl">
<li><strong>Language resource</strong>: <em>اختر مورد language الخاص بك</em>.</li>
<li><strong>Azure search resource</strong>: <em>اختر مورد بحث Azure الخاص بك</em>.</li>
<li><strong>الاسم:</strong> <code>MargiesTravel</code></li>
<li><strong>الوصف</strong>: <code>A simple knowledge base</code></li>
<li><strong>Source language</strong>: English</li>
<li><strong>الإجابة الافتراضية عند عدم إرجاع أي إجابة</strong>: <code>No answer found</code></li>
</ul>
</li>
<li>
<p dir="rtl">في صفحة <strong>مراجعة وإنهاء</strong>، حدد <strong>إنشاء مشروع</strong>.</p>
</li>
<li>
<p dir="rtl">سيتم نقلك إلى صفحة <strong>Manage sources</strong>. حدد <strong>＋Add source</strong> وحدد <strong>عناوين URL</strong>.</p>
</li>
<li>
<p dir="rtl">في المربع <strong>إضافة عناوين URL</strong>، حدد <strong>+ إضافة عنوان url</strong>. اكتب ما يلي وحدد <strong>Add all</strong>:</p>
<ul dir="rtl">
<li><strong>اسم URL</strong>: <code>MargiesKB</code></li>
<li><strong>URL</strong>: <code>https://raw.githubusercontent.com/MicrosoftLearning/mslearn-ai-fundamentals/main/data/natural-language/margies_faq.docx</code></li>
<li><strong>Classify file structure</strong>: <em>Auto-detect</em></li>
</ul>
</li>
<li>
<p dir="rtl">حدد <strong>إضافة الكل.</strong></p>
</li>
</ol>
</li>
<p dir="auto"><a target="_blank" rel="noopener noreferrer" href="https://github.com/MicrosoftLearning/mslearn-ai-fundamentals/blob/main/Instructions/Labs/media/create-a-bot/add-url.png"><img src="https://github.com/MicrosoftLearning/mslearn-ai-fundamentals/blob/main/Instructions/Labs/media/create-a-bot/add-url.png" alt="إضافة URL" style="max-width: 100%;"></a></p>
<div class="markdown-heading" dir="rtl"><h2 tabindex="-1" class="heading-element" dir="rtl">تحرير قاعدة المعرفة</h2><a id="user-content-تحرير-قاعدة-المعرفة" class="anchor" aria-label="Permalink: تحرير قاعدة المعرفة" href="#تحرير-قاعدة-المعرفة"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="rtl">تستند قاعدة معرفتك إلى التفاصيل الواردة في وثيقة الأسئلة الشائعة وبعض الردود المحددة مسبقا. يمكنك إضافة أزواج الأسئلة والأجوبة المخصصة لتكملتهم.</p>
<ol dir="rtl">
<li>قم بتوسيع اللوحة اليسرى وتحديد <strong>تحرير قاعدة المعارف</strong>. ثم حدد <strong>+</strong> لإضافة زوج أسئلة جديد.</li>
<li>في مربع الحوار <strong>إضافة زوج إجابات جديد على الأسئلة</strong>، وفي نوع <strong>السؤال</strong>، <code>Hello</code>وفي نوع <strong>الإجابة</strong>، <code>Hi</code>حدد <strong>تم</strong>.</li>
<li>قم بتوسيع <strong>الأسئلة البديلة</strong> وحدد <strong>+ إضافة سؤال بديل</strong>. ثم أدخِل <code>Hiya</code>كجملة بديلة لكلمة "مرحبًا".</li>
<li>في الجزء العلوي من جزء <strong>أزواج الإجابات على الأسئلة</strong>، حدد <strong>حفظ</strong> لحفظ قاعدة المعرفة الخاصة بك.</li>
</ol>
<div class="markdown-heading" dir="rtl"><h2 tabindex="-1" class="heading-element" dir="rtl">تدريب واختبار قاعدة المعارف</h2><a id="user-content-تدريب-واختبار-قاعدة-المعارف" class="anchor" aria-label="Permalink: تدريب واختبار قاعدة المعارف" href="#تدريب-واختبار-قاعدة-المعارف"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="rtl">الآن بعد أن أصبح لديك قاعدة معارف، يمكنك اختبارها.</p>
<ol dir="rtl">
<li>
<p dir="rtl">في الجزء العلوي من جزء <strong>أزواج الإجابات على الأسئلة</strong>، حدد <strong>اختبار</strong> لاختبار قاعدة المعرفة الخاصة بك.</p>
</li>
<li>
<p dir="rtl">في جزء الاختبار، أدخل في الجزء السفلي رسالة تقول <code>Hi</code>. يجب أن تتم الاستجابة لقولك <em>مرحبًا</em>.</p>
</li>
<li>
<p dir="rtl">في جزء الاختبار، أدخل في الجزء السفلي رسالة تقول <code>I want to book a flight</code>. يجب إرجاع رد مناسب من الأسئلة الشائعة.</p>
<blockquote>
<p dir="rtl"><strong>ملاحظة</strong> يتضمن الرد <em>إجابة قصيرة</em> بالإضافة إلى <em>مقطع إجابة</em> مطول أكثر - يظهر مقطع الإجابة النص الكامل في مستند FAQ لأقرب سؤال مطابق، في حين يتم استخراج الإجابة القصيرة بذكاء من المقطع. يمكنك التحكم فيما إذا كانت الإجابة القصيرة واردة من الاستجابة باستخدام خانة الاختيار <strong>«عرض إجابة قصيرة»</strong> أعلى جزء الاختبار.</p>
</blockquote>
</li>
<li>
<p dir="rtl">جرّب سؤالاً آخر، مثل <code>How can I cancel a reservation?</code></p>
</li>
<li>
<p dir="rtl">عند الانتهاء من اختبار قاعدة المعرفة، حدد <strong>اختبار</strong> لإغلاق جزء الاختبار.</p>
</li>
</ol>
<div class="markdown-heading" dir="rtl"><h2 tabindex="-1" class="heading-element" dir="rtl">نشر مشروعك</h2><a id="user-content-نشر-مشروعك" class="anchor" aria-label="Permalink: نشر مشروعك" href="#نشر-مشروعك"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="rtl">بإمكانك توزيع قاعدة المعارف (KB) كتطبيق عميل للإجابة على الأسئلة.</p>
<ol dir="rtl">
<li>في اللوحة اليسرى، حدد <strong>نشر قاعدة المعارف</strong>.</li>
<li>في أعلى الصفحة، حدد <strong>نشر</strong>. سيسألك مربع حوار عما إذا كنت تريد نشر المشروع. حدد <strong>نشر</strong>.</li>
</ol>
</li>
<p dir="auto"><a target="_blank" rel="noopener noreferrer" href="https://github.com/MicrosoftLearning/mslearn-ai-fundamentals/blob/main/Instructions/Labs/media/create-a-bot/deploy-knowledge-base.png"><img src="https://github.com/MicrosoftLearning/mslearn-ai-fundamentals/blob/main/Instructions/Labs/media/create-a-bot/deploy-knowledge-base.png" alt="انشر قاعدة المعارف." style="max-width: 100%;"></a></p>
<div class="markdown-heading" dir="rtl"><h2 tabindex="-1" class="heading-element" dir="rtl">تنظيف</h2><a id="user-content-تنظيف" class="anchor" aria-label="Permalink: تنظيف" href="#تنظيف"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="rtl">إذا كنت لا تنوي إجراء المزيد من التدريبات، فاحذف أي موارد لم تعد بحاجة إليها. وهذا يتجنب تراكم أي تكاليف غير ضرورية.</p>
<ol dir="rtl">
<li>افتح <a href="https://portal.azure.com" rel="nofollow">مدخل Azure</a> وحدد مجموعة الموارد التي تحتوي على المورد الذي أنشأته.</li>
<li>حدد المورد وحدد <strong>حذف</strong> ثم <strong>نعم</strong> للتأكيد. من ثم يتم حذف المورد.</li>
</ol>
<div class="markdown-heading" dir="rtl"><h2 tabindex="-1" class="heading-element" dir="rtl">معرفة المزيد</h2><a id="user-content-معرفة-المزيد" class="anchor" aria-label="Permalink: معرفة المزيد" href="#معرفة-المزيد"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<ul dir="rtl">
<li>لمعرفة المزيد عن خدمة Question Answering، راجع <a href="https://docs.microsoft.com/azure/cognitive-services/language-service/question-answering/overview" rel="nofollow">الوثائق</a>.</li>
</ul>
</article></div>
