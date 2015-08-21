---
layout: post
title:  "تعديلاتي على شكل vim و terminal "
date:   2015-08-22 01:32:30
categories: general
---
*سأعرض* بشكل سريع الثيم الذي أستخدمه مع vim و iTerm2 مع تعديل بسيط على bash، كلها ممكن تعمل على linux أو mac ، بإستثناء طبعا iTerm2 الخاص بالماك، لكن أكيد لديك terminal آخر ممكن تجري عليه نفس التعديل.

##iTerm2 + bash

> ( يمكنك تجاهل هذه الفقرة إذا كنت لا ترغب به أو تستخدم linux).
الكثير يستخدم [iTerm2][iTerm2] كـ Terminal عوضاً عن الذي يأتي بشكل افتراضي مع OS X ، وأقترح عليك استخدامه . هذه صورة للثيم المستخدم واسمه Twilight -  بالمناسبة ، أكره هذا الفيلم - : 

![iTerm2 twilight color scheme]({{ site.url }}/assets/term2-twilight.png)


إذا أعجبك الثيم أو ترغب في الحصول على آخر أقترح أيضا أن تلقي نظرة على موقع [iTerm2-color-schemes][iTerm2-color-schemes] حيث يحتوي على ملف مضغوط بعشرات من الـ color schemes مع شرح مبسط لطريقة التثبيت.

لعلك لاحظت في الصورة السابقة عبارة "ashammari in github" مع سهم صغير. بالظبط، هنا تحتاج تعدل على bash و تحديدا الـ ``` ~/.bash_profile ``` هذا مثال على بعض التعديلات على ذلك الملف ليضيف لك header في terminal ، أخذت الفكرة من أحد ما من الانترنت  ، لا أذكر المصدر للأسف: 

```
#   Change Prompt
#   ------------------------------------------------------------
export PS1="\[\e[31;5;81m\]\u in \W\n→\[\e[39m\] "
export CLICOLOR=1
export LSCOLORS=ExFxBxDxCxegedabagacad
```

طبعا بعد التعديل تحتاج إعادة تحميل الملف أو إنشاء جلسة جديدة new session ، مثلا ```source ~/.bash_profile``` ستفي بالغرض.



##vim

هذه صورة من الثيم   [gruvbox][github-repo] ستجد ملف اسمه gruvbox.vim، حمله أو حمل غيره، ثم ضعه في المسار ``` ~/.vim/colors/``` ثم عدل على ```~/.vimrc``` بإضافة  التالي:
```
syntax enable
set background=dark
colorscheme gruvbox
```

هذه صورة لأحد الملفات أثناء تحريرها باستخدام vim/gruvbox :

![vim + gruvbox color scheme]({{ site.url }}/assets/gruvbox.png)


إن كان لديك ملاحظات، فعلى حسابي [تويتر][twitter] تجدني.



[github-repo]: https://github.com/morhetz/gruvbox
[iTerm2]: https://www.iterm2.com
[iTerm2-color-schemes]: http://iterm2colorschemes.com/
[twitter]: https://twitter.com/abshammeri



