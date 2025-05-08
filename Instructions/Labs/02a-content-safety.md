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
  <td><div dir="rtl">استكشاف أمان المحتوى في Azure AI Foundry</div></td>
  </tr>
  </tbody>
</table>
</div></td>
  </tr>
  </tbody>
</table></markdown-accessiblity-table>

<div class="markdown-heading" dir="rtl"><h1 tabindex="-1" class="heading-element" dir="rtl">استكشاف أمان المحتوى في Azure AI Foundry</h1><a id="user-content-استكشاف-أمان-المحتوى-في-azure-ai-foundry" class="anchor" aria-label="Permalink: استكشاف أمان المحتوى في Azure AI Foundry" href="#استكشاف-أمان-المحتوى-في-azure-ai-foundry"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="rtl">تساعد خدمات الذكاء الاصطناعي في Azure المستخدمين على إنشاء تطبيقات الذكاء الاصطناعي باستخدام واجهات برمجة التطبيقات المبتكرة والنماذج الجاهزة والمبنية مسبقًا والقابلة للتخصيص. في هذا التمرين، ستلقي نظرة على إحدى الخدمات، أمان المحتوى باستخدام الذكاء الاصطناعي في Azure، التي تمكنك من تعديل محتوى النصوص والصور. في بوابة Azure AI Foundry، وهي منصة Microsoft لإنشاء التطبيقات الذكية، ستستخدم أمان المحتوى باستعمال الذكاء الاصطناعي في Azure لتصنيف النص وتعيين درجة خطورته.</p>
<blockquote>
<p dir="rtl"><strong>ملاحظه</strong> الهدف من هذا التمرين هو تكوين فكرة عامة عن كيفية توفير خدمات Azure للذكاء الاصطناعي واستخدامها. يتم استخدام المحتوى السلامة كمثال، ولكن لا يتوقع منك اكتساب معرفة شاملة بسلامة المحتوى في هذا التمرين!</p>
</blockquote>
<div class="markdown-heading" dir="rtl"><h2 tabindex="-1" class="heading-element" dir="rtl">إنشاء مشروع في مدخل Azure AI Foundry</h2><a id="user-content-إنشاء-مشروع-في-مدخل-azure-ai-foundry" class="anchor" aria-label="Permalink: إنشاء مشروع في مدخل Azure AI Foundry" href="#إنشاء-مشروع-في-مدخل-azure-ai-foundry"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<ol dir="rtl">
<li>
<p dir="rtl">في علامة تبويب المتصفح، انتقل إلى <a href="https://ai.azure.com?azure-portal=true" rel="nofollow">مدخل Azure AI Foundry</a>.</p>
</li>
<li>
<p dir="rtl">سجل الدخول باستخدام حسابك.</p>
</li>
<li>
<p dir="rtl">في الصفحة الرئيسية لمدخل Azure AI Foundry، حدد <strong>إنشاء مشروع</strong>. في Azure AI Foundry، تعتبر المشاريع عبارة عن حاويات تساعد في تنظيم عملك.</p>
<p dir="auto"><a target="_blank" rel="noopener noreferrer" href="https://github.com/MicrosoftLearning/mslearn-ai-fundamentals/blob/main/Instructions/Labs/media/azure-ai-foundry-home-page.png"><img src="https://github.com/MicrosoftLearning/mslearn-ai-fundamentals/blob/main/Instructions/Labs/media/azure-ai-foundry-home-page.png" alt="لقطة شاشة لصفحة Azure AI Foundry الرئيسية مع تحديد إنشاء مشروع." style="max-width: 100%;"></a></p>
</li>
<li>
<p dir="rtl">في جزء <em>إنشاء مشروع</em>، سترى اسم مشروع تم إنشاؤه، والذي يمكنك الاحتفاظ به كما هو. اعتمادًا على ما إذا كنت قد قمت بإنشاء مركز في الماضي، فسترى إما قائمة بالموارد Azure <em>الجديدة</em> التي سيتم إنشاؤها أو قائمة منسدلة بالمراكز الموجودة. إذا رأيت القائمة المنسدلة للمراكز الموجودة، فحدد <em>إنشاء مركز جديد</em>، ثم أنشئ اسمًا فريدًا للمركز الخاص بك، ثم حدد <em>التالي</em>.</p>
<p dir="auto"><a target="_blank" rel="noopener noreferrer" href="https://github.com/MicrosoftLearning/mslearn-ai-fundamentals/blob/main/Instructions/Labs/media/azure-ai-foundry-create-project.png"><img src="https://github.com/MicrosoftLearning/mslearn-ai-fundamentals/blob/main/Instructions/Labs/media/azure-ai-foundry-create-project.png" alt="لقطة شاشة لإنشاء لوحة مشروع مع أسماء تم إنشاؤها تلقائيًا لمركز والمشروع." style="max-width: 100%;"></a></p>
</li>
</ol>
<blockquote>
<p dir="rtl"><strong>هام</strong>: ستحتاج إلى توفير موارد خدمات الذكاء الاصطناعي في Azure في موقع محدد لاستكمال بقية النشاط العملي.</p>
</blockquote>
<ol start="5" dir="rtl">
<li>
<p dir="rtl">في نفس جزء <em>إنشاء مشروع</em>، حدد <strong>تخصيص</strong> ثم حدد أحد <strong>المواقع</strong> التالية: شرق الولايات المتحدة، أو وسط فرنسا، أو وسط كوريا، أو غرب أوروبا، أو غرب الولايات المتحدة لإكمال بقية النشاط العملي. ثم حدد <strong>إنشاء</strong>.</p>
</li>
<li>
<p dir="rtl">لاحظ الموارد التي تم إنشاؤها:</p>
</li>
</ol>
<ul dir="rtl">
<li>خدماتالذكاء الاصطناعي في Azure</li>
<li>مركز الذكاء الاصطناعي في Azure</li>
<li>مشروع الذكاء الاصطناعي في Azure</li>
<li>حساب التخزين</li>
<li>Key Vault</li>
<li>مجموعة الموارد</li>
</ul>
<ol start="6" dir="rtl">
<li>
<p dir="rtl">بعد إنشاء الموارد، سيتم نقلك إلى صفحة <em>نظرة عامة</em> الخاصة بمشروعك.</p>
</li>
<li>
<p dir="rtl">لتتمكن من استخدام "أمان المحتوى"، يتعين عليك إجراء تحديث أذونات لمورد <em>مركز الذكاء الاصطناعي في Azure</em> الخاص بك. للقيام بذلك، افتح <a href="https://portal.azure.com?portal-azure=true" rel="nofollow">بوابة Azure</a> وسجّل الدخول باستخدام نفس الاشتراك الذي استخدمته لإنشاء موارد AI Foundry الخاصة بك.</p>
</li>
<li>
<p dir="rtl">في بوابة Azure، استخدم شريط البحث الموجود أعلى الصفحة للبحث عن <strong>Azure AI Foundry</strong> وتحديده. في صفحة الموارد، حدد المورد الذي أنشأته للتو والذي يكون من <em>النوع</em><strong>مركز الذكاء الاصطناعي في Azure</strong>.</p>
</li>
<li>
<p dir="rtl">في بوابة Azure، في الجزء الأيسر، حدد <strong>التحكم بالوصول (IAM)</strong>. بعد ذلك، في الجزء المفتوح، حدد <strong>إضافة</strong> بجانب علامة الإضافة + وحدد <strong>إضافة تعيين دور</strong>.</p>
</li>
</ol>
<p dir="auto"><a target="_blank" rel="noopener noreferrer" href="https://github.com/MicrosoftLearning/mslearn-ai-fundamentals/blob/main/Instructions/Labs/media/content-safety/access-control-step-one.png"><img src="https://github.com/MicrosoftLearning/mslearn-ai-fundamentals/blob/main/Instructions/Labs/media/content-safety/access-control-step-one.png" alt="لقطة شاشة لمكان تحديد إضافة تعيين دور في جزء التحكم بالوصول." style="max-width: 100%;"></a></p>
<ol start="10" dir="rtl">
<li>
<p dir="rtl">ابحث عن <strong>Azure AI Safety Evaluator</strong> في قائمة الأدوار، ثم حدده. بعد ذلك حدد <strong>التالي</strong>.</p>
</li>
<li>
<p dir="rtl">استخدم الإعدادات التالية لتعيين الدور لنفسك:</p>
<ul dir="rtl">
<li><strong>تعيين الوصول إلى</strong>: حدد <em>المستخدم أو المجموعة أو كيان الخدمة</em></li>
<li><strong>الأعضاء</strong>: انقر فوق <em>تحديد الأعضاء</em>
<ul dir="rtl">
<li>في جزء <em>تحديد الأعضاء</em> المفتوح، ابحث عن اسمك. انقر فوق أيقونة الإضافة بجانب اسمك. ثم انقر فوق "<strong>Select</strong>".</li>
</ul>
</li>
<li><strong>الوصف</strong>: <em>اتركه فارغاً</em></li>
</ul>
</li>
<li>
<p dir="rtl">حدد <strong>مراجعة وتعيين</strong>ثم حدد <strong>مراجعة وتعيين</strong> مجدداً لإضافة تعيين الدور.</p>
</li>
<li>
<p dir="rtl">في متصفحك، عُد إلى <a href="https://ai.azure.com?azure-portal=true" rel="nofollow">مدخل Azure AI Foundry</a>. حدد مشروعك.</p>
</li>
<li>
<p dir="rtl">في القائمة الموجودة على الجانب الأيسر من الشاشة، حدد <strong>خدمات الذكاء الاصطناعي</strong>.</p>
</li>
<p dir="auto"><a target="_blank" rel="noopener noreferrer" href="https://github.com/MicrosoftLearning/mslearn-ai-fundamentals/blob/main/Instructions/Labs/media/azure-ai-foundry-ai-services.png"><img src="https://github.com/MicrosoftLearning/mslearn-ai-fundamentals/blob/main/Instructions/Labs/media/azure-ai-foundry-ai-services.png" alt="لقطة شاشة للقائمة الموجودة على الجانب الأيسر من شاشة المشروع مع تحديد خدمات الذكاء الاصطناعي." style="max-width: 100%;"></a></p>

