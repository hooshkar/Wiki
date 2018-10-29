---
title: نمایش کد در مارک داون (Markdown)  
author: محمد رضا کریمی  
description: آموزش قواعد نمایش کد در مارک داون (Markdown)  
dateModified: 2018/05/16  
datePublished: 2018/05/16  
uid: ComputerAndIt/Markdown/CodeWriting  
---

برای نمایش متن و یا بهتر است بگوییم نمایش کد، کافیست آن قطعه کد را بین دو علامت بک‌‌ تیک (`) قرار دهید.که به این نوع نمایش کد، Inline Code می‌گویند.

مثال:

```
I think you should use an
`code here` element here instead
```

خروجی:

I think you should use an
`code here` element here instead

هرچیزی که داخل دو علامت بک تیک (`) قرار دهید به همان شکا نشان داده میشوند.

اگر شما قصد نمایش یک بلاک کد را دارید کافیست در ابتدا و انتهای آن، سه علامت بک تیک (`) قرار دهید.

مثال :

````
Some basic Git commands are:
```
git status
git add
git commit
```
````

خروجی:

Some basic Git commands are:
```
git status
git add
git commit
```

شما میتوانید زبان قطعه کد  را بنویسید تا با رنگ‌های بهتری نمایش داده شود.

مثال :

````
```ruby
require 'redcarpet'
markdown = Redcarpet.new("Hello World!")
puts markdown.to_html
```
````

خروجی:

```ruby
require 'redcarpet'
markdown = Redcarpet.new("Hello World!")
puts markdown.to_html
```