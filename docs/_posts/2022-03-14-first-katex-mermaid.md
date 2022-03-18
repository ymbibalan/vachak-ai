---
title: "اولین مطلب با KaTeX & Mermaid"
date: 2022-03-14T14:30:00+03:30
categories:
  - math
tags:
  - katex
  - mermaid
---

با استفاده از [لینک](https://katex.org/docs/support_table.html) میتوان تمام دستورات Katex را در داخل دو عدد $ ابتدا و انتها قرار داد و کد نوشته شده ریاضی نمایش داده می شود.

```ruby

$$f(x) = \int_{-\infty}^\infty \hat f(\xi)\,e^{2 \pi i \xi x} \,d\xi$$

```

نتیجه کد بالا برابر با زیر خواهد بود :

$$f(x) = \int_{-\infty}^\infty \hat f(\xi)\,e^{2 \pi i \xi x} \,d\xi$$

برای کشیدن دیاگرام می توانید از [mermaid](https://mermaid-js.github.io/mermaid/#/) استفاده کنید

```mermaid
graph LR
   A --> B
   A -->C
   C -->D
```
