<div class="Box-sc-g0xbh4-0 eoaCFS js-snippet-clipboard-copy-unpositioned undefined" data-hpc="true"><article class="markdown-body entry-content container-lg" itemprop="text"><markdown-accessiblity-table data-catalyst=""><table>
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
  <td><div dir="rtl">استكشاف فهرس بحث الذكاء الاصطناعي في Azure (UI)</div></td>
  </tr>
  </tbody>
</table>
</div></td>
  </tr>
  </tbody>
</table></markdown-accessiblity-table>

<div class="markdown-heading" dir="rtl"><h1 tabindex="-1" class="heading-element" dir="rtl">استكشاف فهرس بحث الذكاء الاصطناعي في Azure (UI)</h1><a id="user-content-استكشاف-فهرس-بحث-الذكاء-الاصطناعي-في-azure-ui" class="anchor" aria-label="Permalink: استكشاف فهرس بحث الذكاء الاصطناعي في Azure (UI)" href="#استكشاف-فهرس-بحث-الذكاء-الاصطناعي-في-azure-ui"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="rtl">لنتخيل أنك تعمل في Fourth Coffee، وهي سلسلة مقاهي وطنية. يُطلب منك المساعدة في بناء حل للتنقيب عن المعرفة يجعل من السهل البحث عن رؤى حول تجارب العملاء. قررت إنشاء فهرس بحث الذكاء الاصطناعي في Azure باستخدام البيانات المستخرجة من مراجعات العملاء.</p>
<p dir="rtl">سوف تتعلم من خلال هذا التمرين المعملي ما يلي:</p>
<ul dir="rtl">
<li>إنشاء موارد Azure</li>
<li>استخراج البيانات من مصدر بيانات</li>
<li>إثراء البيانات بمهارات الذكاء الاصطناعي</li>
<li>استخدام مفهرس Azure في مدخل Azure</li>
<li>الاستعلام عن فهرس البحث</li>
<li>مراجعة النتائج المحفوظة في Knowledge Store</li>
</ul>
<div class="markdown-heading" dir="rtl"><h2 tabindex="-1" class="heading-element" dir="rtl">موارد Azure المطلوبة</h2><a id="user-content-موارد-azure-المطلوبة" class="anchor" aria-label="Permalink: موارد Azure المطلوبة" href="#موارد-azure-المطلوبة"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="rtl">يتطلب الحل الذي ستنشئه لـ Fourth Coffee الموارد التالية في اشتراك Azure الخاص بك:</p>
<ul dir="rtl">
<li>
<p dir="rtl">مورد <strong>بحث الذكاء الاصطناعي في Azure</strong> الذي سيدير ​​الفهرسة والاستعلام.</p>
</li>
<li>
<p dir="rtl">مورد <strong>خدمات الذكاء الاصطناعي في Azure</strong>، والذي يوفر خدمات الذكاء الاصطناعي للمهارات التي يمكن أن يستخدمها حل البحث الخاص بك لإثراء البيانات في مصدر البيانات بالرؤى الناتجة عن الذكاء الاصطناعي.</p>
<blockquote>
<p dir="rtl"><strong>ملاحظة</strong> يجب أن تكون موارد خدمات بحث الذكاء الاصطناعي في Azure والذكاء الاصطناعي في Azure في الموقع نفسه!</p>
</blockquote>
</li>
<li>
<p dir="rtl"><strong>حساب تخزين</strong> مع حاويات الكائنات الثنائية كبيرة الحجم والذي سيخزن المستندات الخام ومجموعات أخرى من الجداول أو الكائنات أو الملفات.</p>
</li>
</ul>
<div class="markdown-heading" dir="rtl"><h3 tabindex="-1" class="heading-element" dir="rtl">إنشاء مورد <em>كلام الذكاء الاصطناعي في Azure</em></h3><a id="user-content-إنشاء-مورد-كلام-الذكاء-الاصطناعي-في-azure" class="anchor" aria-label="Permalink: إنشاء مورد كلام الذكاء الاصطناعي في Azure" href="#إنشاء-مورد-كلام-الذكاء-الاصطناعي-في-azure"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<ol dir="rtl">
<li>
<p dir="rtl">قم بتسجيل الدخول إلى <a href="https://portal.azure.com/learn.docs.microsoft.com?azure-portal=true" rel="nofollow">مدخل Azure</a>.</p>
</li>
<li>
<p dir="rtl">انقر فوق زر <strong>＋إنشاء مورد</strong> وابحث عن <em>بحث الذكاء الاصطناعي في Azure</em>، وأنشئ مورد <strong>بحث الذكاء الاصطناعي في Azure</strong> باستخدام الإعدادات التالية:</p>
<ul dir="rtl">
<li><strong>الاشتراك</strong>: <em>اشتراك Azure الخاص بك</em>.</li>
<li><strong>مجموعة الموارد</strong>: <em>أنشئ مجموعة موارد جديدة ذات اسم فريد</em>.</li>
<li><strong>Service name</strong>: <em>اسم فريد</em>.</li>
<li><strong>الموقع</strong>: <em>اختر أي منطقة متوفِّرة. إذا كنت في شرق الولايات المتحدة، فاستخدم "شرق الولايات المتحدة 2"</em>.</li>
<li><strong>مستوى التسعير</strong>: أساسي</li>
</ul>
</li>
<li>
<p dir="rtl">حدد <strong>معاينة + إنشاء</strong>، وبعد أن تظهر لك استجابة <strong>نجاح التحقق</strong>، حدد <strong>إنشاء</strong>.</p>
</li>
<li>
<p dir="rtl">بعد اكتمال التوزيع، حدد «<strong>Go to resource</strong>». في صفحة النظرة العامة على بحث الذكاء الاصطناعي في Azure، يمكنك إضافة فهارس واستيراد البيانات والبحث في الفهارس التي جرى إنشاؤها.</p>
</li>
</ol>
<div class="markdown-heading" dir="rtl"><h3 tabindex="-1" class="heading-element" dir="rtl">إنشاء مورد خدمات الذكاء الاصطناعي في Azure</h3><a id="user-content-إنشاء-مورد-خدمات-الذكاء-الاصطناعي-في-azure" class="anchor" aria-label="Permalink: إنشاء مورد خدمات الذكاء الاصطناعي في Azure" href="#إنشاء-مورد-خدمات-الذكاء-الاصطناعي-في-azure"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="rtl">ستحتاج إلى توفير مورد خدمات <strong>الذكاء الاصطناعي في Azure</strong> الموجود في موقع مورد بحث الذكاء الاصطناعي في Azure الخاص بك نفسه. سيستخدم حل البحث الخاص بك هذا المورد لإثراء البيانات الموجودة في مخزن البيانات بالرؤى التي تم إنشاؤها بواسطة الذكاء الاصطناعي.</p>
<ol dir="rtl">
<li>
<p dir="rtl">قم بالرجوع إلى الصفحة الرئيسية في مدخل Azure. انقر فوق زر <strong>＋أنشئ مورد</strong> وابحث عن <em>خدمات ذكاء اصطناعي في Azure</em>. حدد <strong>إنشاء</strong> <strong>خطة خدمات الذكاء الاصطناعي في Azure</strong>. سيتم نقلك إلى صفحة لإنشاء مورد خدمات ذكاء اصطناعي في Azure. قم بتكوينه بالإعدادات التالية:</p>
<ul dir="rtl">
<li><strong>الاشتراك</strong>: <em>اشتراك Azure الخاص بك</em>.</li>
<li><strong>مجموعة الموارد</strong>: <em>مجموعة الموارد نفسها مثل مورد بحث الذكاء الاصطناعي في Azure الخاص بك</em>.</li>
<li><strong>المنطقة</strong>: <em>الموقع نفسه كمورد بحث الذكاء الاصطناعي في Azure الخاص بك</em>.</li>
<li><strong>Name</strong>: <em>اسم فريد</em>.</li>
<li><strong>مستوى التسعير</strong>: قياسي S0</li>
<li><strong>By checking this box I acknowledge that I have read and understood all the terms below</strong>: محدد</li>
</ul>
</li>
<li>
<p dir="rtl">حدد "<strong>Review + create</strong>". بعد أن ترى الاستجابة <strong>Validation Passed</strong>، حدد <strong>Create</strong>.</p>
</li>
<li>
<p dir="rtl">انتظر حتى يكتمل النشر، ثم اعرض تفاصيل النشر.</p>
</li>
</ol>
<div class="markdown-heading" dir="rtl"><h3 tabindex="-1" class="heading-element" dir="rtl">إنشاء حساب تخزين</h3><a id="user-content-إنشاء-حساب-تخزين" class="anchor" aria-label="Permalink: إنشاء حساب تخزين" href="#إنشاء-حساب-تخزين"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<ol dir="rtl">
<li>
<p dir="rtl">ارجع إلى الصفحة الرئيسية Azure-Portal، ثم حدد الزر <strong>+ Create a resource</strong>.</p>
</li>
<li>
<p dir="rtl">ابحث عن <em>storage account</em>، وأنشئ مورد <strong>storage account</strong> باستخدام الإعدادات التالية:</p>
<ul dir="rtl">
<li><strong>الاشتراك</strong>: <em>اشتراك Azure الخاص بك</em>.</li>
<li><strong>مجموعة الموارد</strong>: <em>مجموعة الموارد نفسها مثل موارد خدمات بحث الذكاء الاصطناعي في Azure والذكاء الاصطناعي في Azure</em>.</li>
<li><strong>Storage account name</strong>: <em>اسم فريد</em>.</li>
<li><strong>Location</strong>: <em>اختر أي موقع متوفر</em>.</li>
<li><strong>الأداء:</strong> قياسي</li>
<li><strong>التكرار</strong>: التخزين المتكرر محليًا (LRS)</li>
</ul>
</li>
<li>
<p dir="rtl">انقر فوق <strong>Review</strong>، ثم انقر فوق <strong>Create</strong>. انتظر حتى يكتمل النشر، ثم انتقل إلى المورد المنشور.</p>
</li>
<li>
<p dir="rtl">في حساب تخزين Azure الذي أنشأته، في جزء القائمة الأيسر، حدد <strong>تكوين</strong> (ضمن <strong>الإعدادات</strong>).</p>
</li>
<li>
<p dir="rtl">قم بتغيير الإعداد الخاص بـ <em>السماح بالوصول المجهول للكائنات الثنائية الكبيرة الحجم</em> إلى <strong>ممكّن</strong> ثم حدد <strong>حفظ</strong>.</p>
</li>
</ol>
<div class="markdown-heading" dir="rtl"><h2 tabindex="-1" class="heading-element" dir="rtl">تحميل المستندات إلى Azure Storage</h2><a id="user-content-تحميل-المستندات-إلى-azure-storage" class="anchor" aria-label="Permalink: تحميل المستندات إلى Azure Storage" href="#تحميل-المستندات-إلى-azure-storage"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<ol dir="rtl">
<li>
<p dir="rtl">في جزء القائمة الأيمن، حدد <strong>Containers</strong>.</p>
</li>
<p dir="auto"><a target="_blank" rel="noopener noreferrer" href="https://github.com/MicrosoftLearning/mslearn-ai-fundamentals/blob/main/Instructions/Labs/media/create-cognitive-search-solution/storage-blob-1.png"><img src="https://github.com/MicrosoftLearning/mslearn-ai-fundamentals/blob/main/Instructions/Labs/media/create-cognitive-search-solution/storage-blob-1.png" alt="لقطة شاشة تعرض صفحة «Storage Blob Overview»." style="max-width: 100%;"></a></p>
</li>
<li>
<p dir="rtl">حدد <strong>+ Container</strong>. يفتح جزء على جانبك الأيمن.</p>
</li>
<li>
<p dir="rtl">أدخل الإعدادات التالية، وانقر فوق <strong>Create</strong>:</p>
<ul dir="rtl">
<li><strong>الاسم</strong>: مراجعات القهوة</li>
<li><strong>مستوى الوصول العام</strong>: حاوية (وصول مجهول للقراءة للحاويات والكائنات الثنائية كبيرة الحجم)</li>
<li><strong>Advanced</strong>: <em>دون تغييرات</em>.</li>
</ul>
</li>
<li>
<p dir="rtl">في علامة تبويب جديدة بالمستعرض، يمكنك تنزيل <a href="https://aka.ms/mslearn-coffee-reviews" rel="nofollow">مراجعات القهوة المضغوطة</a> من <code>https://aka.ms/mslearn-coffee-reviews</code>، واستخرج الملفات إلى مجلد <em>المراجعات</em>.</p>
</li>
<li>
<p dir="rtl">في مدخل Microsoft Azure، حدد حاوية <em>coffee-reviews</em>. في الحاوية حدد <strong>Upload</strong>.</p>
</li>
<p dir="auto"><a target="_blank" rel="noopener noreferrer" href="https://github.com/MicrosoftLearning/mslearn-ai-fundamentals/blob/main/Instructions/Labs/media/create-cognitive-search-solution/storage-blob-3.png"><img src="https://github.com/MicrosoftLearning/mslearn-ai-fundamentals/blob/main/Instructions/Labs/media/create-cognitive-search-solution/storage-blob-3.png" style="max-width: 100%;"></a></p>
</li>
<li>
<p dir="rtl">في جزء <strong>Upload blob</strong>، حدد <strong>Select a file</strong>.</p>
</li>
<li>
<p dir="rtl">في نافذة المستكشف، حدد <strong>all</strong> الملفات الموجودة في مجلد <em>reviews</em>، وحدد <strong>Open</strong>، ثم حدد <strong>Upload</strong>.</p>
</li>
<p dir="auto"><a target="_blank" rel="noopener noreferrer" href="https://github.com/MicrosoftLearning/mslearn-ai-fundamentals/blob/main/Instructions/Labs/media/create-cognitive-search-solution/6a-azure-container-upload-files.png"><img src="https://github.com/MicrosoftLearning/mslearn-ai-fundamentals/blob/main/Instructions/Labs/media/create-cognitive-search-solution/6a-azure-container-upload-files.png" alt="لقطة شاشة تعرض الملفات التي تم تحميلها إلى حاوية Azure." style="max-width: 100%;"></a></p>
</li>
<li>
<p dir="rtl">بعد اكتمال التحميل، يمكنك إغلاق جزء <strong>Upload blob</strong>. الآن مستنداتك في حاوية تخزين <em>coffee-reviews</em>.</p>
</li>
</ol>
<div class="markdown-heading" dir="rtl"><h2 tabindex="-1" class="heading-element" dir="rtl">فهرسة المستندات</h2><a id="user-content-فهرسة-المستندات" class="anchor" aria-label="Permalink: فهرسة المستندات" href="#فهرسة-المستندات"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="rtl">بعد تخزين المستندات، يمكنك استخدام بحث الذكاء الاصطناعي في Azure لاستخراج نتائج التحليلات من المستندات. يوفر Azure-Portal <em>Import data wizard</em>. باستخدام هذا المعالج، يمكنك تلقائيا إنشاء فهرس ومفهرس لمصادر البيانات المدعومة. ستستخدم المعالج لإنشاء فهرس، واستيراد مستندات البحث الخاصة بك من التخزين إلى فهرس بحث الذكاء الاصطناعي في Azure.</p>
<ol dir="rtl">
<li>
<p dir="rtl">في مدخل Microsoft Azure، استعرض وصولاً إلى مورد بحث الذكاء الاصطناعي في Azure. ثم، في صفحة <strong>Overview</strong> حدد <strong>Import data</strong>.</p>
</li>
<p dir="auto"><a target="_blank" rel="noopener noreferrer" href="https://github.com/MicrosoftLearning/mslearn-ai-fundamentals/blob/main/Instructions/Labs/media/create-cognitive-search-solution/azure-search-wizard-1.png"><img src="https://github.com/MicrosoftLearning/mslearn-ai-fundamentals/blob/main/Instructions/Labs/media/create-cognitive-search-solution/azure-search-wizard-1.png" alt="لقطة شاشة تعرض معالج استيراد البيانات." style="max-width: 100%;"></a></p>
</li>
<li>
<p dir="rtl">في صفحة <strong>الاتصال ببياناتك</strong>، في قائمة <strong>مصدر البيانات</strong>، حدد <strong>Azure Blob Storage</strong>. ثم أكمل تفاصيل مخزن البيانات بالقيم التالية:</p>
<ul dir="rtl">
<li><strong>Data Source</strong>: Azure Blob Storage</li>
<li><strong>اسم مصدر البيانات</strong>: coffee-customer-data</li>
<li><strong>البيانات المراد استخراجها</strong>: المحتوى وبيانات التعريف</li>
<li><strong>وضع التحليل</strong>: افتراضي</li>
<li><strong>سلسلة الاتصال</strong>: *حدد <strong>اختيار اتصال موجود</strong>. حدد حساب التخزين الخاص بك، وحدد حاوية <strong>coffee-reviews</strong>، ثم انقر فوق <strong>Select</strong>.</li>
<li><strong>مصادقة الهوية المُدارة</strong>: لا شيء</li>
<li><strong>Container name</strong>: <em>تتم تعبئة هذا الإعداد تلقائيًا بعد اختيار اتصال موجود</em>.</li>
<li><strong>Blob folder</strong>: <em>اترك هذا فارغًا</em>.</li>
<li><strong>الوصف</strong>: مراجعات لمقاهي Fourth Coffee.</li>
</ul>
</li>
<li>
<p dir="rtl">حدد <strong>Next: Add cognitive skills (Optional)</strong>.</p>
</li>
<li>
<p dir="rtl">في مقطع <strong>إرفاق خدمات الذكاء الاصطناعي</strong> حدد مورد خدمات الذكاء الاصطناعي في Azure لديك.</p>
</li>
<li>
<p dir="rtl">في القسم <strong>إضافة إثراءات</strong>:</p>
<ul dir="rtl">
<li>
<p dir="rtl">غيّر <strong>اسم مجموعة المهارات</strong> إلى <strong>مجموعة مهارات القهوة</strong>.</p>
</li>
<li>
<p dir="rtl">حدد خانة الاختيار <strong>تمكين OCR ودمج كل النص في حقل merged_content</strong>.</p>
<blockquote>
<p dir="rtl"><strong>ملاحظة</strong> من المهم تحديد <strong>Enable OCR</strong> لعرض جميع خيارات الحقول الغنية.</p>
</blockquote>
</li>
<li>
<p dir="rtl">تأكد من تعيين <strong>حقل بيانات المصدر</strong> إلى <strong>merged_content</strong>.</p>
</li>
<li>
<p dir="rtl">غيّر <strong>مستوى دقة الإثراء</strong> إلى <strong>صفحات (5000 مجموعة حرف)</strong>.</p>
</li>
<li>
<p dir="rtl">لا تحدد <em>Enable incremental enrichment</em></p>
</li>
<li>
<p dir="rtl">حدد الحقول الغنية التالية:</p>
<markdown-accessiblity-table data-catalyst=""><table>
<thead>
<tr>
<th>المهارة المعرفية</th>
<th>المعلمة‬</th>
<th>اسم الحقل</th>
</tr>
</thead>
<tbody>
<tr>
<td>استخراج أسماء المواقع</td>
<td></td>
<td>المواقع</td>
</tr>
<tr>
<td>استخراج العبارات الرئيسية</td>
<td></td>
<td>keyphrases</td>
</tr>
<tr>
<td>اكتشاف التوجه</td>
<td></td>
<td>التوجه</td>
</tr>
<tr>
<td>إنشاء علامات من الصور</td>
<td></td>
<td>imageTags</td>
</tr>
<tr>
<td>إنشاء تسميات توضيحية من الصور</td>
<td></td>
<td>imageCaption</td>
</tr>
</tbody>
</table></markdown-accessiblity-table>
</li>
</ul>
</li>
<li>
<p dir="rtl">ضمن <strong>Save Enrichments to a Knowledge Store</strong>، حدد:</p>
<ul dir="rtl">
<li>إسقاطات الصور</li>
<li>المستندات</li>
<li>الصفحات</li>
<li>Key phrases</li>
<li>الكيانات</li>
<li>تفاصيل الصور</li>
<li>مراجع الصور</li>
</ul>
<blockquote>
<p dir="rtl"><strong>ملاحظة</strong> يظهر تحذير يطلب <strong>سلسلة اتصال حساب Storage</strong>.</p>
</li>
<p dir="auto"><a target="_blank" rel="noopener noreferrer" href="https://github.com/MicrosoftLearning/mslearn-ai-fundamentals/blob/main/Instructions/Labs/media/create-cognitive-search-solution/6a-azure-cognitive-search-enrichments-warning.png"><img src="https://github.com/MicrosoftLearning/mslearn-ai-fundamentals/blob/main/Instructions/Labs/media/create-cognitive-search-solution/6a-azure-cognitive-search-enrichments-warning.png" alt="لقطة شاشة تعرض تحذير شاشة اتصال حساب Storage مع تحديد &quot;Choose an existing connection&quot;." style="max-width: 100%;"></a></p>
</blockquote>
</li>
<li>
<p dir="rtl">حدد رابط <strong>Choose an existing connection</strong>. اختر حساب التخزين الذي أنشأته سابقًا.</p>
<blockquote>
<ol dir="rtl">
<li>انقر فوق <strong>+ حاوية</strong> لإنشاء حاوية جديدة تسمى <strong>مخزن المعرفة</strong> مع مستوى خصوصية المُعين إلى <strong>خاص</strong>، وحدد <strong>إنشاء</strong>.</li>
<li>ثم حدد حاوية <strong>knowledge-store</strong> ثم انقر فوق <strong>Select</strong> أسفل الشاشة.</li>
</ol>
</blockquote>
</li>
<li>
<p dir="rtl">حدد <strong>مشاريع كائن ثنائي كبير الحجم في Azure: مستند</strong>. سيظهر إعداد <em>Container name</em> مع حاوية <em>knowledge-store</em> التي تمت تعبئتها تلقائياً. لا تقم بتغيير اسم الحاوية.</p>
</li>
<li>
<p dir="rtl">حدد <strong>Next: Customize target index</strong>. غيّر <strong>Index name</strong> إلى <strong>coffee-index</strong>.</p>
</li>
<li>
<p dir="rtl">تأكد من أن <strong>Key</strong> مضبوط على <strong>metadata_storage_path</strong>. اترك <strong>Suggester name</strong> فارغا و <strong>Search mode</strong> ممتلئا تلقائيا.</p>
</li>
<li>
<p dir="rtl">راجع الإعدادات الافتراضية لحقول الفهرس. حدد <strong>filterable</strong> لجميع الحقول التي تم تحديدها مسبقاً بشكل افتراضي. تتضمن أسماء الحقول التي يجب وضع علامة <em>قابل للتصفية</em> عليها: المحتوى والمواقع والعبارات الأساسية والتوجه وmerged_content والنصوص وlayoutText وimageTags وimageCaption.</p>
</li>
<p dir="auto"><a target="_blank" rel="noopener noreferrer" href="https://github.com/MicrosoftLearning/mslearn-ai-fundamentals/blob/main/Instructions/Labs/media/create-cognitive-search-solution/6a-azure-cognitive-search-customize-index.png"><img src="https://github.com/MicrosoftLearning/mslearn-ai-fundamentals/blob/main/Instructions/Labs/media/create-cognitive-search-solution/6a-azure-cognitive-search-customize-index.png " alt="لقطة شاشة تعرض جزء الفهرس المخصص مع إدخال اسم الفهرس واختيار &quot;Filterable&quot; لحقل فهرس افتراضي." style="max-width: 100%;"></a></p>
</li>
<li>
<p dir="rtl">حدد <strong>التالي: إنشاء مفهرس</strong>.</p>
</li>
<li>
<p dir="rtl">غيّر <strong>Indexer name</strong> إلى <strong>coffee-indexer</strong>.</p>
</li>
<li>
<p dir="rtl">اترك <strong>الجدول</strong> معيناً على <strong>مرة واحدة</strong>.</p>
</li>
<li>
<p dir="rtl">وسّع <strong>Advanced options</strong>. تأكد من تحديد الخيار <strong>Base-64 Encode Keys</strong>، حيث يمكن لمفاتيح الترميز أن تجعل الفهرس أكثر كفاءة.</p>
</li>
<li>
<p dir="rtl">حدد <strong>إرسال</strong> لإنشاء مصدر البيانات ومجموعة المهارات والفهرس والمفهرس. يتم تشغيل المفهرس تلقائياً ويقوم بتشغيل خط أنابيب الفهرسة، والذي:</p>
<ul dir="rtl">
<li>يستخرج محتويات وحقول بيانات تعريف الوثيقة من مصدر البيانات.</li>
<li>يدير مجموعة مهارات المهارات المعرفية لإنشاء حقول غنية أكثر.</li>
<li>يعين الحقول المستخرجة إلى الفهرس.</li>
</ul>
</li>
<li>
<p dir="rtl">ارجع إلى صفحة موارد بحث الذكاء الاصطناعي في Azure الخاصة بك. في الجزء الأيمن، ضمن <strong>إدارة</strong> البحث، حدد <strong>المفهرسات</strong>. حدد <strong>فهرس القهوة</strong> الذي جرى إنشاؤه حديثاً. انتظر دقيقة، ثم حدد <strong>↻ Refresh</strong> حتى تشير <strong>Status</strong> إلى النجاح.</p>
</li>
<li>
<p dir="rtl">حدد اسم المفهرس لمعرفة المزيد من التفاصيل.</p>
</li>
<p dir="auto"><a target="_blank" rel="noopener noreferrer" href="https://github.com/MicrosoftLearning/mslearn-ai-fundamentals/blob/main/Instructions/Labs/media/create-cognitive-search-solution/6a-search-indexer-success.png"><img src="https://github.com/MicrosoftLearning/mslearn-ai-fundamentals/blob/main/Instructions/Labs/media/create-cognitive-search-solution/6a-search-indexer-success.png" alt="لقطة شاشة تظهر إنشاء مفهرس القهوة بنجاح." style="max-width: 100%;"></a></p>
</li>
</ol>
<div class="markdown-heading" dir="rtl"><h2 tabindex="-1" class="heading-element" dir="rtl">الاستعلام عن الفهرس</h2><a id="user-content-الاستعلام-عن-الفهرس" class="anchor" aria-label="Permalink: الاستعلام عن الفهرس" href="#الاستعلام-عن-الفهرس"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="rtl">استخدم مستكشف البحث لكتابة الاستعلامات واختبارها. مستكشف البحث أداة مدرجة في مدخل Microsoft Azure تمنحك طريقة سهلة للتحقق من جودة فهرس البحث. يمكنك استخدام مستكشف البحث لكتابة استعلامات ومراجعة النتائج في JSON.</p>
<ol dir="rtl">
<li>
<p dir="rtl">في صفحة <em>نظرة عامة</em> لخدمة البحث، حدد <strong>مستكشف البحث</strong> أعلى الشاشة.</p>
</li>
<p dir="auto"><a target="_blank" rel="noopener noreferrer" href="https://github.com/MicrosoftLearning/mslearn-ai-fundamentals/blob/main/Instructions/Labs/media/create-cognitive-search-solution/5-exercise-screenshot-7.png"><img src="https://github.com/MicrosoftLearning/mslearn-ai-fundamentals/blob/main/Instructions/Labs/media/create-cognitive-search-solution/5-exercise-screenshot-7.png" alt="لقطة شاشة تبين كيفية العثور على مستكشف البحث." style="max-width: 100%;"></a></p>
</li>
<li>
<p dir="rtl">لاحظ كيف أن الفهرس المحدد هو <em>coffee-index</em> الذي أنشأته. أسفل الفهرس المحدد، يمكن تغيير <em>طريقة العرض</em> إلى <strong>طريقة عرض JSON</strong>.</p>
</li>
<p dir="auto"><a target="_blank" rel="noopener noreferrer" href="https://github.com/MicrosoftLearning/mslearn-ai-fundamentals/blob/main/Instructions/Labs/media/create-cognitive-search-solution/search-explorer-query.png"><img src="https://github.com/MicrosoftLearning/mslearn-ai-fundamentals/blob/main/Instructions/Labs/media/create-cognitive-search-solution/search-explorer-query.png" alt="لقطة شاشة لمتصفح البحث." style="max-width: 100%;"></a></p>
</li>
</ol>
<p dir="rtl">في حقل <strong>محرر استعلام JSON</strong>، انسخ والصق:</p>
<div class="highlight highlight-source-json notranslate position-relative overflow-auto" dir="rtl"><pre>{
    <span class="pl-ent">"search"</span>: <span class="pl-s"><span class="pl-pds">"</span>*<span class="pl-pds">"</span></span>,
    <span class="pl-ent">"count"</span>: <span class="pl-c1">true</span>
}</pre><div class="zeroclipboard-container">
    <clipboard-copy aria-label="Copy" class="ClipboardButton btn btn-invisible js-clipboard-copy m-2 p-0 d-flex flex-justify-center flex-items-center" data-copy-feedback="Copied!" data-tooltip-direction="w" value="{
    &quot;search&quot;: &quot;*&quot;,
    &quot;count&quot;: true
}" tabindex="0" role="button">
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-copy js-clipboard-copy-icon">
    <path d="M0 6.75C0 5.784.784 5 1.75 5h1.5a.75.75 0 0 1 0 1.5h-1.5a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-1.5a.75.75 0 0 1 1.5 0v1.5A1.75 1.75 0 0 1 9.25 16h-7.5A1.75 1.75 0 0 1 0 14.25Z"></path><path d="M5 1.75C5 .784 5.784 0 6.75 0h7.5C15.216 0 16 .784 16 1.75v7.5A1.75 1.75 0 0 1 14.25 11h-7.5A1.75 1.75 0 0 1 5 9.25Zm1.75-.25a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-7.5a.25.25 0 0 0-.25-.25Z"></path>
