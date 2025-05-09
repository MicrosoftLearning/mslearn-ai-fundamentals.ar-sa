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
  <td><div dir="rtl">استخدام فهم لغة المحادثة مع Language Studio</div></td>
  </tr>
  </tbody>
</table>
</div></td>
  </tr>
  </tbody>
</table></markdown-accessiblity-table>

<div class="markdown-heading" dir="rtl"><h1 tabindex="-1" class="heading-element" dir="rtl">استخدام فهم لغة المحادثة مع Language Studio</h1><a id="user-content-استخدام-فهم-لغة-المحادثة-مع-language-studio" class="anchor" aria-label="Permalink: استخدام فهم لغة المحادثة مع Language Studio" href="#استخدام-فهم-لغة-المحادثة-مع-language-studio"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="rtl">تتزايد توقعاتنا بأن تكون أجهزة الكمبيوتر قادرة على استخدام الذكاء الصناعي لفهم الأوامر المنطوقة أو المكتوبة بلغة طبيعية. على سبيل المثال، قد ترغب في أن يتحكم نظام أتمتة المنزل في الأجهزة في منزلك باستخدام الأوامر الصوتية مثل "تشغيل الضوء" أو "تشغيل المروحة". يمكن للأجهزة التي تعمل بالطاقة الذكاء الاصطناعي فهم هذه الأوامر واتخاذ الإجراء المناسب.</p>
<p dir="rtl">في هذا التمرين، ستستخدم Language Studio لإنشاء واختبار مشروع يرسل إرشادات إلى أجهزة مثل الأضواء أو المراوح. ستستخدم قدرات خدمة فهم لغة المحادثة لتهيئة مشروعك.</p>
<div class="markdown-heading" dir="rtl"><h2 tabindex="-1" class="heading-element" dir="rtl">إنشاء مورد <em>Language</em></h2><a id="user-content-إنشاء-مورد-language" class="anchor" aria-label="Permalink: إنشاء مورد Language" href="#إنشاء-مورد-language"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="rtl">يمكنك استخدام العديد من ميزات لغة الذكاء الاصطناعي في Azure مع مورد <strong>Language</strong> أو خدمات <strong>الذكاء الاصطناعي في Azure</strong>. هناك بعض المثيلات التي يمكن فيها استخدام مورد لغة فقط. للتمرين أدناه، سنستخدم مورد <strong>لغة</strong>. إذا لم تكن قد فعلت ذلك بالفعل، بادر بإنشاء مورد <strong>Language</strong> في اشتراك Azure خاصتك.</p>
<ol dir="rtl">
<li>
<p dir="rtl">في علامة تبويب المستعرض، افتح مدخل Azure على <a href="https://portal.azure.com?azure-portal=true" rel="nofollow">https://portal.azure.com</a>، وسجل الدخول باستخدام حساب Microsoft المرتبط باشتراكك في Azure.</p>
</li>
<li>
<p dir="rtl">انقر فوق زر <strong>＋إنشاء مورد</strong> وابحث عن <em>خدمة اللغة</em>. حدد <strong>إنشاء</strong> خطة <strong>خدمة اللغة</strong>. سيتم نقلك إلى صفحة إلى <em>حدد ميزات إضافية</em>*. احتفظ بالتحديد الافتراضي وانقر فوق <strong>متابعة لإنشاء موردك</strong>.</p>
</li>
<li>
<p dir="rtl">في صفحة <strong>إنشاء لغة</strong>، يمكنك تكوينها بالإعدادات التالية:</p>
<ul dir="rtl">
<li><strong>الاشتراك</strong>: <em>اشتراك Azure الخاص بك</em>.</li>
<li><strong>مجموعة الموارد</strong>: <em>أنشئ مجموعة موارد جديدة ذات اسم فريد</em>.</li>
<li><strong>المنطقة</strong>: <em>حدد أقرب منطقة جغرافية لك. إذا كنت في شرق الولايات المتحدة، فاستخدم "شرق الولايات المتحدة 2"</em>.</li>
<li><strong>الاسم</strong>: <em>أدخل اسمًا مميزًا</em>.</li>
<li><strong>مستوى الأسعار</strong>: <em>F0 أو S المجاني إذا لم يكن F0 المجاني متوفراً</em></li>
<li><strong>من خلال تحديد هذا المربع، أقر بأنني قرأت وفهمت جميع الشروط أدناه:</strong> <em>محدد</em>.</li>
</ul>
</li>
<li>
<p dir="rtl">حدد <strong>مراجعة + إنشاء</strong> ثم <strong>إنشاء</strong> وانتظر حتى يكتمل التوزيع.</p>
</li>
</ol>
<div class="markdown-heading" dir="rtl"><h3 tabindex="-1" class="heading-element" dir="rtl">إنشاء تطبيق Conversational Language Understanding</h3><a id="user-content-إنشاء-تطبيق-conversational-language-understanding" class="anchor" aria-label="Permalink: إنشاء تطبيق Conversational Language Understanding" href="#إنشاء-تطبيق-conversational-language-understanding"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="rtl">لفهم اللغة الطبيعية باستخدام تطبيق Conversational Language Understanding، يمكنك إنشاء التطبيق، ثم إضافة الكيانات والأهداف والألفاظ لتحديد الأوامر التي تريد التطبيق.</p>
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
<p dir="rtl">في الجزء العلوي من المدخل، في قائمة <strong>Create new</strong>، حدد <strong>Conversational Language Understanding</strong>.</p>
</li>
<li>
<p dir="rtl">في مربع الحوار <strong>إنشاء مشروع</strong>، في الصفحة <strong>أدخل المعلومات الأساسية</strong>، أدخل التفاصيل التالية وانقر فوق <strong>التالي</strong>:</p>
<ul dir="rtl">
<li><strong>الاسم</strong>: <em>إنشاء اسم فريد</em></li>
<li><strong>لغة التعبيرات الأساسية</strong>: <em>الإنجليزية</em></li>
<li><strong>Enable multiple languages in project</strong>: <em>Do not select</em></li>
<li><strong>الوصف</strong>: <code>Simple home automation</code></li>
</ul>
<blockquote>
<p dir="rtl"><strong>تلميح</strong>: دون <em>اسم مشروعك</em>، وسوف تستخدمه لاحقًا.</p>
</blockquote>
</li>
<li>
<p dir="rtl">في صفحة <strong>مراجعة وإنهاء</strong>، حدد <strong>إنشاء</strong>.</p>
</li>
</ol>
<div class="markdown-heading" dir="rtl"><h3 tabindex="-1" class="heading-element" dir="rtl">إنشاء المقاصد والأقوال والكيانات</h3><a id="user-content-إنشاء-المقاصد-والأقوال-والكيانات" class="anchor" aria-label="Permalink: إنشاء المقاصد والأقوال والكيانات" href="#إنشاء-المقاصد-والأقوال-والكيانات"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="rtl">يعد <em>الهدف</em> عبارة عن إجراء تريد تنفيذه، على سبيل المثال، قد ترغب في تشغيل مصباح أو إيقاف تشغيل مروحة. في هذه الحالة، ستحدد هدفين: أحدهما لتشغيل الجهاز والآخر لإيقاف تشغيل الجهاز. لكل قصد، عليك تحديد نماذج التعبيرات التي تشير إلى <em>الأقوال</em> المستخدمة للإشارة إلى تحقيق النية.</p>
<ol dir="rtl">
<li>
<p dir="rtl">في الجزء <strong>تعريف المخطط</strong>، تأكد من تحديد <strong>الأهداف</strong> ثم انقر فوق <strong>إضافة</strong>، وأضِف هدفًا بالاسم <code>switch_on</code> (أحرف صغيرة) وحدد <strong>إضافة هدف</strong>.</p>
</li>
<p dir="auto"><a target="_blank" rel="noopener noreferrer" href="https://github.com/MicrosoftLearning/mslearn-ai-fundamentals/blob/main/Instructions/Labs/media/conversational-language-understanding/build-schema.png"><img src="https://github.com/MicrosoftLearning/mslearn-ai-fundamentals/blob/main/Instructions/Labs/media/conversational-language-understanding/build-schema.png" alt="انقر فوق إضافة ضمن الأهداف في جزء تخطيط البنية." style="max-width: 100%;"></a></p>
</li>
<p dir="auto"><a target="_blank" rel="noopener noreferrer" href="https://github.com/MicrosoftLearning/mslearn-ai-fundamentals/blob/main/Instructions/Labs/media/conversational-language-understanding/add-intent.png"><img src="https://github.com/MicrosoftLearning/mslearn-ai-fundamentals/blob/main/Instructions/Labs/media/conversational-language-understanding/add-intent.png" alt="أضف الهدف switch_on ثم حدد Add intent." style="max-width: 100%;"></a></p>
</li>
<li>
<p dir="rtl">انقر فوق الهدف <strong>switch_on</strong>. سينقلك إلى صفحة <strong>Data labeling</strong>. في القائمة المنسدلة <strong>Intent</strong>، حدد <strong>switch_on</strong>. بجانب الهدف <strong>switch_on</strong> اكتب تعبير <code>turn the light on</code>واضغط <strong>يدخل</strong> لإرسال هذا التعبير إلى القائمة.</p>
</li>
<p dir="auto"><a target="_blank" rel="noopener noreferrer" href="https://github.com/MicrosoftLearning/mslearn-ai-fundamentals/blob/main/Instructions/Labs/media/conversational-language-understanding/add-utterance-on.png"><img src="https://github.com/MicrosoftLearning/mslearn-ai-fundamentals/blob/main/Instructions/Labs/media/conversational-language-understanding/add-utterance-on.png" alt="أضف تعبيرًا إلى مجموعة التدريب عن طريق الكتابة في &quot;turn the light on&quot; ضمن Utterance." style="max-width: 100%;"></a></p>
</li>
<li>
<p dir="rtl">تحتاج خدمة Language إلى خمسة أمثلة ألفاظ مختلفة على الأقل لكل هدف لتدريب نموذج اللغة بشكل كافٍ. أضف أربعة أمثلة لفظية أخرى إلى هدف <strong>switch_on</strong>:</p>
<ul dir="rtl">
<li><code>switch on the fan</code></li>
<li><code>put the fan on</code></li>
<li><code>put the light on</code></li>
<li><code>switch on the light</code></li>
<li><code>turn the fan on</code></li>
</ul>
</li>
<li>
<p dir="rtl">في جزء <strong>Labeling entities for training</strong> على الجانب الأيمن من الشاشة، حدد <strong>Labels</strong>، ثم حدد <strong>Add entity</strong>. اكتب <code>device</code> (بأحرف صغيرة)، وحدد <strong>القائمة</strong> وحدد <strong>إضافة وحدة</strong>.</p>
</li>
<p dir="auto"><a target="_blank" rel="noopener noreferrer" href="https://github.com/MicrosoftLearning/mslearn-ai-fundamentals/blob/main/Instructions/Labs/media/conversational-language-understanding/add-entity.png"><img src="https://github.com/MicrosoftLearning/mslearn-ai-fundamentals/blob/main/Instructions/Labs/media/conversational-language-understanding/add-entity.png" alt="أضف كيانًا عن طريق تحديد Tags على Tagging entities for training panel، ثم حدد Add entity." style="max-width: 100%;"></a></p>
</li>
<p dir="auto"><a target="_blank" rel="noopener noreferrer" href="https://github.com/MicrosoftLearning/mslearn-ai-fundamentals/blob/main/Instructions/Labs/media/conversational-language-understanding/add-entity-device.png"><img src="https://github.com/MicrosoftLearning/mslearn-ai-fundamentals/blob/main/Instructions/Labs/media/conversational-language-understanding/add-entity-device.png" alt="اكتب device ضمن Entity name وحدد List، ثم حدد Add entity." style="max-width: 100%;"></a></p>
</li>
<li>
<p dir="rtl">عند نطق <em><strong>turn the fan on</strong></em> ميز الكلمة "fan". ثم في القائمة التي تظهر، في المربع <em>Search for an entity</em> حدد <strong>device</strong>.</p>
</li>
<p dir="auto"><a target="_blank" rel="noopener noreferrer" href="https://github.com/MicrosoftLearning/mslearn-ai-fundamentals/blob/main/Instructions/Labs/media/conversational-language-understanding/switch-on-entity.png"><img src="https://github.com/MicrosoftLearning/mslearn-ai-fundamentals/blob/main/Instructions/Labs/media/conversational-language-understanding/switch-on-entity.png" alt="ميّز الكلمة fan في utterance وحدد device." style="max-width: 100%;"></a></p>
</li>
<li>
<p dir="rtl">افعل الشيء نفسه مع جميع الأقوال. ضع علامة على بقية <em>fan</em> أو العبارات <em>الخفيفة</em> باستخدام كيان <strong>device</strong>. عند الانتهاء، تحقق من أن لديك الألفاظ التالية وانقر فوق <strong>Save changes</strong>:</p>
<markdown-accessiblity-table data-catalyst=""><table>
<thead>
<tr>
<th><strong>intent</strong></th>
<th><strong>utterance</strong></th>
<th><strong>كيان</strong></th>
</tr>
</thead>
<tbody>
<tr>
<td>switch_on</td>
<td>وضع المروحة في حالة التشغيل</td>
<td>الجهاز - <em>select fan</em></td>
</tr>
<tr>
<td>switch_on</td>
<td>إشعال المصباح</td>
<td>الجهاز - <em>select light</em></td>
</tr>
<tr>
<td>switch_on</td>
<td>تشغيل المصباح</td>
<td>الجهاز - <em>select light</em></td>
</tr>
<tr>
<td>switch_on</td>
<td>تشغيل المروحة</td>
<td>الجهاز - <em>select fan</em></td>
</tr>
<tr>
<td>switch_on</td>
<td>تشغيل المروحة</td>
<td>الجهاز - <em>select fan</em></td>
</tr>
<tr>
<td>switch_on</td>
<td>إضاءة المصباح</td>
<td>الجهاز - <em>select light</em></td>
</tr>
</tbody>
</table></markdown-accessiblity-table>
</li>
<p dir="auto"><a target="_blank" rel="noopener noreferrer" href="https://github.com/MicrosoftLearning/mslearn-ai-fundamentals/blob/main/Instructions/Labs/media/conversational-language-understanding/save-changes.png"><img src="https://github.com/MicrosoftLearning/mslearn-ai-fundamentals/blob/main/Instructions/Labs/media/conversational-language-understanding/save-changes.png" alt="بعد الانتهاء، حدد Save changes." style="max-width: 100%;"></a></p>
</li>
<li>
<p dir="rtl">في الجزء على اليسار، انقر فوق <strong>تعريف المخطط</strong> وتحقق من إدراج الهدف <strong>switch_on</strong> خاصتك. ثم حدد <strong>إضافة</strong> وأضف هدفًا جديداً بالاسم <code>switch_off</code> (بأحرف صغيرة).</p>
</li>
<p dir="rtl"><a target="_blank" rel="noopener noreferrer" href="https://github.com/MicrosoftLearning/mslearn-ai-fundamentals/blob/main/Instructions/Labs/media/conversational-language-understanding/add-switch-off.png"><img src="https://github.com/MicrosoftLearning/mslearn-ai-fundamentals/blob/main/Instructions/Labs/media/conversational-language-understanding/add-switch-off.png" alt="ارجع إلى شاشة Build Schema وأضف الهدف switch_off." style="max-width: 100%;"></a></p>
</li>
<li>
<p dir="rtl">حدد الهدف <strong>switch_off</strong>. سينقلك إلى صفحة <strong>Data labeling</strong>. في القائمة المنسدلة <strong>Intent</strong>، حدد <strong>switch_off</strong>. بجوار <strong>الهدف switch_off</strong>، أضف التعبير <code>turn the light off</code>.</p>
</li>
<li>
<p dir="rtl">أضف خمسة أمثلة لفظية أخرى إلى هدف <strong>switch_off</strong>.</p>
<ul dir="rtl">
<li><code>switch off the fan</code></li>
<li><code>put the fan off</code></li>
<li><code>put the light off</code></li>
<li><code>turn off the light</code></li>
<li><code>switch the fan off</code></li>
</ul>
</li>
<li>
<p dir="rtl">ضع علامة على الكلمات <em>الخفيفة</em> أو <em>fan</em> باستخدام كيان <strong>device</strong>. عند الانتهاء، تحقق من أن لديك الألفاظ التالية وانقر فوق <strong>Save changes</strong>:</p>
<markdown-accessiblity-table data-catalyst=""><table>
<thead>
<tr>
<th><strong>intent</strong></th>
<th><strong>utterance</strong></th>
<th><strong>كيان</strong></th>
</tr>
</thead>
<tbody>
<tr>
<td>switch_off</td>
<td>وضع المروحة في حالة إيقاف التشغيل</td>
<td>الجهاز - <em>select fan</em></td>
</tr>
<tr>
<td>switch_off</td>
<td>إطفاء المصباح</td>
<td>الجهاز - <em>select light</em></td>
</tr>
<tr>
<td>switch_off</td>
<td>إيقاف تشغيل المصباح</td>
<td>الجهاز - <em>select light</em></td>
</tr>
<tr>
<td>switch_off</td>
<td>إيقاف المروحة</td>
<td>الجهاز - <em>select fan</em></td>
</tr>
<tr>
<td>switch_off</td>
<td>إيقاف تشغيل المروحة</td>
<td>الجهاز - <em>select fan</em></td>
</tr>
<tr>
<td>switch_off</td>
<td>إيقاف إضاءة المصباح</td>
<td>الجهاز - <em>select light</em></td>
</tr>
</tbody>
</table></markdown-accessiblity-table>
</li>
</ol>
<div class="markdown-heading" dir="rtl"><h3 tabindex="-1" class="heading-element" dir="rtl">التدريب على النموذج</h3><a id="user-content-التدريب-على-النموذج" class="anchor" aria-label="Permalink: التدريب على النموذج" href="#التدريب-على-النموذج"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="rtl">الآن أنت مستعد لاستخدام المقاصد والكيانات التي حددتها لتدريب نموذج لغة المحادثة لتطبيقك.</p>
<ol dir="rtl">
<li>
<p dir="rtl">على الجانب الأيسر من Language Studio، حدد <strong>Training jobs</strong>، ثم حدد <strong>Start a training job</strong>. استخدم الإعدادات التالية:</p>
<ul dir="rtl">
<li><strong>Train a new model</strong>: <em>Selected and choose a model name</em></li>
<li><strong>وضع التدريب</strong>: تدريب قياسي (مجاني)</li>
<li><strong>تقسيم البيانات</strong>: <em>حدد تقسيم مجموعة الاختبارات تلقائياً من بيانات التدريب، واحتفظ بالنسب المئوية الافتراضية</em></li>
<li>انقر فوق <strong>تدريب</strong> أسفل الصفحة.</li>
</ul>
</li>
<li>
<p dir="rtl">انتظر حتى يكتمل التدريب.</p>
</li>
</ol>
<div class="markdown-heading" dir="rtl"><h3 tabindex="-1" class="heading-element" dir="rtl">نشر النموذج واختباره</h3><a id="user-content-نشر-النموذج-واختباره" class="anchor" aria-label="Permalink: نشر النموذج واختباره" href="#نشر-النموذج-واختباره"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="rtl">لاستخدام النموذج المدرَّب في تطبيق العميل، يجب عليك نشره كنقطة نهاية يمكن لتطبيقات العميل أن ترسل إليها ألفاظ جديدة؛ من خلالها سيتم توقع الأهداف والكيانات.</p>
<ol dir="rtl">
<li>
<p dir="rtl">على الجانب الأيسر من Language Studio، حدد <strong>Deploying a model</strong>.</p>
</li>
<li>
<p dir="rtl">حدد اسم نموذجك وانقر فوق <strong>Add deployment</strong>. استخدم الإعدادات التالية:</p>
<ul dir="rtl">
<li><strong>Create or select an existing deployment name</strong>: <em>حدد create a new deployment name. أضف اسم فريد</em>.</li>
<li><strong>Assign trained model to your deployment name</strong>: * حدد اسم النموذج المدرب*.</li>
<li>حدد <strong>توزيع</strong></li>
</ul>
<blockquote>
<p dir="rtl"><strong>تلميح</strong>: اكتب <em>اسم التوزيع</em> الخاص بك، الذي سوف تستخدمه لاحقًا.</p>
</blockquote>
</li>
<li>
<p dir="rtl">عندما يتم توزيع النموذج، حدد <strong>Testing deployments</strong> على الجانب الأيسر من الصفحة، ثم حدد النموذج الموزع الخاص بك ضمن <strong>Deployment name</strong>.</p>
</li>
<li>
<p dir="rtl">أدخل النص التالي، ثم حدد <strong>Run the test</strong>:</p>
<p dir="rtl"><code>switch the light on</code></p>
</li>
<p dir="auto"><a target="_blank" rel="noopener noreferrer" href="https://github.com/MicrosoftLearning/mslearn-ai-fundamentals/blob/main/Instructions/Labs/media/conversational-language-understanding/test-model.png"><img src="https://github.com/MicrosoftLearning/mslearn-ai-fundamentals/blob/main/Instructions/Labs/media/conversational-language-understanding/test-model.png" alt="اختبر النموذج الخاص بك عن طريق تحديد النموذج الموزع، ثم أدخل النص وحدد Run the test." style="max-width: 100%;"></a></p>
<p dir="rtl">راجع النتيجة التي تم إرجاعها، مع ملاحظة أنها تتضمن الهدف المتوقع (الذي يجب أن يكون <strong>switch_on</strong>) والكيان المتوقع (<strong>device</strong>) مع درجات الثقة التي تشير إلى احتمال احتساب النموذج لـ الهدف والكيان المتوقعين. تُظهر علامة التبويب JSON الثقة النسبية لكل هدف محتمل (الهدف الذي يتمتع بأعلى درجة ثقة هو الهدف المتوقع)</p>
</li>
<li>
<p dir="rtl">امسح مربع النص واختبر النموذج من خلال الألفاظ التالية ضمن <em>Enter your own text, or upload a text document</em>:</p>
<ul dir="rtl">
<li><code>turn off the fan</code></li>
<li><code>put the light on</code></li>
<li><code>put the fan off</code></li>
</ul>
</li>
</ol>
<p dir="rtl">لقد قمت الآن بتكوين مشروع لغة محادثة بنجاح، وكيانات محددة، والأهداف، والتعبيرات. لقد رأيت كيفية تدريب نموذج وتوزيعه في Language Studio. وقد جربت ذلك بكلا التعبيرين اللذين حددتهما، وبعض الكلمات التي لم تحددها صراحة ولكن النموذج كان قادرًا على تحديدها.</p>
<blockquote>
<p dir="rtl"><strong>ملاحظة</strong>: يوفر فهم لغة المحادثة الذكاء لتفسير هدف الإدخال؛ لا يقوم بأي إجراءات مثل تشغيل الضوء أو المروحة. سيحتاج المطور إلى إنشاء تطبيق يستخدم نموذج فهم لغة المحادثة لتحديد هدف المستخدم، ثم أتمتة الإجراء المناسب.</p>
</blockquote>
<div class="markdown-heading" dir="rtl"><h2 tabindex="-1" class="heading-element" dir="rtl">تنظيف</h2><a id="user-content-تنظيف" class="anchor" aria-label="Permalink: تنظيف" href="#تنظيف"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="rtl">إذا كنت لا تنوي إجراء المزيد من التدريبات، فاحذف أي موارد لم تعد بحاجة إليها. وهذا يتجنب تكبد أي تكاليف غير ضرورية.</p>
<p dir="rtl">1.افتح <a href="https://portal.azure.com" rel="nofollow">مدخل Microsoft Azure</a> وحدد مجموعة الموارد التي تحتوي على المورد الذي أنشأته. 1. حدد المورد وحدد <strong>حذف</strong> ثم <strong>نعم</strong> للتأكيد. ثم يتم حذف المورد.</p>
<div class="markdown-heading" dir="rtl"><h2 tabindex="-1" class="heading-element" dir="rtl">معرفة المزيد</h2><a id="user-content-معرفة-المزيد" class="anchor" aria-label="Permalink: معرفة المزيد" href="#معرفة-المزيد"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path d="m7.775 3.275 1.25-1.25a3.5 3.5 0 1 1 4.95 4.95l-2.5 2.5a3.5 3.5 0 0 1-4.95 0 .751.751 0 0 1 .018-1.042.751.751 0 0 1 1.042-.018 1.998 1.998 0 0 0 2.83 0l2.5-2.5a2.002 2.002 0 0 0-2.83-2.83l-1.25 1.25a.751.751 0 0 1-1.042-.018.751.751 0 0 1-.018-1.042Zm-4.69 9.64a1.998 1.998 0 0 0 2.83 0l1.25-1.25a.751.751 0 0 1 1.042.018.751.751 0 0 1 .018 1.042l-1.25 1.25a3.5 3.5 0 1 1-4.95-4.95l2.5-2.5a3.5 3.5 0 0 1 4.95 0 .751.751 0 0 1-.018 1.042.751.751 0 0 1-1.042.018 1.998 1.998 0 0 0-2.83 0l-2.5 2.5a1.998 1.998 0 0 0 0 2.83Z"></path></svg></a></div>
<p dir="rtl">لا يعرض هذا التطبيق سوى بعض إمكانات ميزة Conversational Language Understanding في خدمة Language. لمعرفة المزيد حول ما يمكنك القيام به مع هذه الخدمة، راجع <a href="https://docs.microsoft.com/azure/cognitive-services/language-service/conversational-language-understanding/overview" rel="nofollow">صفحة Conversational Language Understanding</a>.</p>
</article></div>
