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
  <td><div dir="rtl">استخراج البيانات من المستندات في مدخل Azure AI Foundry</div></td>
  </tr>
  </tbody>
</table>
</div></td>
  </tr>
  </tbody>
</table></markdown-accessiblity-table>

<div class="markdown-heading" dir="rtl"><h1 tabindex="-1" class="heading-element" dir="rtl">استخراج البيانات من المستندات في مدخل Azure AI Foundry</h1><a id="user-content-استخراج-البيانات-من-المستندات-في-مدخل-azure-ai-foundry" class="anchor" aria-label="Permalink: استخراج البيانات من المستندات في مدخل Azure AI Foundry" href="#استخراج-البيانات-من-المستندات-في-مدخل-azure-ai-foundry"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="rtl">تتيح لك خدمة <strong>ذكاء المستندات باستخدام الذكاء الاصطناعي في Azure</strong> تحليل المعلومات واستخراجها من النماذج والمستندات، ثم تحديد أسماء الحقول والبيانات.</p>
<p dir="rtl">كيف يعتمد Document Intelligence على التعرف البصري على الحروف (OCR)؟ بينما يمكن لـ OCR قراءة المستندات المطبوعة أو المكتوبة بخط اليد، يستخرج التعرف البصري على الحروف النص بتنسيق غير منظم يصعب تخزينه في قاعدة بيانات أو تحليله. يساعد ذكاء المستندات على فهم البيانات غير المنظمة من خلال التقاط بنية النص، مثل حقول البيانات والمعلومات الموجودة في الجداول.</p>
<p dir="rtl">في هذا التمرين، ستستخدم النماذج المعدة مسبقًا من ذكاء المستندات باستخدام الذكاء الاصطناعي في Azure في مدخل Azure AI Foundry، وهي منصة Microsoft لإنشاء التطبيقات الذكية، للتعرف على البيانات من استلام.</p>
<div class="markdown-heading" dir="rtl"><h2 tabindex="-1" class="heading-element" dir="rtl">إنشاء مشروع في مدخل Azure AI Foundry</h2><a id="user-content-إنشاء-مشروع-في-مدخل-azure-ai-foundry" class="anchor" aria-label="Permalink: إنشاء مشروع في مدخل Azure AI Foundry" href="#إنشاء-مشروع-في-مدخل-azure-ai-foundry"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<ol dir="rtl">
<li>
<p dir="rtl">في علامة تبويب المتصفح، انتقل إلى <a href="https://ai.azure.com?azure-portal=true" rel="nofollow">Azure AI Foundry</a>.</p>
</li>
<li>
<p dir="rtl">سجل الدخول باستخدام حسابك.</p>
</li>
<li>
<p dir="rtl">في الصفحة الرئيسية لمدخل Azure AI Foundry، حدد <strong>إنشاء مشروع</strong>. في Azure AI Foundry، تعتبر المشاريع عبارة عن حاويات تساعد في تنظيم عملك.</p>
</li>
<p dir="auto"><a target="_blank" rel="noopener noreferrer" href="https://github.com/MicrosoftLearning/mslearn-ai-fundamentals/blob/main/Instructions/Labs/media/azure-ai-foundry-home-page.png"><img src="https://github.com/MicrosoftLearning/mslearn-ai-fundamentals/blob/main/Instructions/Labs/media/azure-ai-foundry-home-page.png" alt="لقطة شاشة لصفحة Azure AI Foundry الرئيسية مع تحديد إنشاء مشروع." style="max-width: 100%;"></a></p>
</li>
<li>
<p dir="rtl">في جزء <em>إنشاء مشروع</em>، سترى اسم مشروع تم إنشاؤه، والذي يمكنك الاحتفاظ به كما هو. اعتمادًا على ما إذا كنت قد قمت بإنشاء مركز في الماضي، فسترى إما قائمة بالموارد Azure <em>الجديدة</em> التي سيتم إنشاؤها أو قائمة منسدلة بالمراكز الموجودة. إذا رأيت القائمة المنسدلة للمراكز الموجودة، فحدد <em>إنشاء مركز جديد</em>، ثم أنشئ اسمًا فريدًا للمركز الخاص بك، ثم حدد <em>التالي</em>.</p>
</li>
<p dir="auto"><a target="_blank" rel="noopener noreferrer" href="https://github.com/MicrosoftLearning/mslearn-ai-fundamentals/blob/main/Instructions/Labs/media/azure-ai-foundry-create-project.png"><img src="https://github.com/MicrosoftLearning/mslearn-ai-fundamentals/blob/main/Instructions/Labs/media/azure-ai-foundry-create-project.png" alt="لقطة شاشة لإنشاء لوحة مشروع مع أسماء تم إنشاؤها تلقائيًا لمركز والمشروع." style="max-width: 100%;"></a></p>
</li>
</ol>
<blockquote>
<p dir="rtl"><strong>هام</strong>: ستحتاج إلى توفير موارد خدمات الذكاء الاصطناعي في Azure في موقع محدد لاستكمال بقية النشاط العملي.</p>
</blockquote>
<ol dir="rtl">
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
<ol dir="rtl">
<li>
<p dir="rtl">بعد إنشاء الموارد، سيتم نقلك إلى صفحة <em>نظرة عامة</em> الخاصة بمشروعك. في القائمة الموجودة على الجانب الأيسر من الشاشة، حدد <strong>خدمات الذكاء الاصطناعي</strong>.</p>
</li>
<p dir="auto"><a target="_blank" rel="noopener noreferrer" href="https://github.com/MicrosoftLearning/mslearn-ai-fundamentals/blob/main/Instructions/Labs/media/azure-ai-foundry-ai-services.png"><img src="https://github.com/MicrosoftLearning/mslearn-ai-fundamentals/blob/main/Instructions/Labs/media/azure-ai-foundry-ai-services.png" alt="لقطة شاشة للقائمة الموجودة على الجانب الأيسر من شاشة المشروع مع تحديد خدمات الذكاء الاصطناعي." style="max-width: 100%;"></a></p>
</li>
<li>
<p dir="rtl">في صفحة <em>خدمات الذكاء الاصطناعي</em>، حدد مربع <em>الرؤية + المستند</em> لتجربة إمكانات ذكاء المستندات باستخدام الذكاء الاصطناعي في Azure.</p>
</li>
<p dir="auto"><a target="_blank" rel="noopener noreferrer" href="https://github.com/MicrosoftLearning/mslearn-ai-fundamentals/blob/main/Instructions/Labs/media/vision-document-tile.png"><img src="https://github.com/MicrosoftLearning/mslearn-ai-fundamentals/blob/main/Instructions/Labs/media/vision-document-tile.png" alt="لقطة شاشة للوحة الرؤية والوثيقة المحددين في صفحة خدمات الذكاء الاصطناعي." style="max-width: 100%;"></a></p>
</li>
</ol>
<div class="markdown-heading" dir="rtl"><h2 tabindex="-1" class="heading-element" dir="rtl">تحليل استلام باستخدام ذكاء المستندات باستخدام الذكاء الاصطناعي في Azure في Azure AI Foundry</h2><a id="user-content-تحليل-استلام-باستخدام-ذكاء-المستندات-باستخدام-الذكاء-الاصطناعي-في-azure-في-azure-ai-foundry" class="anchor" aria-label="Permalink: تحليل استلام باستخدام ذكاء المستندات باستخدام الذكاء الاصطناعي في Azure في Azure AI Foundry" href="#تحليل-استلام-باستخدام-ذكاء-المستندات-باستخدام-الذكاء-الاصطناعي-في-azure-في-azure-ai-foundry"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="rtl">أنت الآن جاهز لتحليل إيصال لشركة البيع بالتجزئة في Northwind Traders الوهمية.</p>
<ol dir="rtl">
<li>
<p dir="rtl">في صفحة <em>الرؤية + المستند</em>، مرّر لأسفل وحدد <strong>المستند</strong>. تحت <em>النماذج المعدة مسبقًا لمستندات محددة</em>، حدد لوحة <strong>الاستلامات</strong>.</p>
</li>
<li>
<p dir="rtl">في القائمة المنسدلة ضمن <em>جربه</em>، لاحظ أنه تم تحديد مورد خدمات الذكاء الاصطناعي في Azure الخاص بك. اتركه كما هو.</p>
</li>
<li>
<p dir="rtl">على حاسوبك، استخدم <a href="https://aka.ms/mslearn-receipt" rel="nofollow"><strong>https://aka.ms/mslearn-receipt</strong></a> لفتح صورة نموذجية لاستلام. احفظه في مجلد التنزيلات أو على سطح المكتب.</p>
</li>
<li>
<p dir="rtl">في Azure AI Foundry، في صفحة <em>الاستلامات</em>، حدد <strong>تصفح الملفات</strong> وانتقل إلى المجلد حيث حفظت الصورة. حدد صورة الإيصال ثم <strong>فتح</strong>. تظهر الصورة على الجانب الأيمن من الشاشة.</p>
</li>
<p dir="auto"><a target="_blank" rel="noopener noreferrer" href="https://github.com/MicrosoftLearning/mslearn-ai-fundamentals/blob/main/Instructions/Labs/media/document-intelligence/receipt.jpg"><img src="https://github.com/MicrosoftLearning/mslearn-ai-fundamentals/blob/main/Instructions/Labs/media/document-intelligence/receipt.jpg" alt="لقطة شاشة لاستلام northwind." style="max-width: 100%;"></a></p>
</li>
<li>
<p dir="rtl">على اليمين، حدد <strong>تشغيل التحليلات</strong>.</p>
</li>
<li>
<p dir="rtl">عند تشغيل التحليل، يتم إرجاع النتائج. لاحظ أن الخدمة تعرفت على حقول بيانات محددة مثل اسم التاجر والعنوان ورقم الهاتف وتاريخ المعاملة ووقتها، بالإضافة إلى البنود والإجمالي الفرعي والضريبة والمبالغ الإجمالية. بجوار كل حقل توجد نسبة احتمالية أن يكون الحقل صحيحًا.</p>
</li>
<p dir="auto"><a target="_blank" rel="noopener noreferrer" href="https://github.com/MicrosoftLearning/mslearn-ai-fundamentals/blob/main/Instructions/Labs/media/receipt-lab-result.png"><img src="https://github.com/MicrosoftLearning/mslearn-ai-fundamentals/blob/main/Instructions/Labs/media/receipt-lab-result.png" alt="لقطة شاشة لنتيجة تحليل الاستلام في مدخل Azure AI Foundry، تُظهر المربعات المحددة حول حقول البيانات والنص في تلك الحقول المستخرجة." style="max-width: 100%;"></a></p>
</li>
</ol>
<p dir="rtl">في هذا التمرين، استخدمت نموذج الاستلامات المُعد مسبقًا لذكاء المستندات باستخدام الذكاء الاصطناعي في Azure في مدخل Azure AI Foundry. من النتائج التي تم إرجاعها، رأيت كيف تمكنت Document Intelligence من تحديد حقول معينة، مما يتيح معالجة البيانات من المستندات اليومية بسهولة أكبر. قبل إغلاق العرض التوضيحي، لماذا لا تجرب بعض الاستلامات النموذجية، بما في ذلك تلك الموجودة بلغات مختلفة؟</p>
<div class="markdown-heading" dir="rtl"><h2 tabindex="-1" class="heading-element" dir="rtl">تنظيف</h2><a id="user-content-تنظيف" class="anchor" aria-label="Permalink: تنظيف" href="#تنظيف"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="rtl">إذا كنت لا تنوي إجراء المزيد من التدريبات، فاحذف أي موارد لم تعد بحاجة إليها. وهذا يتجنب تراكم أي تكاليف غير ضرورية.</p>
<ol dir="rtl">
<li>افتح <a href="https://portal.azure.com" rel="nofollow">مدخل Azure</a> وحدد مجموعة الموارد التي تحتوي على المورد الذي أنشأته.</li>
<li>حدد المورد وحدد <strong>حذف</strong> ثم <strong>نعم</strong> للتأكيد. من ثم يتم حذف المورد.</li>
</ol>
<div class="markdown-heading" dir="rtl"><h2 tabindex="-1" class="heading-element" dir="rtl">معرفة المزيد</h2><a id="user-content-معرفة-المزيد" class="anchor" aria-label="Permalink: معرفة المزيد" href="#معرفة-المزيد"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="rtl">أظهر هذا التمرين فقط بعض قدرات خدمة الذكاء الاصطناعي Document Intelligence. للتعّرف على المزيد حول ما يمكنك القيام به مع هذه الخدمة، يرجى مراجعة<a href="https://learn.microsoft.com/azure/ai-services/document-intelligence/overview?view=doc-intel-3.1.0" rel="nofollow">صفحة Document Intelligence</a>.</p>
</article></div>