</svg>
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-check js-clipboard-check-icon color-fg-success d-none">
    <path d="M13.78 4.22a.75.75 0 0 1 0 1.06l-7.25 7.25a.75.75 0 0 1-1.06 0L2.22 9.28a.751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018L6 10.94l6.72-6.72a.75.75 0 0 1 1.06 0Z"></path>
</svg>
    </clipboard-copy>
  </div></div>
<ol start="3" dir="rtl">
<li>
<p dir="rtl">حدد <strong>بحث</strong>. يعرض استعلام البحث جميع المستندات الموجودة في فهرس البحث، بما في ذلك عدد جميع المستندات في الحقل <strong>@odata.count</strong>. يجب أن يُرجع فهرس البحث مستند JSON مدرجًا فيه نتائج البحث.</p>
</li>
<li>
<p dir="rtl">الآن دعونا نباشر بتصفية حسب الموقع. في حقل <strong>محرر استعلام JSON</strong>، انسخ والصق:</p>
</li>
</ol>
<div class="highlight highlight-source-json notranslate position-relative overflow-auto" dir="rtl"><pre>{
    <span class="pl-ent">"search"</span>: <span class="pl-s"><span class="pl-pds">"</span>locations:'Chicago'<span class="pl-pds">"</span></span>,
    <span class="pl-ent">"count"</span>: <span class="pl-c1">true</span>
}</pre><div class="zeroclipboard-container">
    <clipboard-copy aria-label="Copy" class="ClipboardButton btn btn-invisible js-clipboard-copy m-2 p-0 d-flex flex-justify-center flex-items-center" data-copy-feedback="Copied!" data-tooltip-direction="w" value="{
    &quot;search&quot;: &quot;locations:'Chicago'&quot;,
    &quot;count&quot;: true
}" tabindex="0" role="button">
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-copy js-clipboard-copy-icon">
    <path d="M0 6.75C0 5.784.784 5 1.75 5h1.5a.75.75 0 0 1 0 1.5h-1.5a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-1.5a.75.75 0 0 1 1.5 0v1.5A1.75 1.75 0 0 1 9.25 16h-7.5A1.75 1.75 0 0 1 0 14.25Z"></path><path d="M5 1.75C5 .784 5.784 0 6.75 0h7.5C15.216 0 16 .784 16 1.75v7.5A1.75 1.75 0 0 1 14.25 11h-7.5A1.75 1.75 0 0 1 5 9.25Zm1.75-.25a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-7.5a.25.25 0 0 0-.25-.25Z"></path>
