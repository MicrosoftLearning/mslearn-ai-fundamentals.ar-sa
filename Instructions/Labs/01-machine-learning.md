<div class="Box-sc-g0xbh4-0 eoaCFS js-snippet-clipboard-copy-unpositioned undefined" data-hpc="true"><article class="markdown-body entry-content container-lg" itemprop="text"><div dir="auto"><div dir="rtl"><markdown-accessiblity-table data-catalyst=""><table>
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
  <td><div dir="rtl">استكشاف التعلُّم الآلي التلقائي ي Azure Machine Learning</div></td>
  </tr>
  </tbody>
</table>
</div></td>
  </tr>
  </tbody>
</table></markdown-accessiblity-table>
<div dir="rtl"><div dir="rtl"><div class="markdown-heading" dir="auto"><h1 tabindex="-1" dir="rtl" class="heading-element">استكشاف التعلُّم الآلي التلقائي ي Azure Machine Learning</h1><a id="user-content-استكشاف-التعلُّم-الآلي-التلقائي-ي-azure-machine-learning" class="anchor" aria-label="Permalink: استكشاف التعلُّم الآلي التلقائي ي Azure Machine Learning" href="#استكشاف-التعلُّم-الآلي-التلقائي-ي-azure-machine-learning"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div><a id="user-content-استكشاف-التعلُّم-الآلي-التلقائي-ي-azure-machine-learning" aria-label="Permalink: استكشاف التعلُّم الآلي التلقائي ي Azure Machine Learning" href="#استكشاف-التعلُّم-الآلي-التلقائي-ي-azure-machine-learning"></a></div><a id="user-content-استكشاف-التعلُّم-الآلي-التلقائي-ي-azure-machine-learning" aria-label="Permalink: استكشاف التعلُّم الآلي التلقائي ي Azure Machine Learning" href="#استكشاف-التعلُّم-الآلي-التلقائي-ي-azure-machine-learning"></a></div>
<p dir="rtl">في هذا التمرين، ستستخدم ميزة التعلّم الآلي التلقائي في التعلّم الآلي في Azure لتدريب نموذج التعلم الآلي وتقييمه. ثم ستقوم بنشر النموذج المُدرّب واختباره.</p>
<p dir="rtl">يجب أن يستغرق هذا التمرين حوالي <strong>35</strong> دقيقة لإكماله.</p>
<div dir="rtl"><div dir="rtl"><div class="markdown-heading" dir="auto"><h2 tabindex="-1" dir="rtl" class="heading-element">إنشاء مساحة عمل "التعلم الآلي من Azure"</h2><a id="user-content-إنشاء-مساحة-عمل-التعلم-الآلي-من-azure" class="anchor" aria-label="Permalink: إنشاء مساحة عمل &quot;التعلم الآلي من Azure&quot;" href="#إنشاء-مساحة-عمل-التعلم-الآلي-من-azure"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div><a id="user-content-إنشاء-مساحة-عمل-التعلم-الآلي-من-azure" aria-label="Permalink: إنشاء مساحة عمل &quot;التعلم الآلي من Azure&quot;" href="#إنشاء-مساحة-عمل-التعلم-الآلي-من-azure"></a></div><a id="user-content-إنشاء-مساحة-عمل-التعلم-الآلي-من-azure" aria-label="Permalink: إنشاء مساحة عمل &quot;التعلم الآلي من Azure&quot;" href="#إنشاء-مساحة-عمل-التعلم-الآلي-من-azure"></a></div>
<p dir="rtl">لاستخدام التعلّم الآلي في Azure، تحتاج إلى توفير مساحة عمل تعلّم آلي في Azure في اشتراك Azure الخاص بك. ثم ستتمكن من استخدام استوديو التعلّم الآلي في Azure للعمل مع الموارد في مساحة العمل الخاصة بك.</p>
<blockquote>
<p dir="rtl"><strong>تلميح</strong>: إذا كان لديك بالفعل مساحة عمل التعلّم الآلي في Azure، يمكنك استخدام ذلك والتخطي إلى المهمة التالية.</p>
</blockquote>
<ol dir="rtl">
<li>
<p dir="rtl">سجل الدخول إلى <a href="https://portal.azure.com" rel="nofollow">مدخل Azure</a> في <code>https://portal.azure.com</code> باستخدام بيانات اعتماد Microsoft الخاصة بك.</p>
</li>
<li>
<p dir="rtl">حدد <strong>＋إنشاء مورد</strong>، وابحث عن <em>التعلّم الآلي</em>، وقم بإنشاء مورد <strong>تعلّم آلي</strong> جديد بالإعدادات التالية:</p>
<ul dir="rtl">
<li><strong>الاشتراك</strong>: <em>اشتراك Azure الخاص بك</em>.</li>
<li><strong>Resource group</strong>: <em>أنشئ مجموعة موارد أو حددها</em>.</li>
<li><strong>الاسم</strong>: <em>أدخل اسم فريد لمساحة العمل الخاصة بك</em>.</li>
<li><strong>المنطقة</strong>: شرق الولايات المتحدة</li>
<li><strong>Storage account</strong>: <em>لاحظ حساب التخزين الجديد الافتراضي الذي سيتم إنشاؤه لمساحة العمل الخاصة بك</em>.</li>
<li><strong>Key vault</strong>: <em>لاحظ الحاوية الرئيسية الجديدة الافتراضية التي سيتم إنشاؤها لمساحة العمل الخاصة بك</em>.</li>
<li><strong>Application insights</strong>: <em>لاحظ مورد application insights الجديد الافتراضي الذي سيتم إنشاؤه لمساحة العمل الخاصة بك</em>.</li>
<li><strong>Container registry</strong>: None (<em>سيتم إنشاء سجل واحد تلقائيًا عند أول مرة تقوم فيها بتوزيع نموذج في حاوية</em>).</li>
</ul>
</li>
<li>
<p dir="rtl">حدد <strong>Review + create</strong>، ثم حدد <strong>Create</strong>. انتظر حتى يتم إنشاء مساحة العمل الخاصة بك (قد يستغرق الأمر بضع دقائق)، ثم انتقل إلى المورد الموزع.</p>
</li>
</ol>
<div dir="rtl"><div dir="rtl"><div class="markdown-heading" dir="auto"><h4 tabindex="-1" dir="rtl" class="heading-element">تشغيل الاستوديو</h4><a id="user-content-تشغيل-الاستوديو" class="anchor" aria-label="Permalink: تشغيل الاستوديو" href="#تشغيل-الاستوديو"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div><a id="user-content-تشغيل-الاستوديو" aria-label="Permalink: تشغيل الاستوديو" href="#تشغيل-الاستوديو"></a></div><a id="user-content-تشغيل-الاستوديو" aria-label="Permalink: تشغيل الاستوديو" href="#تشغيل-الاستوديو"></a></div>
<ol dir="rtl">
<li>
<p dir="rtl">في مورد مساحة عمل تعلم الآلة في Azure، حدد <strong>تشغيل الاستوديو</strong> (أو افتح علامة تبويب جديدة للمتصفح وانتقل إلى <a href="https://ml.azure.com?azure-portal=true" rel="nofollow">https://ml.azure.com</a>، وسجّل الدخول إلى استوديو Azure Machine Learning باستخدام حساب Microsoft الخاص بك). أغلق أي رسائل يتم عرضها.</p>
</li>
<li>
<p dir="rtl">في Azure Machine Learning studio، يجب أن تشاهد مساحة العمل التي تم إنشاؤها حديثًا. إذا لم يكن الأمر كذلك، فحدد <strong>جميع مساحات العمل</strong> في القائمة اليسرى ثم حدد مساحة العمل التي أنشأتها للتو.</p>
</li>
</ol>
<div dir="rtl"><div dir="rtl"><div class="markdown-heading" dir="auto"><h2 tabindex="-1" dir="rtl" class="heading-element">استخدم التعلّم الآلي التلقائي لتدريب نماذج</h2><a id="user-content-استخدم-التعلّم-الآلي-التلقائي-لتدريب-نماذج" class="anchor" aria-label="Permalink: استخدم التعلّم الآلي التلقائي لتدريب نماذج" href="#استخدم-التعلّم-الآلي-التلقائي-لتدريب-نماذج"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div><a id="user-content-استخدم-التعلّم-الآلي-التلقائي-لتدريب-نماذج" aria-label="Permalink: استخدم التعلّم الآلي التلقائي لتدريب نماذج" href="#استخدم-التعلّم-الآلي-التلقائي-لتدريب-نماذج"></a></div><a id="user-content-استخدم-التعلّم-الآلي-التلقائي-لتدريب-نماذج" aria-label="Permalink: استخدم التعلّم الآلي التلقائي لتدريب نماذج" href="#استخدم-التعلّم-الآلي-التلقائي-لتدريب-نماذج"></a></div>
<p dir="rtl">يتيح لك التعلّم الآلي التلقائي تجربة خوارزميات ومعلمات متعددة لتدريب نماذج متعددة، وتحديد أفضل نموذج لبياناتك. في هذا التمرين، ستستخدم مجموعة بيانات من التفاصيل القديمة لتأجير الدراجات لتدريب نموذج يتنبأ بعدد مرات تأجير الدراجات التي ينبغي توقعها في يوم معين، بناءً على الميزات الموسمية والأرصاد الجوية.</p>
<blockquote>
<p dir="rtl"><strong>الاقتباس</strong>: <em>البيانات المستخدمة في هذا التمرين مُشتقة من <a href="https://www.capitalbikeshare.com/system-data" rel="nofollow">Capital Bikeshare</a> وتستخدم وفقًا لـ<a href="https://www.capitalbikeshare.com/data-license-agreement" rel="nofollow">اتفاقية ترخيص</a>البيانات المنشورة</em>.</p>
</blockquote>
<ol dir="rtl">
<li>
<p dir="rtl">في <a href="https://ml.azure.com?azure-portal=true" rel="nofollow">استوديو التعلم الآلي في Azure</a>، اعرض صفحة <strong>التعلّم الآلي التلقائي</strong> (ضمن <strong>التأليف</strong>).</p>
</li>
<li>
<p dir="rtl">إنشاء مهمة تعلّم آلي تلقائية جديدة باستخدام الإعدادات التالية، باستخدام <strong>التالي</strong> كما هو مطلوب للتقدم من خلال واجهة المستخدم:</p>
<p dir="rtl"><strong>الإعدادات الأساسية</strong>:</p>
<ul dir="rtl">
<li><strong>اسم الوظيفة</strong>: يجب أن يكون حقل اسم الوظيفة مملوءًا مسبقًا باسم فريد. احتفظ به كما هو.</li>
<li><strong>اسم التجربة الجديدة</strong>: <code>mslearn-bike-rental</code></li>
<li><strong>الوصف</strong>: تعلّم آلي تلقائي للتنبؤ باستئجار الدراجات</li>
<li><strong>العلامات</strong>: <em>بدون</em></li>
</ul>
<p dir="rtl"><strong>نوع المهمة والبيانات</strong>:</p>
<ul dir="rtl">
<li>
<p dir="rtl"><strong>تحديد نوع المهمة</strong>: تراجع</p>
</li>
<li>
<p dir="rtl"><strong>حدد مجموعة البيانات</strong>: إنشاء مجموعة بيانات جديدة بالإعدادات التالية:</p>
<ul dir="rtl">
<li><strong>Data type</strong>:
<ul dir="rtl">
<li><strong>الاسم:</strong> <code>bike-rentals</code></li>
<li><strong>الوصف</strong>: <code>Historic bike rental data</code></li>
<li><strong>Type</strong>: جدول (mltable)</li>
</ul>
</li>
<li><strong>مصدر البيانات</strong>:
<ul dir="rtl">
<li>حدد <strong>من ملفات محلية</strong></li>
</ul>
</li>
<li><strong>نوع تخزين الوجهة</strong>:
<ul dir="rtl">
<li><strong>نوع مخزن البيانات</strong>: Azure Blob Storage</li>
<li><strong>الاسم</strong>: workspaceblobstore</li>
</ul>
</li>
<li><strong>تحديد MLtable</strong>:
<ul dir="rtl">
<li><strong>قم بتحميل المجلد</strong>: <em>قم بتنزيل المجلد المتضمن الملفين اللذين تحتاج إلى تحميلهما وفك ضغطه</em> <code>https://aka.ms/bike-rentals</code></li>
</ul>
</li>
</ul>
<p dir="rtl">حدد <strong>إنشاء</strong>. بعد إنشاء مجموعة البيانات، حدد مجموعة بيانات <strong>تأجير الدراجات</strong> لمواصلة إرسال مهمة التعلُّم الآلي التلقائي.</p>
</li>
</ul>
<p dir="rtl"><strong>إعدادات المهمة</strong>:</p>
<ul dir="rtl">
<li><strong>نوع المهمة</strong>: تراجع</li>
<li><strong>مجموعة البيانات</strong>: bike-rentals</li>
<li><strong>العمود الهدف</strong>: التأجيرات (عدد صحيح)</li>
<li><strong>إعدادات التكوين الإضافية</strong>:
<ul dir="rtl">
<li><strong>القياس الرئيسي</strong>: NormalizedRootMeanSquaredError</li>
<li><strong>شرح أفضل نموذج</strong>: <em>غير محدد</em></li>
<li><strong>تمكين تكديس المجموعات</strong>: <em>تم إلغاء التحديد</em></li>
<li><strong>استخدام جميع النماذج المدعومة</strong>: غير محدد. <em>ستقيد الوظيفة لتجربة عدد قليل من الخوارزميات المحددة فقط.</em></li>
<li><strong>Allowed models</strong>: <em>حدد فقط <strong>RandomForest</strong> و<strong>LightGBM</strong> — عادة ما ترغب في تجربة أكبر عدد ممكن، ولكن كل نموذج مضاف يزيد من الوقت الذي يستغرقه تشغيل الوظيفة.</em></li>
</ul>
</li>
<li>**** الحدود: <em>توسيع هذا القسم</em>
<ul dir="rtl">
<li><strong>الحد الأقصى للمحاولات</strong>: <code>3</code></li>
<li><strong>الحد الأقصى للمحاولات المتوازية</strong>: <code>3</code></li>
<li><strong>الحد الأقصى للعُقد</strong>: <code>3</code></li>
<li><strong>حد درجة القياس</strong>: <code>0.085</code> (<em>بحيث تنتهي المهمة إذا وصل النموذج إلى درجة القياس التي تمت تسويتها لجذر متوسط الخطأ التربيعي التي تبلغ 0,085 أو أقل.</em>)</li>
<li><strong>مهلة التجربة</strong>: <code>15</code></li>
<li><strong>انتهاء مهلة التكرار</strong>: <code>15</code></li>
<li><strong>تمكين الإنهاء المبكر</strong>: <em>محدد</em></li>
</ul>
</li>
<li>**    التحقق من الصحة والاختبار**:
<ul dir="rtl">
<li><strong>نوع التحقق من الصحة</strong>: تقسيم التحقق من صحة التدريب</li>
<li><strong>النسبة المئوية للبيانات</strong> التحقق من الصحة: 10</li>
<li><strong>مجموعة بيانات الاختبار</strong>: بدون</li>
</ul>
</li>
</ul>
<p dir="rtl"><strong>الحساب</strong>:</p>
<ul dir="rtl">
<li><strong>حدد نوع الحساب</strong>: بلا خادم</li>
<li><strong>Virtual machine type</strong>: معالج</li>
<li><strong>Virtual machine tier</strong>: Dedicated</li>
<li><strong>Virtual machine size</strong>: Standard_DS3_V2*</li>
<li><strong>عدد المثيلات</strong>: 1</li>
</ul>
<p dir="rtl">* <em>إذا كان اشتراكك يقيد أحجام الأجهزة الافتراضية المتوفِّرة لك، فاختر أي حجم متوفِّر.</em></p>
</li>
<li>
<p dir="rtl">تقديم وظيفة التدريب. تبدأ تلقائيًا.</p>
</li>
<li>
<p dir="rtl">انتظر حتى تنتهي المهمة. قد يستغرق بعض الوقت - الآن قد يكون الوقت المناسب لفترة استراحة لتناول القهوة!</p>
</li>
</ol>
<div dir="rtl"><div dir="rtl"><div class="markdown-heading" dir="auto"><h2 tabindex="-1" dir="rtl" class="heading-element">مراجعة أفضل نموذج</h2><a id="user-content-مراجعة-أفضل-نموذج" class="anchor" aria-label="Permalink: مراجعة أفضل نموذج" href="#مراجعة-أفضل-نموذج"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div><a id="user-content-مراجعة-أفضل-نموذج" aria-label="Permalink: مراجعة أفضل نموذج" href="#مراجعة-أفضل-نموذج"></a></div><a id="user-content-مراجعة-أفضل-نموذج" aria-label="Permalink: مراجعة أفضل نموذج" href="#مراجعة-أفضل-نموذج"></a></div>
<p dir="rtl">عند اكتمال مهمة التعلّم الآلي التلقائي، يمكنك مراجعة أفضل نموذج تم تدريبه.</p>
<ol dir="rtl">
<li>
<p dir="rtl">في علامة التبويب <strong>Overview</strong> شغّل التعلم الآلي التلقائي، لاحظ أفضل ملخص نموذج.
<a href="https://github.com/MicrosoftLearning/mslearn-ai-fundamentals.ar-sa/blob/main/Instructions/Labs/media/use-automated-machine-learning/complete-run.png"><img src="https://github.com/MicrosoftLearning/mslearn-ai-fundamentals.ar-sa/raw/main/Instructions/Labs/media/use-automated-machine-learning/complete-run.png" alt="لقطة شاشة لأفضل ملخص نموذج لوظيفة التعلم الآلي التلقائية مع مربع حول algorithm name." style="max-width: 100%;"></a></p>
</li>
<li>
<p dir="rtl">حدد النص الموجود أسفل <strong>اسم الخوارزمية</strong> لأفضل نموذج لعرض تفاصيله.</p>
</li>
<li>
<p dir="rtl">حدد علامة التبويب ⁧<strong>المقاييس⁧</strong>⁩ وحدد ⁧<strong>⁩القيم المتبقية⁧</strong>⁩ ومخططات ⁧<strong>⁩predicted_true⁧</strong>⁩ إذا لم تكن محددة بالفعل.</p>
<p dir="rtl">راجع المخططات البيانية التي توضح أداء النموذج. يظهر مخطط<strong>القيم المتبقية</strong> <em>القيم المتبقية</em> (الاختلافات بين القيم المتوقعة والقيم الفعلية) كمدرج تكراري. يقارن مخطط <strong>predicted_true</strong> القيم المتوقعة بالقيم الحقيقية.</p>
</li>
</ol>
<div dir="rtl"><div dir="rtl"><div class="markdown-heading" dir="auto"><h2 tabindex="-1" dir="rtl" class="heading-element">نشر النموذج واختباره</h2><a id="user-content-نشر-النموذج-واختباره" class="anchor" aria-label="Permalink: نشر النموذج واختباره" href="#نشر-النموذج-واختباره"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div><a id="user-content-نشر-النموذج-واختباره" aria-label="Permalink: نشر النموذج واختباره" href="#نشر-النموذج-واختباره"></a></div><a id="user-content-نشر-النموذج-واختباره" aria-label="Permalink: نشر النموذج واختباره" href="#نشر-النموذج-واختباره"></a></div>
<ol dir="rtl">
<li>
<p dir="rtl">على علامة تبويب <strong>النموذج</strong> لأفضل نموذج مدرب من قبل مهمة التعلم الآلي التلقائية خاصتك، حدد <strong>توزيع</strong> واستخدم خيار <strong>نقطة النهاية في الوقت الحقيقي</strong> لتوزيع النموذج مع الإعدادات التالية:</p>
<ul dir="rtl">
<li><strong>جهاز ظاهري</strong>: Standard_DS3_v2</li>
<li><strong>عدد المثيلات</strong>: 3</li>
<li><strong>نقطة النهاية</strong>: جديد</li>
<li><strong>اسم نقطة النهاية</strong>: <em>احتفظ بالاسم الافتراضي أو تأكد من أنه فريد بشكل عمومي</em></li>
<li><strong>اسم التوزيع</strong>: <em>اترك الإعداد الافتراضي</em></li>
<li><strong>استنتاج تجميع البيانات</strong>: <em>معطّل</em></li>
<li><strong>نموذج الحزمة</strong>: <em>معطّل</em></li>
</ul>
<blockquote>
<p dir="rtl"><strong>ملاحظة</strong> إذا تلقيت رسالة تفيد بعدم وجود حصة كافية لتحديد الجهاز الظاهري <em>Standard_DS3_v2</em>، فيرجى تحديد جهاز آخر.</p>
</blockquote>
</li>
<li>
<p dir="rtl">انتظر حتى بدء التوزيع - قد يستغرق هذا بضع ثوانٍ. سيتم الإشارة إلى <strong>حالة النشر</strong> لنقطة نهاية<strong>predict-rentals</strong> في الجزء الرئيسي من الصفحة <em>قيد التشغيل</em>.</p>
</li>
<li>
<p dir="rtl">انتظر حتى تتغير <strong>حالة النشر</strong> إلى <em>نجح</em>. قد يستغرق هذا ما يصل إلى 5-10 دقائق.</p>
</li>
</ol>
<div dir="rtl"><div dir="rtl"><div class="markdown-heading" dir="auto"><h2 tabindex="-1" dir="rtl" class="heading-element">اختبار الخدمة المنشورة</h2><a id="user-content-اختبار-الخدمة-المنشورة" class="anchor" aria-label="Permalink: اختبار الخدمة المنشورة" href="#اختبار-الخدمة-المنشورة"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div><a id="user-content-اختبار-الخدمة-المنشورة" aria-label="Permalink: اختبار الخدمة المنشورة" href="#اختبار-الخدمة-المنشورة"></a></div><a id="user-content-اختبار-الخدمة-المنشورة" aria-label="Permalink: اختبار الخدمة المنشورة" href="#اختبار-الخدمة-المنشورة"></a></div>
<p dir="rtl">يمكنك الآن اختبار الخدمة التي تم توزيعها.</p>
<ol dir="rtl">
<li>
<p dir="rtl">في استوديو Azure Machine Learning، في القائمة اليسرى، حدد <strong>نقاط النهاية</strong> وافتح نقطة النهاية في الوقت الفعلي <strong>predict-rentals</strong></p>
</li>
<li>
<p dir="rtl">في عرض صفحة نقطة نهاية <strong>predict-rentals</strong>، اعرض علامة تبويب <strong>الاختبار</strong>.</p>
</li>
<li>
<p dir="rtl">في جزء <strong>بيانات الإدخال لاختبار نقطة النهاية</strong>، استبدل قالب JSON ببيانات الإدخال التالية:</p>
</li>
<div dir="auto"><pre>  {
 <span>"input_data"</span>: {
   <span>"columns"</span>: [
     <span><span>"</span>day<span>"</span></span>,
     <span><span>"</span>mnth<span>"</span></span>,
     <span><span>"</span>year<span>"</span></span>,
     <span><span>"</span>season<span>"</span></span>,
     <span><span>"</span>holiday<span>"</span></span>,
     <span><span>"</span>weekday<span>"</span></span>,
     <span><span>"</span>workingday<span>"</span></span>,
     <span><span>"</span>weathersit<span>"</span></span>,
     <span><span>"</span>temp<span>"</span></span>,
     <span><span>"</span>atemp<span>"</span></span>,
     <span><span>"</span>hum<span>"</span></span>,
     <span><span>"</span>windspeed<span>"</span></span>
   ],
   <span>"index"</span>: [<span>0</span>],
   <span>"data"</span>: [[<span>1</span>,<span>1</span>,<span>2022</span>,<span>2</span>,<span>0</span>,<span>1</span>,<span>1</span>,<span>2</span>,<span>0.3</span>,<span>0.3</span>,<span>0.3</span>,<span>0.3</span>]]
 }
}
</pre><div dir="rtl">
  </div></div>
<li>
<p dir="rtl">انقر فوق الزر <strong>الاختبار</strong>.</p>
</li>
<li>
<p dir="rtl">راجع نتائج الاختبار، التي تتضمن عددًا متوقعًا من مرات الإيجار استنادً إلى ميزات الإدخال - مثل:</p>
</li>
<div dir="auto"><pre>[
  <span>352.3564674945718</span>
]</pre><div dir="rtl">
  </div></div>
<p dir="rtl">أخذ جزء الاختبار بيانات الإدخال واستخدم النموذج الذي دربته لإرجاع العدد المتوقع من الإيجارات.</p>
</ol>
<p dir="rtl">دعونا نستعرض ما فعلته. لقد استخدمت مجموعة بيانات من بيانات تأجير الدراجات التاريخية لتدريب نموذج. يتوقع النموذج عدد مرات تأجير الدراجات المتوقع في يوم معين، استناداً إلى <em>الميزات</em>الموسمية والأرصاد الجوية.</p>
<div dir="rtl"><div dir="rtl"><div class="markdown-heading" dir="auto"><h2 tabindex="-1" dir="rtl" class="heading-element">التنظيف</h2><a id="user-content-التنظيف" class="anchor" aria-label="Permalink: التنظيف" href="#التنظيف"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div><a id="user-content-التنظيف" aria-label="Permalink: التنظيف" href="#التنظيف"></a></div><a id="user-content-التنظيف" aria-label="Permalink: التنظيف" href="#التنظيف"></a></div>
<p dir="rtl">تتم استضافة خدمة الويب التي قمت بإنشائها في <em>Azure Container Instance</em>. إذا كنت لا تنوي إجراء المزيد من التجارب عليها، فإنه يجب عليك حذف نقطة النهاية لتجنب تراكم استخدام Azure غير الضروري.</p>
<ol dir="rtl">
<li>
<p dir="rtl">في <a href="https://ml.azure.com?azure-portal=true" rel="nofollow">آلة ستوديو Azure Machine Learning</a>، في علامة التبويب <strong>نقاط النهاية</strong>، حدد نقطة النهاية <strong>predict-rentals</strong>. ثم حدد <strong>Delete</strong>، وقم بالتأكيد على رغبتك في حذف نقطة النهاية.</p>
<p dir="rtl">يضمن حذف الحساب عدم تحصيل رسوم من اشتراكك مقابل موارد الحساب. ومع ذلك، سيتم تحصيل مبلغ صغير لتخزين البيانات طالما أن مساحة عمل التعلم الآلي من Azure موجودة في اشتراكك. إذا انتهيت من استكشاف التعلم الآلي من Azure، فإنه يمكنك حذف مساحة عمل التعلم الآلي من Azure والموارد المقترنة بها.</p>
</li>
</ol>
<p dir="rtl">لحذف مساحة العمل لديك:</p>
<ol dir="rtl">
<li>في <a href="https://portal.azure.com?azure-portal=true" rel="nofollow">مدخل Azure</a>، ومن صفحة <strong>Resource groups</strong>، افتح مجموعة الموارد التي حددتها عند إنشاء مساحة عمل Azure Machine Learning.</li>
<li>انقر فوق <strong>حذف مجموعة الموارد</strong>، واكتب اسم مجموعة الموارد لتأكيد أنك ترغب في حذفها، ثم حدد <strong>Delete</strong>.</li>
</ol>
</div>
</div>
</article></div>
