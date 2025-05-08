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
  <td><div dir="rtl">استكشاف الكلام في مدخل Azure AI Foundry</div></td>
  </tr>
  </tbody>
</table>
</div></td>
  </tr>
  </tbody>
</table></markdown-accessiblity-table>

<div class="markdown-heading" dir="rtl"><h1 tabindex="-1" class="heading-element" dir="rtl">استكشاف الكلام في مدخل Azure AI Foundry</h1><a id="user-content-استكشاف-الكلام-في-مدخل-azure-ai-foundry" class="anchor" aria-label="Permalink: استكشاف الكلام في مدخل Azure AI Foundry" href="#استكشاف-الكلام-في-مدخل-azure-ai-foundry"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="rtl">تنسخ خدمة <strong>Azure AI Speech</strong> الكلام إلى نص، والنص إلى كلام مسموع. يمكنك استخدام AI Speech لإنشاء تطبيق يمكنه نسخ ملاحظات الاجتماع أو إنشاء نص من تسجيل المقابلات.</p>
<p dir="rtl">في هذا التمرين، ستستخدم Azure AI Speech في مدخل Azure AI Foundry، وهي منصة Microsoft لإنشاء التطبيقات الذكية، لنسخ الصوت باستخدام التجارب المدمجة.</p>
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
<p dir="rtl">في صفحة <em>خدمات الذكاء الاصطناعي</em>، حدد مربع <em>الكلام</em> لتجربة إمكانات Azure AI Speech.</p>
</li>
<p dir="auto"><a target="_blank" rel="noopener noreferrer" href="https://github.com/MicrosoftLearning/mslearn-ai-fundamentals/blob/main/Instructions/Labs/media/speech-tile.png"><img src="https://github.com/MicrosoftLearning/mslearn-ai-fundamentals/blob/main/Instructions/Labs/media/speech-tile.png" alt="لقطة شاشة للوحة الكلام المحدد في صفحة خدمات الذكاء الاصطناعي." style="max-width: 100%;"></a></p>
</li>
</ol>
<div class="markdown-heading" dir="rtl"><h2 tabindex="-1" class="heading-element" dir="rtl">استكشف تحويل الكلام إلى نص في "بيئة الكلام" الخاصة بـ Azure AI Foundry</h2><a id="user-content-استكشف-تحويل-الكلام-إلى-نص-في-بيئة-الكلام-الخاصة-بـ-azure-ai-foundry" class="anchor" aria-label="Permalink: استكشف تحويل الكلام إلى نص في &quot;بيئة الكلام&quot; الخاصة بـ Azure AI Foundry" href="#استكشف-تحويل-الكلام-إلى-نص-في-بيئة-الكلام-الخاصة-بـ-azure-ai-foundry"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="rtl">دعنا نجرب <em>تحويل الكلام إلى نص</em> في "بيئة الكلام" الخاصة بـ Azure AI Foundry.</p>
<ol dir="rtl">
<li>
<p dir="rtl">في صفحة <em>الكلام</em>، مرّر للأسفل وحدد <strong>كتابة الحديث في الوقت الفعلي</strong> ضمن <em>تجربة إمكانات الكلام</em>. سيتم نقلك إلى <em>بيئة الكلام</em>.</p>
</li>
<li>
<p dir="rtl">حدد <a href="https://aka.ms/mslearn-speech-files" rel="nofollow"><strong>https://aka.ms/mslearn-speech-files</strong></a>لتنزيل <strong>speech.zip</strong>. افتح المجلد.</p>
</li>
<li>
<p dir="rtl">ضمن <em>تحميل الملفات</em>، حدد <strong>تصفح الملفات</strong> وانتقل إلى المجلد الذي قمت بحفظ الملف فيه. حدد <strong>WhatAICanDo.m4a</strong> ثم <strong>فتح</strong>.</p>
</li>
<p dir="auto"><a target="_blank" rel="noopener noreferrer" href="https://github.com/MicrosoftLearning/mslearn-ai-fundamentals/blob/main/Instructions/Labs/media/recognize-synthesize-speech/browse-files-speech.png"><img src="https://github.com/MicrosoftLearning/mslearn-ai-fundamentals/blob/main/Instructions/Labs/media/recognize-synthesize-speech/browse-files-speech.png" alt="تصفح ملفات" style="max-width: 100%;"></a></p>
</li>
<li>
<p dir="rtl">تنسخ خدمة Speech النص وتعرضه في الوقت الحقيقي. إذا كان لديك صوت على الكمبيوتر، يمكنك الاستماع إلى التسجيل أثناء نسخ النص.</p>
</li>
<li>
<p dir="rtl">راجع الإخراج، الذي كان يجب أن يتعرف على الصوت وينسخه بنجاح إلى نص.</p>
</li>
</ol>
<p dir="rtl">في هذا التمرين، جرّبت خدمات Azure AI Speech في "بيئة الكلام" الخاصة بـ Azure AI Foundry. ثم استخدمت كتابة الحديث في الوقت الفعلي لنسخ تسجيل صوتي. كنت قادراً على رؤية كتابة النص الذي يتم إنشاؤه أثناء تشغيل الملف الصوتي.</p>
<div class="markdown-heading" dir="rtl"><h2 tabindex="-1" class="heading-element" dir="rtl">تنظيف</h2><a id="user-content-تنظيف" class="anchor" aria-label="Permalink: تنظيف" href="#تنظيف"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="rtl">إذا كنت لا تنوي القيام بمزيد من التمارين، فاحذف أي موارد لم تعد بحاجة إليها. وهذا يتجنب تراكم أي تكاليف غير ضرورية.</p>
<ol dir="rtl">
<li>افتح <a href="https://portal.azure.com" rel="nofollow">مدخل Azure</a> وحدد مجموعة الموارد التي تحتوي على المورد الذي أنشأته.</li>
<li>حدد المورد وحدد <strong>حذف</strong> ثم <strong>نعم</strong> للتأكيد. من ثم يتم حذف المورد.</li>
</ol>
<div class="markdown-heading" dir="rtl"><h2 tabindex="-1" class="heading-element" dir="rtl">معرفة المزيد</h2><a id="user-content-معرفة-المزيد" class="anchor" aria-label="Permalink: معرفة المزيد" href="#معرفة-المزيد"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="rtl">أظهر هذا التمرين إحدى القدرات العديدة التي تتمتع بها خدمة الكلام. لمعرفة المزيد حول ما يمكنك القيام به باستخدام هذه الخدمة، راجع <a href="https://azure.microsoft.com/services/cognitive-services/speech-services" rel="nofollow">صفحة الكلام</a>.</p>
</article></div>