</svg>
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-check js-clipboard-check-icon color-fg-success d-none">
    <path d="M13.78 4.22a.75.75 0 0 1 0 1.06l-7.25 7.25a.75.75 0 0 1-1.06 0L2.22 9.28a.751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018L6 10.94l6.72-6.72a.75.75 0 0 1 1.06 0Z"></path>
</svg>
    </clipboard-copy>
  </div></div>
<ol start="5" dir="rtl">
<li>
<p dir="rtl">حدد <strong>بحث</strong>. يبحث الاستعلام في جميع المستندات الموجودة في الفهرس وعوامل التصفية لمراجعات ذات موقع في شيكاغو. يجب أن تشاهد <code>3</code> في الحقل <code>@odata.count</code>.</p>
</li>
<li>
<p dir="rtl">الآن دعونا نصفي حسب التوجه. في حقل <strong>محرر استعلام JSON</strong>، انسخ والصق:</p>
</li>
</ol>
<div class="highlight highlight-source-json notranslate position-relative overflow-auto" dir="rtl"><pre>{
    <span class="pl-ent">"search"</span>: <span class="pl-s"><span class="pl-pds">"</span>sentiment:'negative'<span class="pl-pds">"</span></span>,
    <span class="pl-ent">"count"</span>: <span class="pl-c1">true</span>
}</pre><div class="zeroclipboard-container">
    <clipboard-copy aria-label="Copy" class="ClipboardButton btn btn-invisible js-clipboard-copy m-2 p-0 d-flex flex-justify-center flex-items-center" data-copy-feedback="Copied!" data-tooltip-direction="w" value="{
    &quot;search&quot;: &quot;sentiment:'negative'&quot;,
    &quot;count&quot;: true
}" tabindex="0" role="button">
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-copy js-clipboard-copy-icon">
    <path d="M0 6.75C0 5.784.784 5 1.75 5h1.5a.75.75 0 0 1 0 1.5h-1.5a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-1.5a.75.75 0 0 1 1.5 0v1.5A1.75 1.75 0 0 1 9.25 16h-7.5A1.75 1.75 0 0 1 0 14.25Z"></path><path d="M5 1.75C5 .784 5.784 0 6.75 0h7.5C15.216 0 16 .784 16 1.75v7.5A1.75 1.75 0 0 1 14.25 11h-7.5A1.75 1.75 0 0 1 5 9.25Zm1.75-.25a.25.25 0 0 0-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 0 0 .25-.25v-7.5a.25.25 0 0 0-.25-.25Z"></path>