<li>
<p dir="rtl">في صفحة <em>خدمات الذكاء الاصطناعي</em>، حدد لوحة <em>الرؤية + المستند</em> لتجربة إمكانات المستندات والرؤية من الذكاء الاصطناعي في Azure</p>
</li>
<p dir="auto"><a target="_blank" rel="noopener noreferrer" href="https://github.com/MicrosoftLearning/mslearn-ai-fundamentals/blob/main/Instructions/Labs/media/content-safety-tile.png"><img src="https://github.com/MicrosoftLearning/mslearn-ai-fundamentals/blob/main/Instructions/Labs/media/content-safety-tile.png" alt="لقطة شاشة للوحة &quot;أمان المحتوى&quot;." style="max-width: 100%;"></a></p>

</ol>
<div class="markdown-heading" dir="rtl"><h2 tabindex="-1" class="heading-element" dir="rtl">جرّب تعديل النص باستخدام "أمان المحتوى" في مدخل Azure AI Foundry</h2><a id="user-content-جرّب-تعديل-النص-باستخدام-أمان-المحتوى-في-مدخل-azure-ai-foundry" class="anchor" aria-label="Permalink: جرّب تعديل النص باستخدام &quot;أمان المحتوى&quot; في مدخل Azure AI Foundry" href="#جرّب-تعديل-النص-باستخدام-أمان-المحتوى-في-مدخل-azure-ai-foundry"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<ol dir="rtl">
<li>
<p dir="rtl">في صفحة <em>سلامة المحتوى</em>، ضمن <em>تصفية محتوى النص</em>، حدد <strong>تعديل محتوى النص</strong>.</p>
</li>
<li>
<p dir="rtl">في صفحة <em>تعديل محتوى النص</em>، ضمن عنوان <em>جرّبه</em>، حدد مورد خدمات الذكاء الاصطناعي في Azure الذي قمت بإنشائه للتو من القائمة المنسدلة.</p>
</li>
<li>
<p dir="rtl">ضمن <em>تشغيل اختبار بسيط</em>، حدد لوحة <strong>المحتوى الآمن</strong>. لاحظ أنه يتم عرض النص في المربع أدناه.</p>
</li>
<li>
<p dir="rtl">انقر فوق <strong>تشغيل الاختبار</strong>. يؤدي تشغيل اختبار إلى استدعاء نموذج التعلم العميق لاستوديو سلامة المحتوى. تم بالفعل تدريب نموذج التعلم العميق على التعرف على المحتوى غير الآمن.</p>
</li>
<li>
<p dir="rtl">في لوحة <em>النتائج</em>، افحص النتائج. هناك أربعة مستويات خطورة من آمنة إلى عالية، وأربعة أنواع من المحتوى الضار. هل تعتبر خدمة سلامة المحتوى بالذكاء الاصطناعي أن هذه العينة مقبولة أم لا؟ ما يجب ملاحظته هو أن النتائج تقع ضمن نطاق الثقة. يمكن للنموذج المُدرب جيدًا، مثل أحد نماذج الذكاء الاصطناعي الجاهزة في Azure، إرجاع النتائج التي لديها احتمال كبير لمطابقة ما قد يصنفه الإنسان على النتيجة. في كل مرة تقوم فيها بتشغيل اختبار، يمكنك استدعاء النموذج مرة أخرى.</p>
</li>
<li>
<p dir="rtl">الآن جرّب عينة أخرى. حدد النص ضمن المحتوى العنيف الذي به خطأ إملائي. تحقق من عرض المحتوى في المربع أدناه.</p>
</li>
<li>
<p dir="rtl">انقر فوق <strong>تشغيل الاختبار</strong> وافحص النتائج في لوحة النتائج مرة أخرى.</p>
</li>
</ol>
<p dir="rtl">يمكنك تشغيل الاختبارات على جميع العينات المقدمة، ثم فحص النتائج.</p>
<div class="markdown-heading" dir="rtl"><h2 tabindex="-1" class="heading-element" dir="rtl">التنظيف</h2><a id="user-content-التنظيف" class="anchor" aria-label="Permalink: التنظيف" href="#التنظيف"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="rtl">إذا كنت لا تنوي إجراء المزيد من التدريبات، فاحذف أي موارد لم تعد بحاجة إليها. وهذا يتجنب تراكم أي تكاليف غير ضرورية.</p>
<ol dir="rtl">
<li>افتح <a href="https://portal.azure.com" rel="nofollow">مدخل Azure</a> وحدد مجموعة الموارد التي تحتوي على المورد الذي أنشأته.</li>
<li>حدد المورد وحدد <strong>حذف</strong> ثم <strong>نعم</strong> للتأكيد. من ثم يتم حذف المورد.</li>
</ol>
<div class="markdown-heading" dir="rtl"><h2 tabindex="-1" class="heading-element" dir="rtl">معرفة المزيد</h2><a id="user-content-معرفة-المزيد" class="anchor" aria-label="Permalink: معرفة المزيد" href="#معرفة-المزيد"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="rtl">لقد أظهر هذا التمرين بعضًا فقط من قدرات خدمة "أمان المحتوى". لمعرفة المزيد حول ما يمكنك فعله باستخدام هذه الخدمة، راجع <a href="https://learn.microsoft.com/azure/ai-services/content-safety/overview" rel="nofollow">صفحة "أمان المحتوى"</a>.</p>
</article></div>
