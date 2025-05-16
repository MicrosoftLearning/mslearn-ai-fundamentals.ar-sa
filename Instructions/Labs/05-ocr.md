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
  <td><div dir="rtl">قراءة النص في Vision Studio</div></td>
  </tr>
  </tbody>
</table>
</div></td>
  </tr>
  </tbody>
</table></markdown-accessiblity-table>

<div class="markdown-heading" dir="rtl"><h1 tabindex="-1" class="heading-element" dir="rtl">قراءة النص في Vision Studio</h1><a id="user-content-قراءة-النص-في-vision-studio" class="anchor" aria-label="Permalink: قراءة النص في Vision Studio" href="#قراءة-النص-في-vision-studio"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="rtl">في هذا التمرين، ستستخدم خدمة الذكاء الاصطناعي في Azure لاستكشاف قدرات التعرّف البصري على الحروف في Azure AI Vision. ستستخدم Vision Studio لتجربة استخراج النص من الصور، دون الحاجة إلى كتابة أي تعليمات برمجية.</p>
<p dir="rtl">يتمثل أحد التحديات الشائعة في الرؤية الخاصة بالكمبيوتر في اكتشاف النص المُضمَّن في صورة ما وتفسيره. يُعرَف هذا باسم التعرّف البصري على الحروف (OCR). في هذا التمرين، ستستخدم مورد خدمات الذكاء الاصطناعي في Azure، والذي يتضمن خدمات Azure AI Vision. ثم ستستخدم Vision Studio لتجربة التعرّف البصري على الحروف (OCR) باستخدام أنواع مختلفة من الصور.</p>
<div class="markdown-heading" dir="rtl"><h2 tabindex="-1" class="heading-element" dir="rtl">إنشاء مورد <em>خدمات ذكاء اصطناعي في Azure</em></h2><a id="user-content-إنشاء-مورد-خدمات-ذكاء-اصطناعي-في-azure" class="anchor" aria-label="Permalink: إنشاء مورد خدمات ذكاء اصطناعي في Azure" href="#إنشاء-مورد-خدمات-ذكاء-اصطناعي-في-azure"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="rtl">يمكنك استخدام قدرات التعرّف البصري على الحروف الموجودة في Azure AI Vision من خلال مورد متعدد الخدمات لـ <strong>خدمات الذكاء الاصطناعي في Azure</strong>. إذا لم تكن قد قمت بذلك بالفعل، فأنشئ مورد <strong>خدمات ذكاء اصطناعي في Azure</strong> في اشتراكك في Azure.</p>
<ol dir="rtl">
<li>
<p dir="rtl">في علامة تبويب مستعرض آخر، افتح <strong>مُدخل Azure</strong> على <a href="https://portal.azure.com?azure-portal=true" rel="nofollow">https://portal.azure.com</a>، وقم بتسجيل الدخول باستخدام حساب Microsoft المرتبط باشتراكك في Azure.</p>
</li>
<li>
<p dir="rtl">انقر فوق زر <strong>＋أنشئ مورد</strong> وابحث عن <em>خدمات ذكاء اصطناعي في Azure</em>. حدد <strong>إنشاء</strong> <strong>خطة خدمات الذكاء الاصطناعي في Azure</strong>. سيتم نقلك إلى صفحة لإنشاء مورد خدمات ذكاء اصطناعي في Azure. قم بتكوينه بالإعدادات التالية:</p>
<ul dir="rtl">
<li><strong>الاشتراك</strong>: <em>اشتراك Azure الخاص بك</em>.</li>
<li><strong>مجموعة الموارد</strong>: <em>أنشئ مجموعة موارد جديدة ذات اسم فريد</em>.</li>
<li><strong>المنطقة</strong>: <em>حدد أقرب منطقة جغرافية لك. إذا كنت في شرق الولايات المتحدة، فاستخدم "شرق الولايات المتحدة 2"</em>.</li>
<li><strong>الاسم</strong>: <em>أدخل اسمًا مميزًا</em>.</li>
<li><strong>مستوى الأسعار</strong>: <em>القياسي (S0).</em></li>
<li><strong>من خلال تحديد هذا المربع، أقر بأنني قرأت وفهمت جميع الشروط أدناه:</strong> <em>محدد</em>.</li>
</ul>
</li>
<li>
<p dir="rtl">حدد <strong>مراجعة + إنشاء</strong> ثم <strong>إنشاء</strong> وانتظر حتى يكتمل التوزيع.</p>
</li>
</ol>
<div class="markdown-heading" dir="rtl"><h2 tabindex="-1" class="heading-element" dir="rtl">توصيل مورد خدمة Azure الذكاء الاصطناعي Vision Studio</h2><a id="user-content-توصيل-مورد-خدمة-azure-الذكاء-الاصطناعي-vision-studio" class="anchor" aria-label="Permalink: توصيل مورد خدمة Azure الذكاء الاصطناعي Vision Studio" href="#توصيل-مورد-خدمة-azure-الذكاء-الاصطناعي-vision-studio"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="rtl">بعد ذلك، قم بتوصيل مورد خدمات Azure الذكاء الاصطناعي الذي قمت بتوفيره أعلاه لـ Vision Studio.</p>
<ol dir="rtl">
<li>
<p dir="rtl">في علامة تبويب متصفح أخرى، انتقل إلى <strong>Vision Studio</strong> في<a href="https://portal.vision.cognitive.azure.com?azure-portal=true" rel="nofollow">https://portal.vision.cognitive.azure.com</a>.</p>
</li>
<li>
<p dir="rtl">سجل الدخول باستخدام حسابك وتأكد من أنك تستخدم نفس الدليل الذي أنشأت فيه مورد خدمات Azure الذكاء الاصطناعي.</p>
</li>
<li>
<p dir="rtl">في الصفحة الرئيسية لـ Vision Studio، حدد <strong>عرض كل المصادر</strong> ضمن <strong>عنوان بدء استخدام Vision</strong>.</p>
</li>
<p dir="auto"><a target="_blank" rel="noopener noreferrer" href="https://github.com/MicrosoftLearning/mslearn-ai-fundamentals/blob/main/Instructions/Labs/media/analyze-images-vision/vision-resources.png"><img src="https://github.com/MicrosoftLearning/mslearn-ai-fundamentals/blob/main/Instructions/Labs/media/analyze-images-vision/vision-resources.png" alt="يتم تمييز ارتباط &quot;عرض كل المصادر&quot; ضمن بدء استخدام Vision في Vision Studio." style="max-width: 100%;"></a></p>
</li>
<li>
<p dir="rtl">في <strong>الصفحة تحديد مورد للعمل معه</strong>، مرر مؤشر الماوس فوق المورد الذي أنشأته أعلاه في القائمة ثم حدد المربع إلى يسار اسم المورد، ثم حدد <strong>تحديد كمورد</strong> افتراضي.</p>
<blockquote>
<p dir="rtl"><strong>ملاحظة</strong> : إذا لم يتم عرض المورد الخاص بك بعد، فقد تحتاج إلى <strong>تحديث</strong> الصفحة.</p>
</li>
</blockquote>
<p dir="auto"><a target="_blank" rel="noopener noreferrer" href="https://github.com/MicrosoftLearning/mslearn-ai-fundamentals/blob/main/Instructions/Labs/media/analyze-images-vision/default-resource.png"><img src="https://github.com/MicrosoftLearning/mslearn-ai-fundamentals/blob/main/Instructions/Labs/media/analyze-images-vision/default-resource.png" alt="يتم عرض &quot;تحديد مصدر للعمل مع مربع الحوار&quot; مع تمييز cog-ms-learn-vision-SUFFIX مورد الخدمات المعرفية وفحصه. يتم تمييز الزر &quot;تحديد كمورد افتراضي&quot;." style="max-width: 100%;"></a></p>
</li>
<li>
<p dir="rtl">أغلق صفحة الإعدادات عن طريق تحديد "x" في أعلى يمين الشاشة.</p>
</li>
</ol>
<div class="markdown-heading" dir="rtl"><h2 tabindex="-1" class="heading-element" dir="rtl">استخراج النص من الصور في Vision Studio</h2><a id="user-content-استخراج-النص-من-الصور-في-vision-studio" class="anchor" aria-label="Permalink: استخراج النص من الصور في Vision Studio" href="#استخراج-النص-من-الصور-في-vision-studio"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<ol dir="rtl">
<li>
<p dir="rtl">في مستعرض ويب، انتقل إلى <strong>Vision Studio</strong> في <a href="https://portal.vision.cognitive.azure.com?azure-portal=true" rel="nofollow">https://portal.vision.cognitive.azure.com</a>.</p>
</li>
<li>
<p dir="rtl">في الصفحة المقصودة <strong>بدء استخدام Vision</strong>، حدّد <strong>التعرّف البصري على الحروف</strong>، ثم لوحة <strong>استخراج النص من الصور</strong>.</p>
</li>
<li>
<p dir="rtl">ضمن العنوان الفرعي <strong>تجربة الخدمة</strong>، أقر بنهج استخدام الموارد عن طريق قراءة المربع وتحديده.</p>
</li>
<li>
<p dir="rtl">حدّد <a href="https://aka.ms/mslearn-ocr-images" rel="nofollow"><strong>https://aka.ms/mslearn-ocr-images</strong></a> لتنزيل <strong>ocr-images.zip</strong>. ثم افتح المجلد.</p>
</li>
<li>
<p dir="rtl">في المُدخل، حدّد <strong>استعراض بحثًا عن ملف</strong> وانتقل إلى المجلد على جهاز الكمبيوتر الخاص بك حيث قمت بتنزيل <strong>ocr-images.zip</strong>. حدّد <strong>advert.jpg</strong> وحدّد <strong>فتح</strong>.</p>
</li>
<li>
<p dir="rtl">راجع الآن ما تم إرجاعه:</p>
<ul dir="rtl">
<li>في <strong>السمات المكتشفة</strong>، يُنَظم أي نص موجود في الصورة في بنية هرمية للمناطق والخطوط والكلمات.</li>
<li>في الصورة، يُشار إلى موقع النص بواسطة مربع إحاطة، كما هو موضح هنا:</li>
</ul>
</li>
<p dir="auto"><a target="_blank" rel="noopener noreferrer" href="https://github.com/MicrosoftLearning/mslearn-ai-fundamentals/blob/main/Instructions/Labs/media/read-text-computer-vision/advert-bounding-boxes.jpg"><img src="https://github.com/MicrosoftLearning/mslearn-ai-fundamentals/blob/main/Instructions/Labs/media/read-text-computer-vision/advert-bounding-boxes.jpg" alt="صورة للنص في الصورة الموضحة." style="max-width: 100%;"></a></p>
</li>
<li>
<p dir="rtl">يمكنك الآن تجربة صورة أخرى. حدّد <strong>استعراض بحثًا عن ملف</strong> وانتقل إلى المجلد حيث حفظت الصورة من GitHub. حدّد <strong>letter.jpg</strong>.</p>
</li>
<p dir="auto"><a target="_blank" rel="noopener noreferrer" href="https://github.com/MicrosoftLearning/mslearn-ai-fundamentals/blob/main/Instructions/Labs/media/read-text-computer-vision/letter.jpg"><img src="https://github.com/MicrosoftLearning/mslearn-ai-fundamentals/blob/main/Instructions/Labs/media/read-text-computer-vision/letter.jpg" alt="صورة لرسالة مطبوعة." style="max-width: 100%;"></a></p>
</li>
<li>
<p dir="rtl">راجع نتائج الصورة الثانية. يجب أن ترجع النص والمربعات المحيطة بالنص. إذا كان لديك الوقت، فجرب <strong>note.jpg</strong> و<strong>receipt.jpg</strong>.</p>
</li>
</ol>
<div class="markdown-heading" dir="rtl"><h2 tabindex="-1" class="heading-element" dir="rtl">تنظيف</h2><a id="user-content-تنظيف" class="anchor" aria-label="Permalink: تنظيف" href="#تنظيف"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="rtl">إذا كنت لا تنوي إجراء المزيد من التدريبات، فاحذف أي موارد لم تعد بحاجة إليها. وهذا يتجنب تكبد أي تكاليف غير ضرورية.</p>
<ol dir="rtl">
<li>افتح <strong>مدخل Azure</strong> في <a href="https://portal.azure.com?azure-portal=true" rel="nofollow">https://portal.azure.com</a> وحدد مجموعة الموارد التي تحتوي على المورد الذي أنشأته.</li>
<li>حدد المورد وحدد <strong>حذف</strong> ثم <strong>نعم</strong> للتأكيد. من ثم يتم حذف المورد.</li>
</ol>
<div class="markdown-heading" dir="rtl"><h2 tabindex="-1" class="heading-element" dir="rtl">معرفة المزيد</h2><a id="user-content-معرفة-المزيد" class="anchor" aria-label="Permalink: معرفة المزيد" href="#معرفة-المزيد"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="rtl">للتعرّف على المزيد حول ما يمكنك القيام به من خلال استخدام هذه الخدمة، فاطّلع على وثائق Azure AI Vision حول <a href="https://learn.microsoft.com/azure/ai-services/computer-vision/overview-ocr" rel="nofollow">التعرّف البصري على الحروف</a>.</p>
</article></div>
