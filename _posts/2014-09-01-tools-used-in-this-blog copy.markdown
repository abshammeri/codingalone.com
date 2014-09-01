---
layout: post
title:  "مرحباً والأدوات المستخدمة في تطوير الموقع و أشياء أخرى"
date:   2014-09-01 00:00:13
categories: general
---
*مرحباً*  لأنها االتدوينة الأولى في الموقع الذي فكرت فيه تسع سنوات ونفذته في ساعتين ليس لأني Geek ولكن لأني كرهت حياتي بسبب التأجيل و الكسل 

استخدمت أدوات مفتوحة المصدر في تطوير هذا الموقع ، واعتمدت على "تصميم بسيط" ليظهر بهذا الشكل. [Jekyll][jekyll] هي الأداة التي استخدمتها في بناء هذا الموقع، وهي مبنية باستخدام Ruby وصدقني : لا أعرف Ruby كما لا أعرف كيف أكتب Jekyll بطريقة صحيحة في كل مرة. Jekyll هي أداة لتوليد ملفات html ستاتيكية ، لا يوجد قاعدة بيانات ، حيث كل البيانات مخزنة في مستودع على github ، وبالمناسبة ، موقعي [مفتوح المصدر] [github-codingalone]. أستخدم سيرفر شخصي VPS مستضاف لدى الشركة الرائعة جدا [linode][linode]، حيث نظام التشغيل Ubuntu و الويب سيرفر هو [nginx][nginx]. أستخدم [git hook][git-hook] لعمل deployment من جهازي إلى السيرفر ، سأشرح في تدوينة قادمة كيف حدث هذا. طبعا عملية تثبيت السيرفر وإعداده لأول مرة عملية متبعة لمن لا يفقه بنظام linux إلا القليل ، لكن استفدت كثيرا من [مقالات متعددة][first-5-minutes-linux-server] ترشدك للخمس الدقائق الأولى التي تحتاجها ، مثل تثبيت Fail2ban و إنشاء users و إضافة privielges. أما logs فأستخدم أداة [logwatch][logwatch] لمشاهدة ملخص يومي يصلني على بريدي الشخصي عن حالة server ، من دخل ومن خرج وماذا حدث.

##التصميم

هل أعجبك هذا الخط؟ أتمنى ذلك لأني دفعت مقابل الحصول عليه مئة ريال واسمه [Eskorte][eskorte] ، هذه النسخة تجريبية تنتهي بعد سنة ولم أقرا الرخصة بالتفصيل ، لكن سأعطيه بعض الوقت وسأرى. أما الموقع نفسه فاستخدمت نفس css/sass الافتراضي في jekyll ، مع بعض التعديلات ليتوافق مع اللغة العربية. لازال الوقت طويلا للوصول إلى تصميم مرضي.


##وش سالفة اسم النطاق

codingalone.com هو النطاق الذي حجزته منذ مدة عندما كنت " أبرمج وحيدا " كما هي العادة  في منتصف كل ليلة ، حالي حال أي مبرمج و مبرمجة ابتلي بإدمان البرمجة ،لا أعرف إن كنت سأستمر على هذا النطاق أم أحجز نطاق كلاسيكي باسمي التقليدي؟ لا أعرف.

##اهتماماتي

أهتم في تطوير تطبيقات الويب و الموبايل ، لكن قد أكتب عن أشياء مثل nginx as load balancer أو OpenGL Graphics Programming أو Paraller Processing ، بالعربي بتاع كلّه، حسب المزاج.

سأسعى لتحسين المدونة مع الوقت ، بإضافة نظام  للتعليقات ( هل سيهتم أحد ؟ )  و تحسين الشكل والأهم المضمون المفيد، إلى ذلك الحين يمكننا التواصل عبر حسابي الشخصي في [twitter][twitter].




[jekyll]:      http://jekyllrb.com
[linode]: http://linode.com
[github-codingalone]:   https://github.com/abshammeri/codingalone.com
[nginx]: http://nginx.org/
[git-hook]: http://git-scm.com/book/en/Customizing-Git-Git-Hooks
[watchlog]: http://linux.about.com/library/cmd/blcmdl8_logwatch.htm
[first-5-minutes-linux-server]: http://plusbryan.com/my-first-5-minutes-on-a-server-or-essential-security-for-linux-servers
[eskorte]: https://www.rosettatype.com/Eskorte
[twitter]: https://twitter.com/abshammeri