</svg>
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-check js-clipboard-check-icon color-fg-success d-none">
    <path d="M13.78 4.22a.75.75 0 0 1 0 1.06l-7.25 7.25a.75.75 0 0 1-1.06 0L2.22 9.28a.751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018L6 10.94l6.72-6.72a.75.75 0 0 1 1.06 0Z"></path>
</svg>
    </clipboard-copy>
  </div></div>
<ol start="7" dir="rtl">
<li>
<p dir="rtl">حدد <strong>بحث</strong>. يبحث الاستعلام في جميع المستندات الموجودة في الفهرس وعوامل التصفية لمراجعات ذات توجه سلبي. يجب أن تشاهد <code>1</code> في الحقل <code>@odata.count</code>.</p>
<blockquote>
<p dir="rtl"><strong>ملاحظة</strong> راجع كيفية فرز النتائج بواسطة <code>@search.score</code>. هذه هي النتيجة التي حددها محرك البحث لإظهار مدى تطابق النتائج مع الاستعلام المحدد.</p>
</blockquote>
</li>
<li>
<p dir="rtl">إحدى المشكلات التي قد نرغب في حلها هي سبب وجود مراجعات معينة. دعنا نلقِ نظرة على العبارات الرئيسية المرتبطة بالمراجعة السلبية. ما هو برأيك سبب المراجعة؟</p>
</li>
</ol>
<div class="markdown-heading" dir="rtl"><h2 tabindex="-1" class="heading-element" dir="rtl">مراجعة مخزن المعرفة</h2><a id="user-content-مراجعة-مخزن-المعرفة" class="anchor" aria-label="Permalink: مراجعة مخزن المعرفة" href="#مراجعة-مخزن-المعرفة"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="rtl">دعنا نرَ قوة مخزن المعرفة أثناء العمل. عند تشغيل <em>Import data wizard</em>، يمكنك أيضاً إنشاء مخزن معرفة. ستجد داخل مخزن المعرفة أن البيانات المخصّصة المستخرجة من مهارات الذكاء الاصطناعي تستمر في شكل إسقاطات وجداول.</p>
<ol dir="rtl">
<li>
<p dir="rtl">في مدخل Azure، انتقل مرةً أخرى إلى حساب Azure Storage خاصتك.</p>
</li>
<li>
<p dir="rtl">في جزء القائمة الأيمن، حدد <strong>Containers</strong>. حدد حاوية <strong>knowledge-store</strong>.</p>
</li>
<p dir="auto"><a target="_blank" rel="noopener noreferrer" href="https://github.com/MicrosoftLearning/mslearn-ai-fundamentals/blob/main/Instructions/Labs/media/create-cognitive-search-solution/knowledge-store-blob-0.png"><img src="https://github.com/MicrosoftLearning/mslearn-ai-fundamentals/blob/main/Instructions/Labs/media/create-cognitive-search-solution/knowledge-store-blob-0.png" alt="لقطة شاشة لحاوية مخزن المعرفة." style="max-width: 100%;"></a></p>
</li>
<li>
<p dir="rtl">سترى قائمة مجلدات. يوجد مجلد واحد لكل بيانات تعريف لكل مستند مراجعة. <strong>حدد أياً من المجلدات</strong>. داخل المجلد، انقر فوق ملف <strong>objectprojection.json</strong>.</p>
</li>
<p dir="auto"><a target="_blank" rel="noopener noreferrer" href="https://github.com/MicrosoftLearning/mslearn-ai-fundamentals/blob/main/Instructions/Labs/media/create-cognitive-search-solution/knowledge-store-blob-1.png"><img src="https://github.com/MicrosoftLearning/mslearn-ai-fundamentals/blob/main/Instructions/Labs/media/create-cognitive-search-solution/knowledge-store-blob-1.png" alt="لقطة شاشة من objectproject.json." style="max-width: 100%;"></a></p>
</li>
<li>
<p dir="rtl">انقر فوق <strong>Edit</strong> لرؤية JSON الذي تم إنتاجه لأحد المستندات من مخزن بيانات Azure.</p>
</li>
<p dir="auto"><a target="_blank" rel="noopener noreferrer" href="https://github.com/MicrosoftLearning/mslearn-ai-fundamentals/blob/main/Instructions/Labs/media/create-cognitive-search-solution/knowledge-store-blob-2.png"><img src="https://github.com/MicrosoftLearning/mslearn-ai-fundamentals/blob/main/Instructions/Labs/media/create-cognitive-search-solution/knowledge-store-blob-2.png" alt="لقطة شاشة لكيفية العثور على زر التحرير." style="max-width: 100%;"></a></p>
</li>
<li>
<p dir="rtl">حدد عنوان storage blob في أعلى يسار الشاشة للعودة إلى <em>Containers</em> لـ Storage account.</p>
</li>
<p dir="auto"><a target="_blank" rel="noopener noreferrer" href="https://github.com/MicrosoftLearning/mslearn-ai-fundamentals/blob/main/Instructions/Labs/media/create-cognitive-search-solution/knowledge-store-blob-4.png"><img src="https://github.com/MicrosoftLearning/mslearn-ai-fundamentals/blob/main/Instructions/Labs/media/create-cognitive-search-solution/knowledge-store-blob-4.png" alt="لقطة شاشة لمسار تنقل بيانات تخزين البيانات الثنائية الكبيرة." style="max-width: 100%;"></a></p>
</li>
<li>
<p dir="rtl">في <em>Containers</em>، حدد الحاوية <em>coffee-skillset-image-projection</em>. حدد أي من العناصر.</p>
</li>
<p dir="auto"><a target="_blank" rel="noopener noreferrer" href="https://github.com/MicrosoftLearning/mslearn-ai-fundamentals/blob/main/Instructions/Labs/media/create-cognitive-search-solution/knowledge-store-blob-5.png"><img src="https://github.com/MicrosoftLearning/mslearn-ai-fundamentals/blob/main/Instructions/Labs/media/create-cognitive-search-solution/knowledge-store-blob-5.png" alt="لقطة شاشة لحاوية مجموعة المهارات." style="max-width: 100%;"></a></p>
</li>
<li>
<p dir="rtl">حدد أي من ملفات <em>.jpg</em>. انقر فوق <strong>Edit</strong> لمشاهدة الصورة المخزنة من المستند. لاحظ كيف يتم تخزين جميع الصور من المستندات بهذه الطريقة.</p>
</li>
<p dir="auto"><a target="_blank" rel="noopener noreferrer" href="https://github.com/MicrosoftLearning/mslearn-ai-fundamentals/blob/main/Instructions/Labs/media/create-cognitive-search-solution/knowledge-store-blob-3.png"><img src="https://github.com/MicrosoftLearning/mslearn-ai-fundamentals/blob/main/Instructions/Labs/media/create-cognitive-search-solution/knowledge-store-blob-3.png" alt="لقطة شاشة للصورة المحفوظة." style="max-width: 100%;"></a></p>
</li>
<li>
<p dir="rtl">حدد عنوان storage blob في أعلى يسار الشاشة للعودة إلى <em>Containers</em> لـ Storage account.</p>
</li>
<li>
<p dir="rtl">حدد <strong>Storage browser</strong> على اللوحة اليسرى، وحدد <strong>Tables</strong>. يوجد جدول لكل كيان في الفهرس. حدد الجدول <em>coffeeSkillsetKeyPhrases</em>.</p>
<p dir="rtl">ألق نظرة على العبارات الرئيسية التي تمكن مخزن المعرفة من التقاطها من المحتوى في المراجعات. العديد من الحقول هي مفاتيح، حتى تتمكن من ربط الجداول مثل قاعدة بيانات ارتباطية. الحقل الأخير يظهر العبارات الرئيسية التي اُستخرِجت بواسطة مجموعة المهارات.</p>
</li>
</ol>
<div class="markdown-heading" dir="rtl"><h2 tabindex="-1" class="heading-element" dir="rtl">معرفة المزيد</h2><a id="user-content-معرفة-المزيد" class="anchor" aria-label="Permalink: معرفة المزيد" href="#معرفة-المزيد"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="rtl">يفهرس هذا البحث البسيط بعض إمكانيات خدمة بحث الذكاء الاصطناعي في Azure فقط. لمعرفة المزيد حول ما يمكنك فعله بهذه الخدمة، راجع <a href="https://learn.microsoft.com/azure/search" rel="nofollow">صفحة خدمة بحث الذكاء الاصطناعي في Azure</a>.</p>
</article></div>
