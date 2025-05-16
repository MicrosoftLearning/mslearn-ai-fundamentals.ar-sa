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
  <td><div dir="rtl">ميزة اكتشاف الوجوه في Vision Studio</div></td>
  </tr>
  </tbody>
</table>
</div></td>
  </tr>
  </tbody>
</table></markdown-accessiblity-table>

<div class="markdown-heading" dir="rtl"><h1 tabindex="-1" class="heading-element" dir="rtl">ميزة اكتشاف الوجوه في Vision Studio</h1><a id="user-content-ميزة-اكتشاف-الوجوه-في-vision-studio" class="anchor" aria-label="Permalink: ميزة اكتشاف الوجوه في Vision Studio" href="#ميزة-اكتشاف-الوجوه-في-vision-studio"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="rtl">غالبا ما تتطلب حلول الرؤية الذكاء الاصطناعي لتكون قادرة على اكتشاف الوجوه البشرية. لنفترض أن شركة البيع بالتجزئة الوهمية Northwind Traders تريد تحديد مكان تواجد العملاء في المتجر لمساعدتهم بشكل أفضل. إحدى الطرق لتحقيق ذلك هي تحديد ما إذا كان هناك أي وجوه في الصور، وإذا كان الأمر كذلك، قم بإرجاع إحداثيات المربع المحيط التي توضح موقعها.</p>
<p dir="rtl">لاختبار قدرات الكشف عن الوجه لخدمة Azure الذكاء الاصطناعي Face، ستستخدم <a href="https://portal.vision.cognitive.azure.com/" rel="nofollow">Azure Vision Studio</a>. هذا نظام أساسي قائم على واجهة المستخدم يتيح لك استكشاف ميزات Azure الذكاء الاصطناعي Vision دون الحاجة إلى كتابة أي تعليمة برمجية.</p>
<div class="markdown-heading" dir="rtl"><h2 tabindex="-1" class="heading-element" dir="rtl">إنشاء مورد <em>خدمات ذكاء اصطناعي في Azure</em></h2><a id="user-content-إنشاء-مورد-خدمات-ذكاء-اصطناعي-في-azure" class="anchor" aria-label="Permalink: إنشاء مورد خدمات ذكاء اصطناعي في Azure" href="#إنشاء-مورد-خدمات-ذكاء-اصطناعي-في-azure"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="rtl">يمكنك استخدام خدمة Azure الذكاء الاصطناعي Face مع <strong>مورد خدمات</strong> Azure الذكاء الاصطناعي متعدد الخدمات. إذا لم تكن قد قمت بذلك بالفعل، فأنشئ مورد <strong>خدمات ذكاء اصطناعي في Azure</strong> في اشتراكك في Azure.</p>
<ol dir="rtl">
<li>
<p dir="rtl">في علامة تبويب المتصفح، افتح مدخل Microsoft Azure على <a href="https://portal.azure.com?azure-portal=true" rel="nofollow">https://portal.azure.com</a>، وقم بتسجيل الدخول باستخدام حساب Microsoft المرتبط باشتراكك في Azure.</p>
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
<div class="markdown-heading" dir="rtl"><h2 tabindex="-1" class="heading-element" dir="rtl">ميزة اكتشاف الوجوه في Vision Studio</h2><a id="user-content-ميزة-اكتشاف-الوجوه-في-vision-studio-1" class="anchor" aria-label="Permalink: ميزة اكتشاف الوجوه في Vision Studio" href="#ميزة-اكتشاف-الوجوه-في-vision-studio-1"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<ol dir="rtl">
<li>
<p dir="rtl">في مستعرض ويب، انتقل إلى <strong>Vision Studio</strong> في <a href="https://portal.vision.cognitive.azure.com?azure-portal=true" rel="nofollow">https://portal.vision.cognitive.azure.com</a>.</p>
</li>
<li>
<p dir="rtl">في الصفحة المقصودة <strong>الحصول على بدء استخدام Vision</strong>، حدد <strong>علامة التبويب Face</strong> ثم حدد <strong>لوحة اكتشاف الوجوه في صورة</strong>.</p>
</li>
<li>
<p dir="rtl">ضمن العنوان الفرعي <strong>تجربة الخدمة</strong>، أقر بنهج استخدام الموارد عن طريق قراءة المربع وتحديده.</p>
</li>
<li>
<p dir="rtl">حدد كل صورة من عينات الصور ولاحظ بيانات الكشف عن الوجه التي يتم إرجاعها.</p>
</li>
<li>
<p dir="rtl">الآن دعونا نحاول مع بعض الصور الخاصة بنا. حدد <a href="https://aka.ms/mslearn-detect-faces" rel="nofollow"><strong>https://aka.ms/mslearn-detect-faces</strong></a>لتنزيل <strong>detect-faces.zip.</strong> ثم افتح المجلد على الكمبيوتر.</p>
</li>
<li>
<p dir="rtl">حدد موقع الملف المسمى <strong>store-camera-1.jpg</strong>؛ الذي يحتوي على الصورة التالية:</p>
</li>
<p dir="auto"><a target="_blank" rel="noopener noreferrer" href="https://github.com/MicrosoftLearning/mslearn-ai-fundamentals/blob/main/Instructions/Labs/media/analyze-images-vision/store-camera-1.jpg"><img src="https://github.com/MicrosoftLearning/mslearn-ai-fundamentals/blob/main/Instructions/Labs/media/analyze-images-vision/store-camera-1.jpg" alt="صورة لأشخاص في متجر." style="max-width: 100%;"></a></p>
</li>
<li>
<p dir="rtl">تحميل <strong>store-camera-1.jpg</strong> ومراجعة تفاصيل الكشف عن الوجه التي يتم إرجاعها.</p>
</li>
<li>
<p dir="rtl">حدد موقع الملف المسمى <strong>store-camera-2.jpg</strong>؛ الذي يحتوي على الصورة التالية:</p>
</li>
<p dir="auto"><a target="_blank" rel="noopener noreferrer" href="https://github.com/MicrosoftLearning/mslearn-ai-fundamentals/blob/main/Instructions/Labs/media/create-face-solutions/store-camera-2.jpg"><img src="https://github.com/MicrosoftLearning/mslearn-ai-fundamentals/blob/main/Instructions/Labs/media/create-face-solutions/store-camera-2.jpg" alt="صورة لأشخاص في متجر." style="max-width: 100%;"></a></p>
</li>
<li>
<p dir="rtl">تحميل <strong>store-camera-2.jpg</strong> ومراجعة تفاصيل الكشف عن الوجه التي يتم إرجاعها.</p>
</li>
<li>
<p dir="rtl">حدد موقع الملف المسمى <strong>store-camera-3.jpg</strong>؛ الذي يحتوي على الصورة التالية:</p>
</li>
<p dir="auto"><a target="_blank" rel="noopener noreferrer" href="https://github.com/MicrosoftLearning/mslearn-ai-fundamentals/blob/main/Instructions/Labs/media/create-face-solutions/store-camera-3.jpg"><img src="https://github.com/MicrosoftLearning/mslearn-ai-fundamentals/blob/main/Instructions/Labs/media/create-face-solutions/store-camera-3.jpg" alt="صورة لأشخاص في متجر مع نبات يحجب وجها." style="max-width: 100%;"></a></p>
</li>
<li>
<p dir="rtl">تحميل <strong>store-camera-3.jpg</strong> ومراجعة تفاصيل الكشف عن الوجه التي يتم إرجاعها. لاحظ كيف لم يكتشف Azure الذكاء الاصطناعي Face الوجه الذي تم حجبه.</p>
</li>
</ol>
<p dir="rtl">في هذا التمرين، استكشفت كيف يمكن لخدمات Azure الذكاء الاصطناعي اكتشاف الوجوه في الصور. إذا كان لديك الوقت، فلا تتردد في تجربة عينات الصور أو بعض الصور الخاصة بك.</p>
<div class="markdown-heading" dir="rtl"><h2 tabindex="-1" class="heading-element" dir="rtl">تنظيف</h2><a id="user-content-تنظيف" class="anchor" aria-label="Permalink: تنظيف" href="#تنظيف"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="rtl">إذا كنت لا تنوي إجراء المزيد من التدريبات، فاحذف أي موارد لم تعد بحاجة إليها. وهذا يتجنب تكبد أي تكاليف غير ضرورية.</p>
<ol dir="rtl">
<li>افتح <strong>مدخل Azure</strong> في <a href="https://portal.azure.com?azure-portal=true" rel="nofollow">https://portal.azure.com</a> وحدد مجموعة الموارد التي تحتوي على المورد الذي أنشأته.</li>
<li>حدد المورد وحدد <strong>حذف</strong> ثم <strong>نعم</strong> للتأكيد. من ثم يتم حذف المورد.</li>
</ol>
<div class="markdown-heading" dir="rtl"><h2 tabindex="-1" class="heading-element" dir="rtl">معرفة المزيد</h2><a id="user-content-معرفة-المزيد" class="anchor" aria-label="Permalink: معرفة المزيد" href="#معرفة-المزيد"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="rtl">للتعّرف على المزيد حول ما يمكنك فعله بهذه الخدمة، راجع <a href="https://learn.microsoft.com/azure/ai-services/computer-vision/overview-identity" rel="nofollow">صفحة خدمة Azure الذكاء الاصطناعي Face</a>.</p>
</article></div>
