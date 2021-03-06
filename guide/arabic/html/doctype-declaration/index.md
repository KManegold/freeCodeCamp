---
title: Doctype Declaration
localeTitle: Doctype Declaration
---
## Doctype Declaration

تعريف نوع مستند HTML ، المعروف أيضًا باسم `DOCTYPE` ، هو السطر الأول من الشفرة المطلوب في كل مستند HTML أو XHTML. يُعد إعلان `DOCTYPE` أحد التعليمات لمتصفح الويب حول إصدار HTML الذي تتم كتابة الصفحة به. وهذا يضمن تحليل صفحة الويب بنفس الطريقة من خلال متصفحات الويب المختلفة.

في HTML 4.01 ، يشير تعريف `DOCTYPE` إلى تعريف نوع الوثيقة (DTD). يعرف DTD البنية والعناصر القانونية لوثيقة XML. نظرًا لأن HTML 4.01 كان مستندًا إلى لغة الترميز المعيارية القياسية (SGML) ، كان من الضروري الإشارة إلى DTD في إعلان `DOCTYPE` .

بالإضافة إلى ذلك ، تطلبت doctypes الخاصة بـ HTML 4.01 إعلان إما DTD `strict` أو `transitional` أو `frameset` ، كل منها له حالة استخدام مختلفة كما هو موضح أدناه.

*   **Strict DTD** : يستخدم لصفحات الويب التي _تستبعد_ السمات والعناصر التي يتوقع W3C التخلص منها مع زيادة دعم CSS
*   **DTD الانتقالي** : يُستخدم لصفحات الويب التي _تتضمن_ سمات وعناصر يتوقع W3C التخلص منها مع زيادة دعم CSS
*   **Frameset DTD** : يستخدم لصفحات الويب ذات الإطارات

في المقابل ، فإن إعلان HTML5 `DOCTYPE` أبسط من ذلك بكثير: فهو لم يعد يتطلب إشارة إلى DTDs لأنه لم يعد يعتمد على SGML. راجع الأمثلة أدناه للمقارنة بين HTML 4.01 و HTML5 `DOCTYPE` s.

### أمثلة

بناء جملة Doctype لـ HTML5 وما بعدها:

 `
<!DOCTYPE html> 
` 

بناء جملة Doctype لـ HTML 4.01 صارم:

 `
<!DOCTYPE HTML PUBLIC "-//W3C//DTD HTML 4.01//EN" "http://www.w3.org/TR/html4/strict.dtd"> 
` 

Doctype syntax for Transitional HTML 4.01:

 `
<!DOCTYPE HTML PUBLIC "-//W3C//DTD HTML 4.01 Transitional//EN" "http://www.w3.org/TR/html4/loose.dtd"> 
` 

بناء جملة Doctype لـ frameset HTML 4.01:

 `
<!DOCTYPE HTML PUBLIC "-//W3C//DTD HTML 4.01 Frameset//EN" "http://www.w3.org/TR/html4/frameset.dtd"> 
` 

## التاريخ

خلال سنوات تكوين HTML ، لم يتم الاتفاق على معايير الويب بعد. يمكن لبائعي المتصفح إنشاء ميزات جديدة بأي طريقة يريدونها. كان هناك القليل من الاهتمام للمتصفحات المتنافسة. وكانت النتيجة أن على مطوري الويب اختيار متصفح لتطوير مواقعهم. هذا يعني أن المواقع لن يتم عرضها جيدًا في المتصفحات غير المدعومة. هذا الوضع لا يمكن أن يستمر.

كتب W3C (World Wide Web Consortium) مجموعة من معايير الويب للتعامل مع هذا الموقف. يجب أن يلتزم جميع موردي المتصفح ومطوري الويب بهذه المعايير. وهذا من شأنه ضمان أن المواقع الإلكترونية ستعرض بشكل جيد عبر المتصفحات. كانت التغييرات التي تتطلبها المعايير مختلفة تمامًا عن بعض الممارسات الحالية. فالالتزام بها يؤدي إلى كسر المواقع الحالية غير المتوافقة مع المعايير.

للتعامل مع هذه المشكلة ، بدأ البائعون في برمجة طرق العرض في المتصفحات الخاصة بهم. يحتاج مطورو الويب إلى إضافة تعريف مكون إلى أعلى مستند HTML. سيخبر تعريف doctype المتصفح الذي يستخدم وضع التقديم لهذا المستند. كانت ثلاثة أساليب عرض منفصلة متاحة بشكل عام عبر المتصفحات. **وضع المعايير الكاملة** يجعل الصفحات وفقا لمعايير W3C على شبكة الإنترنت. **يضع وضع Quirks** الصفحات بطريقة غير متوافقة مع المعايير. يقترب **وضع المعايير تقريبًا من وضع المعايير** الكاملة ، ولكنه يدعم عددًا قليلًا من المراوغات.

في العصر الحديث لـ HTML5 ، يتم تنفيذ معايير الويب بشكل كامل في جميع المتصفحات الرئيسية. يتم تطوير مواقع الويب بشكل عام بطريقة متوافقة مع المعايير. ولهذا السبب ، لا يوجد تعريف نوع HTML5 إلا لإعلام المتصفح بعرض المستند في وضع المعايير الكاملة.

## استعمال

يجب أن يكون Doctype Declaration السطر الأول من التعليمات البرمجية في مستند HTML ، بغض النظر عن التعليقات ، والتي يمكن أن تمر قبلها إذا لزم الأمر. بالنسبة إلى مستندات HTML5 الحديثة ، يجب أن يكون تعريف المقطع كما يلي:

`<!DOCTYPE html>`

#### معلومات اكثر:

على الرغم من أنه لم يعد يتم الاستخدام بشكل عام ، فهناك العديد من أنواع تعريفات الأنواع الأخرى من الإصدارات السابقة من HTML. هناك أيضًا إصدارات محددة لمستندات XML. لقراءة المزيد عن هذا ، ولرؤية أمثلة التعليمات البرمجية لكل منها ، ألق نظرة على [مقالة Wikipedia](https://en.wikipedia.org/wiki/Document_type_declaration) .

[ملاحظة من W3](https://www.w3.org/QA/Tips/Doctype)

[MDN Glossary entry](https://developer.mozilla.org/en-US/docs/Glossary/Doctype)

[W3Schools](https://www.w3schools.com/tags/tag_doctype.asp)

[شرح سريع "لوضع المرتقب" و "وضع المعايير"](https://developer.mozilla.org/en-US/docs/Quirks_Mode_and_Standards_Mode)