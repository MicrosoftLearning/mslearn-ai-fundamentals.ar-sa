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
  <td><div dir="rtl">تحليل الصور في مدخل Azure AI Foundry</div></td>
  </tr>
  </tbody>
</table>
</div></td>
  </tr>
  </tbody>
</table></markdown-accessiblity-table>

<div class="markdown-heading" dir="rtl"><h1 tabindex="-1" class="heading-element" dir="rtl">تحليل الصور في مدخل Azure AI Foundry</h1><a id="user-content-تحليل-الصور-في-مدخل-azure-ai-foundry" class="anchor" aria-label="Permalink: تحليل الصور في مدخل Azure AI Foundry" href="#تحليل-الصور-في-مدخل-azure-ai-foundry"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="rtl">تتضمن <strong>Azure AI Vision</strong> العديد من القدرات لفهم محتوى الصورة والسياق واستخراج المعلومات من الصور. في هذا التمرين، ستستخدم Azure AI Vision في مدخل Azure AI Foundry، وهي منصة Microsoft لإنشاء التطبيقات الذكية، لتحليل الصور باستخدام التجارب المدمجة.</p>
<p dir="rtl">افترض أن بائع التجزئة الوهمي <em>Northwind Traders</em> قرر تنفيذ "متجر ذكي"، حيث تراقب خدمات الذكاء الاصطناعي المتجر لتحديد العملاء الذين يحتاجون إلى المساعدة، وتوجيه الموظفين لمساعدتهم. باستخدام Azure AI Vision، يمكن تحليل الصور التي التقطتها الكاميرات في جميع أنحاء المتجر لتقديم أوصاف ذات مغزى لما تصوره.</p>
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
<blockquote>
<p dir="rtl"><strong>هام</strong>: ستحتاج إلى توفير موارد خدمات الذكاء الاصطناعي في Azure في موقع محدد لاستكمال بقية النشاط العملي.</p>
</blockquote>
</li>
<li>
<p dir="rtl">في نفس جزء <em>إنشاء مشروع</em>، حدد <strong>تخصيص</strong> وحدد أحد <strong>المواقع</strong> التالية: <em>شرق الولايات المتحدة، أو وسط فرنسا، أو وسط كوريا، أو غرب أوروبا، أو غرب الولايات المتحدة</em> لإكمال بقية النشاط العملي. حدد <strong>التالي</strong> ثم حدد <strong>إنشاء</strong>.</p>
</li>
<li>
<p dir="rtl">لاحظ الموارد التي تم إنشاؤها:</p>
<ul dir="rtl">
<li>خدماتالذكاء الاصطناعي في Azure</li>
<li>مركز الذكاء الاصطناعي في Azure</li>
<li>مشروع الذكاء الاصطناعي في Azure</li>
<li>حساب التخزين</li>
<li>Key Vault</li>
<li>مجموعة الموارد</li>
</ul>
</li>
<li>
<p dir="rtl">بعد إنشاء الموارد، سيتم نقلك إلى صفحة <em>نظرة عامة</em> الخاصة بمشروعك. في القائمة الموجودة على الجانب الأيسر من الشاشة، حدد <strong>خدمات الذكاء الاصطناعي</strong>.</p>
</li>
<p dir="auto"><a target="_blank" rel="noopener noreferrer" href="https://github.com/MicrosoftLearning/mslearn-ai-fundamentals/blob/main/Instructions/Labs/media/azure-ai-foundry-ai-services.png"><img src="https://github.com/MicrosoftLearning/mslearn-ai-fundamentals/blob/main/Instructions/Labs/media/azure-ai-foundry-ai-services.png" alt="لقطة شاشة للقائمة الموجودة على الجانب الأيسر من شاشة المشروع مع تحديد خدمات الذكاء الاصطناعي." style="max-width: 100%;"></a></p>
</li>
<li>
<p dir="rtl">في صفحة <em>خدمات الذكاء الاصطناعي</em>، حدد لوحة <em>الرؤية + المستند</em> لتجربة إمكانات المستندات والرؤية من الذكاء الاصطناعي في Azure</p>
</li>
<p dir="auto"><a target="_blank" rel="noopener noreferrer" href="https://github.com/MicrosoftLearning/mslearn-ai-fundamentals/blob/main/Instructions/Labs/media/vision-document-tile.png"><img src="https://github.com/MicrosoftLearning/mslearn-ai-fundamentals/blob/main/Instructions/Labs/media/vision-document-tile.png" alt="لقطة شاشة للوحة الرؤية والوثيقة المحددين في صفحة خدمات الذكاء الاصطناعي." style="max-width: 100%;"></a></p>
</li>
</ol>
<div class="markdown-heading" dir="rtl"><h2 tabindex="-1" class="heading-element" dir="rtl">إنشاء تسميات توضيحية لصورة</h2><a id="user-content-إنشاء-تسميات-توضيحية-لصورة" class="anchor" aria-label="Permalink: إنشاء تسميات توضيحية لصورة" href="#إنشاء-تسميات-توضيحية-لصورة"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="rtl">دعنا نستخدم وظيفة تسمية الصور في Azure AI Vision لتحليل الصور الملتقطة بواسطة كاميرا في متجر <em>Northwind Traders</em>. تتوفر التسميات التوضيحية للصور من خلال ميزات <strong>التسمية التوضيحية</strong> و<strong>التسميات التوضيحية الكثيفة</strong> .</p>
<ol dir="rtl">
<li>
<p dir="rtl">في صفحة <em>الرؤية + المستند</em>، مرّر لأسفل وحدد <strong>الصورة</strong> ضمن <em>عرض كل إمكانات الرؤية الأخرى</em>. ثم حدد لوحة <strong>تسمية الصورة</strong>.</p>
</li>
<p dir="auto"><a target="_blank" rel="noopener noreferrer" href="https://github.com/MicrosoftLearning/mslearn-ai-fundamentals/blob/main/Instructions/Labs/media/vision-image-captioning-tile.png"><img src="https://github.com/MicrosoftLearning/mslearn-ai-fundamentals/blob/main/Instructions/Labs/media/vision-image-captioning-tile.png" alt="لقطة شاشة للوحة تسمية الصورة في قسم الصور في صفحة &quot;الرؤية&quot; و&quot;المستندات&quot;." style="max-width: 100%;"></a></p>
</li>
<li>
<p dir="rtl">في صفحة <strong>إضافة تسميات توضيحية للصور</strong>، راجع المورد الذي تتصل به والمدرج ضمن العنوان الفرعي <strong>جرّبه</strong>. يجب ألا تضطر إلى إجراء تغييرات. (<em>ملاحظة</em>: إذا لم تقم بتخصيص موقع مورد صالح في وقت سابق أثناء إنشاء المورد، فقد يُطلب منك إنشاء مورد جديد لخدمات الذكاء الاصطناعي في Azure موجود في منطقة صالحة. ستحتاج إلى إنشاء المورد الجديد لمواصلة النشاط العملي.)</p>
</li>
<li>
<p dir="rtl">حدد <a href="https://aka.ms/mslearn-images-for-analysis" rel="nofollow"><strong>https://aka.ms/mslearn-images-for-analysis</strong></a> لتنزيل <strong>image-analysis.zip</strong>. افتح المجلد على الكمبيوتر وحدد موقع الملف المسمى <strong>store-camera-1.jpg</strong>؛ الذي يحتوي على الصورة التالية:</p>
</li>
<p dir="auto"><a target="_blank" rel="noopener noreferrer" href="https://github.com/MicrosoftLearning/mslearn-ai-fundamentals/blob/main/Instructions/Labs/media/analyze-images-vision/store-camera-1.jpg"><img src="https://github.com/MicrosoftLearning/mslearn-ai-fundamentals/blob/main/Instructions/Labs/media/analyze-images-vision/store-camera-1.jpg" alt="صورة لأحد الوالدين باستخدام كاميرا الهاتف المحمول لالتقاط صورة لطفل في متجر" style="max-width: 100%;"></a></p>
</li>
<li>
<p dir="rtl">قم بتحميل صورة <strong>store-camera-1.jpg</strong> عن طريق سحبها إلى مربع <strong>سحب الملفات وإفلاتها هنا</strong>، أو عن طريق استعراضها على نظام الملفات.</p>
</li>
<li>
<p dir="rtl">لاحظ نص التسمية التوضيحية الذي تم إنشاؤها، مرئي في لوحة <strong>السمات المكتشفة</strong> على يمين الصورة.</p>
<p dir="rtl">توفر وظيفة <strong>التسمية التوضيحية</strong> جملة إنجليزية واحدة يمكن للبشر قراءتها تصف محتوى الصورة.</p>
</li>
<li>
<p dir="rtl">بعد ذلك، استخدم الصورة نفسها لإجراء <strong>تسمية توضيحية كثيفة</strong>. عُد إلى صفحة <strong>الرؤية + المستند</strong> عن طريق تحديد سهم <em>الرجوع</em> في أعلى الصفحة. في صفحة <em>الرؤية + المستند</em>، حدد علامة التبويب <strong>الصورة</strong>، ثم حدد لوحة <strong>التسميات التوضيحية الكثيفة</strong>.</p>
<p dir="rtl">تختلف ميزة <strong>التسميات التوضيحية الكثيفة</strong> عن إمكانية <strong>التسمية التوضيحية</strong> من حيث أنها توفر العديد من التسميات التوضيحية القابلة للقراءة من قبل الإنسان للصورة، واحدة تصف محتوى الصورة والأخرى، كل منها يغطي العناصر الأساسية المكتشفة في الصورة. يتضمن كل كائن تم اكتشافه مربع إحاطة، والذي يحدد إحداثيات البكسل داخل الصورة المقترنة بالعنصر.</p>
</li>
<li>
<p dir="rtl">مرر مؤشر الماوس فوق أحد التسميات التوضيحية في قائمة السمات <strong>المكتشفة</strong> ولاحظ ما يحدث داخل الصورة.</p>
</li>
<p dir="auto"><a target="_blank" rel="noopener noreferrer" href="https://github.com/MicrosoftLearning/mslearn-ai-fundamentals/blob/main/Instructions/Labs/media/analyze-images-vision/dense-captioning.png"><img src="https://github.com/MicrosoftLearning/mslearn-ai-fundamentals/blob/main/Instructions/Labs/media/analyze-images-vision/dense-captioning.png" alt="يتم عرض الصورة والتسميات التوضيحية الخاصة بها." style="max-width: 100%;"></a></p>
<p dir="rtl">حرك مؤشر الماوس فوق التسميات التوضيحية الأخرى في القائمة، ولاحظ كيف ينتقل المربع المحيط في الصورة لتمييز جزء الصورة المستخدم لإنشاء التسمية التوضيحية.</p>
</li>
</ol>
<div class="markdown-heading" dir="rtl"><h2 tabindex="-1" class="heading-element" dir="rtl">وضع علامات على الصور</h2><a id="user-content-وضع-علامات-على-الصور" class="anchor" aria-label="Permalink: وضع علامات على الصور" href="#وضع-علامات-على-الصور"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="rtl">الميزة التالية التي ستجربها هي وظيفة <em>استخراج العلامات</em> . تستند علامات الاستخراج إلى آلاف الكائنات التي يمكن التعرف عليها، بما في ذلك الكائنات الحية والمناظر الطبيعية والإجراءات.</p>
<ol dir="rtl">
<li>
<p dir="rtl">عُد إلى صفحة <em>الرؤية + المستند</em> في Azure AI Foundry، ثم حدد علامة التبويب <strong>الصورة</strong>، ثم حدد لوحة <strong>استخراج العلامة الشائعة</strong>.</p>
</li>
<li>
<p dir="rtl">افتح المجلد الذي يحتوي على الصور التي قمت بتنزيلها وحدد موقع الملف المسمى <strong>store-image-2.jpg</strong>، والذي يبدو كما يلي:</p>
</li>
<p dir="auto"><a target="_blank" rel="noopener noreferrer" href="https://github.com/MicrosoftLearning/mslearn-ai-fundamentals/blob/main/Instructions/Labs/media/analyze-images-vision/store-camera-2.jpg"><img src="https://github.com/MicrosoftLearning/mslearn-ai-fundamentals/blob/main/Instructions/Labs/media/analyze-images-vision/store-camera-2.jpg" alt="صورة لشخص مع سلة تسوق في سوبر ماركت" style="max-width: 100%;"></a></p>
</li>
<li>
<p dir="rtl">قم بتحميل ملف <strong>store-camera-2.jpg</strong>.</p>
</li>
<li>
<p dir="rtl">راجع قائمة العلامات المستخرجة من الصورة ودرجة الثقة لكل منها في لوحة السمات المكتشفة. هنا درجة الثقة هي احتمال أن يصف نص السمة المكتشفة ما هو في الواقع في الصورة. لاحظ في قائمة العلامات أنه لا يتضمن الكائنات فقط، ولكن الإجراءات، مثل <em>التسوق</em> و<em>البيع</em> و<em>الوقوف</em>.</p>
</li>
<p dir="auto"><a target="_blank" rel="noopener noreferrer" href="https://github.com/MicrosoftLearning/mslearn-ai-fundamentals/blob/main/Instructions/Labs/media/analyze-images-vision/detect-attributes.png"><img src="https://github.com/MicrosoftLearning/mslearn-ai-fundamentals/blob/main/Instructions/Labs/media/analyze-images-vision/detect-attributes.png" alt="لقطة شاشة للوحة كشف السمات في Vision Studio مع عرض النص ودرجات الثقة بجوار الصورة الأصلية." style="max-width: 100%;"></a></p>
</li>
</ol>
<div class="markdown-heading" dir="rtl"><h2 tabindex="-1" class="heading-element" dir="rtl">كشف الكائنات</h2><a id="user-content-كشف-الكائنات" class="anchor" aria-label="Permalink: كشف الكائنات" href="#كشف-الكائنات"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="rtl">في هذه المهمة، يمكنك استخدام ميزة <strong>الكشف عن الكائنات</strong> لتحليل الصور. الكشف عن الكائنات يكتشف ويستخرج مربعات الإحاطة استناداً إلى آلاف الكائنات التي يمكن التعرف عليها والكائنات الحية.</p>
<ol dir="rtl">
<li>
<p dir="rtl">عُد إلى صفحة <em>الرؤية + المستند</em> في Azure AI Foundry، ثم حدد علامة التبويب <strong>الصورة</strong>، واختر لوحة <strong>اكتشاف الكائنات الشائعة</strong>.</p>
</li>
<li>
<p dir="rtl">افتح المجلد الذي يحتوي على الصور التي قمت بتنزيلها وحدد موقع الملف المسمى <strong>store-camera-3.jpg</strong>، والذي يبدو كما يلي:</p>
</li>
<p dir="auto"><a target="_blank" rel="noopener noreferrer" href="https://github.com/MicrosoftLearning/mslearn-ai-fundamentals/blob/main/Instructions/Labs/media/analyze-images-vision/store-camera-3.jpg"><img src="https://github.com/MicrosoftLearning/mslearn-ai-fundamentals/blob/main/Instructions/Labs/media/analyze-images-vision/store-camera-3.jpg" alt="صورة لشخص يحمل عربة تسوق" style="max-width: 100%;"></a></p>
</li>
<li>
<p dir="rtl">قم بتحميل ملف <strong>store-camera-3.jpg</strong>.</p>
</li>
<li>
<p dir="rtl">في مربع <strong>السمات المكتشفة</strong>، لاحظ قائمة الكائنات المكتشفة ودرجات الثقة الخاصة بها.</p>
</li>
<li>
<p dir="rtl">مرر مؤشر الماوس فوق الكائنات في قائمة <strong>السمات المكتشفة</strong> لتمييز مربع إحاطة العنصر في الصورة.</p>
</li>
<li>
<p dir="rtl">حرك شريط تمرير <strong>قيمة الحد</strong> حتى يتم عرض قيمة 70 إلى يمين شريط التمرير. لاحظ ما يحدث للكائنات في القائمة. يحدد شريط تمرير الحد أنه يجب عرض الكائنات المحددة بدرجة ثقة أو احتمال أكبر من الحد فقط.</p>
</li>
</ol>
<div class="markdown-heading" dir="rtl"><h2 tabindex="-1" class="heading-element" dir="rtl">تنظيف</h2><a id="user-content-تنظيف" class="anchor" aria-label="Permalink: تنظيف" href="#تنظيف"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="rtl">إذا كنت لا تنوي إجراء المزيد من التدريبات، فاحذف أي موارد لم تعد بحاجة إليها. وهذا يتجنب تكبد أي تكاليف غير ضرورية.</p>
<ol dir="rtl">
<li>افتح <a href="https://portal.azure.com" rel="nofollow">بوابة Azure</a> وحدد مجموعة الموارد التي تحتوي على الموارد التي قمت بإنشائها.</li>
<li>حدد المورد وحدد <strong>حذف</strong> ثم <strong>نعم</strong> للتأكيد. من ثم يتم حذف المورد.</li>
</ol>
<div class="markdown-heading" dir="rtl"><h2 tabindex="-1" class="heading-element" dir="rtl">معرفة المزيد</h2><a id="user-content-معرفة-المزيد" class="anchor" aria-label="Permalink: معرفة المزيد" href="#معرفة-المزيد"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="rtl">لمعرفة المزيد حول ما يمكنك القيام به بهذه الخدمة، راجع <a href="https://learn.microsoft.com/azure/ai-services/computer-vision/overview" rel="nofollow">صفحة Azure AI Vision</a>.</p>
</article></div>
