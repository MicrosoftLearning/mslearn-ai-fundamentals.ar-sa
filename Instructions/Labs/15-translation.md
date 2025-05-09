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
  <td><div dir="rtl">استكشف Azure AI Translator</div></td>
  </tr>
  </tbody>
</table>
</div></td>
  </tr>
  </tbody>
</table></markdown-accessiblity-table>

<div class="markdown-heading" dir="rtl"><h1 tabindex="-1" class="heading-element" dir="rtl">استكشف Azure AI Translator</h1><a id="user-content-استكشف-azure-ai-translator" class="anchor" aria-label="Permalink: استكشف Azure AI Translator" href="#استكشف-azure-ai-translator"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<blockquote>
<p dir="rtl"><strong>ملاحظة</strong> لإكمال هذا النشاط المعملي، ستحتاج إلى <a href="https://azure.microsoft.com/free?azure-portal=true" rel="nofollow">اشتراك Azure</a> الذي لديك فيه حق الوصول الإداري.</p>
</blockquote>
<p dir="rtl">يمكن أن يساعد الذكاء الاصطناعي في تبسيط عملية الترجمة بين اللغات، مما يساعد في إزالة الحواجز التي تحول دون التواصل بين البلدان والثقافات.</p>
<p dir="rtl">لاختبار قدرات خدمة Azure AI Translator، سنلقي نظرة عليه أثناء العمل في بوابة Azure. تنطبق نفس المبادئ والوظائف في حلول العالم الحقيقي، مثل مواقع الويب أو تطبيقات الهاتف.</p>
<div class="markdown-heading" dir="rtl"><h2 tabindex="-1" class="heading-element" dir="rtl">إنشاء مورد <em>المترجم</em></h2><a id="user-content-إنشاء-مورد-المترجم" class="anchor" aria-label="Permalink: إنشاء مورد المترجم" href="#إنشاء-مورد-المترجم"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="rtl">يمكنك استخدام خدمة المترجم عن طريق إنشاء إما مورد <strong>مترجم</strong> أو مورد <strong>خدمات ذكاء اصطناعي في Azure</strong>.</p>
<p dir="rtl">لهذا التمرين، أنشئ مورد <strong>المترجم</strong> في اشتراك Azure الخاص بك.</p>
<ol dir="rtl">
<li>
<p dir="rtl">في علامة تبويب مستعرض أخرى، افتح مدخل Azure في <a href="https://portal.azure.com?azure-portal=true" rel="nofollow">https://portal.azure.com</a>، وقم بتسجيل الدخول باستخدام حساب Microsoft الخاص بك.</p>
</li>
<li>
<p dir="rtl">انقر فوق الزر <strong>＋إنشاء مورد</strong> وابحث عن <em>المترجم</em>. حدد <strong>إنشاء</strong>. سيتم نقلك إلى صفحة لإنشاء مورد المترجم. قم بتكوينه بالإعدادات التالية:</p>
<ul dir="rtl">
<li><strong>الاشتراك</strong>: <em>اشتراك Azure الخاص بك</em>.</li>
<li><strong>مجموعة الموارد</strong>: <em>أنشئ مجموعة موارد جديدة ذات اسم فريد</em>.</li>
<li><strong>Region</strong>: <em>اختر أي منطقة متوفرة</em>.</li>
<li><strong>الاسم</strong>: <em>أدخل اسمًا مميزًا</em>.</li>
<li><strong>مستوى التسعير</strong>: قياسي S0</li>
</ul>
</li>
<li>
<p dir="rtl">راجع المورد وأنشئه، وانتظر حتى يكتمل التوزيع. ثم انتقل إلى المورد الموزع.</p>
</li>
</ol>
<div class="markdown-heading" dir="rtl"><h2 tabindex="-1" class="heading-element" dir="rtl">استكشف خدمة المترجم</h2><a id="user-content-استكشف-خدمة-المترجم" class="anchor" aria-label="Permalink: استكشف خدمة المترجم" href="#استكشف-خدمة-المترجم"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="rtl">يمكننا استكشاف إمكانيات خدمة المترجم في بوابة Azure.</p>
<ol dir="rtl">
<li>
<p dir="rtl">في بوابة Azure، في المورد الموزع، راجع صفحة <em>نظرة عامة</em>.</p>
</li>
<p dir="auto"><a target="_blank" rel="noopener noreferrer" href="https://github.com/MicrosoftLearning/mslearn-ai-fundamentals/blob/main/Instructions/Labs/media/use-translator/translator-azure-portal.png"><img src="https://github.com/MicrosoftLearning/mslearn-ai-fundamentals/blob/main/Instructions/Labs/media/use-translator/translator-azure-portal.png" alt="لقطة شاشة لصفحة النظرة العامة لمورد المترجم." style="max-width: 100%;"></a></p>
</li>
<li>
<p dir="rtl">في قسم <em>جربه</em> من صفحة النظرة العامة، ضمن قسم <em>من: الكشف التلقائي</em>، اكتب النص <code>Welcome to Azure AI Fundamentals</code>. لاحظ JSON الذي يظهر في المراسلات في قسم <em>عرض الطلب</em>.</p>
</li>
<li>
<p dir="rtl">في قسم <em>عرض الاستجابة</em>، اعرض ملف JSON. في الخلفية، تم إرسال <em>طلب</em> إلى خدمة المترجم. تتضمن <em>الاستجابة</em> لغة المصدر المكتشفة مع درجة الثقة، والترجمة باستخدام أبجدية لغة الإخراج، ورمز لغة الإخراج.</p>
</li>
<li>
<p dir="rtl">يُظهر العرض التوضيحي الموجود في قسم <em>جربه</em> كيف سيبدو الأمر إذا قمت بإنشاء تطبيق ترجمة بسيط بواجهة مستخدم. في حالة العرض التوضيحي، بمجرد كتابة النص، يتم تقديم طلب إلى خدمة المترجم. كيف يمكنك إجراء هذا الطلب؟ تفضل بزيارة علامة التبويب <em>نموذج التعليمة البرمجية</em>. ستجد هنا أمثلة على تعليمات برمجية بلغات برمجة مختلفة يمكن استخدامها لإنشاء الطلب.</p>
</li>
<li>
<p dir="rtl">حدد الأسطر الموجودة في عينات التعليمات البرمجية حيث تحتاج إلى تضمين <strong>المفتاح</strong> و<strong>نقطة النهاية</strong> لخدمة المترجم الخاصة بك. باستخدام مفتاحك ونقطة النهاية، ستتمكن من إرسال طلب إلى خدمة المترجم، وتلقي استجابة كما رأيتها في العرض التوضيحي.</p>
</li>
<li>
<p dir="rtl">انتقل إلى القائمة الموجودة على الجانب الأيسر. ضمن "<em>Resource Management</em>"، حدد "<em>Keys and Endpoint</em>". إذا كنت تريد إنشاء تطبيق، فستجد مفتاحك ونقطة النهاية هنا.</p>
</li>
</ol>
<div class="markdown-heading" dir="rtl"><h2 tabindex="-1" class="heading-element" dir="rtl">التنظيف</h2><a id="user-content-التنظيف" class="anchor" aria-label="Permalink: التنظيف" href="#التنظيف"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<ol dir="rtl">
<li>احذف موردك بمجرد الانتهاء من استخدامه.</li>
</ol>
<div class="markdown-heading" dir="rtl"><h2 tabindex="-1" class="heading-element" dir="rtl">معرفة المزيد</h2><a id="user-content-معرفة-المزيد" class="anchor" aria-label="Permalink: معرفة المزيد" href="#معرفة-المزيد"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="rtl">لمعرفة المزيد حول ما يمكنك القيام به مع هذه الخدمة، راجع <a href="https://learn.microsoft.com/en-us/azure/ai-services/translator/translator-overview" rel="nofollow">صفحة Translator</a>.</p>
</article></div>
