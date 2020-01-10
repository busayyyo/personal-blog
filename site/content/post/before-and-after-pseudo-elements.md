---
title: Before and After Pseudo Elements
date: 2020-01-08T13:08:32.668Z
description: Some interesting use cases
---
Before now, I never really understood the exact context the `::before` and `::after` pseudo elements could be useful. It just felt like it was some fancy piece of CSS that you may never use but you should be aware of. Well, that was before I came across a few visual design styles that didn't have a traditional markup to them. It was like seeing a pretty thing without a skeleton! I inspected these pretty skeletons of course, and  lo and behold, the `::before` and `::after` pseudo elements were used!

## A little note about  ::before and ::after

The `::before` and `::after` pseudo elements, also known as `:before` and `:after` are used to style HTML elements without the need to insert non essential elements in the markup. The objective here is to have a clean semantic markup, while still getting the intended styles. You don't need to continually insert span for icons in your semantic markup for example, if it does not provide a meaning to your document structure. That's where the before and after pseudo elements come in.

At the advent of CSS3, the markup was changed from the one colon syntax i.e `:before` to the two colon syntax `::before` to distinguish between pseudo classes and pseudo elements (to understand the difference between pseudo classes and pseudo elements, check out this [article ](https://www.d.umn.edu/~lcarlson/csswork/selectors/pseudo_dif.html)). However, the browser understands both syntaxes. So either is valid. In this article however, I will be using the updated syntax i.e `::before` and `::after`.

The `::before` and `::after` can only be activated by adding the `content` property to it, otherwise it won't work. Its default `display` is `inline`, so be aware of that while styling. 

## Some Interesting Usage

**1. Quotes**

For quotes, it's as easy as using the content values `open-quote` and `close-quote`

![sample quote to markup](/img/quote.png)

```
<p>The best things are yet to come</p>p::before {content: open-quote;}p::after {content: close-quote;}
```

and voila! we have something like this: with no need to use javascript to include it for dynamic data nor manually insert it in the markup.

**2. Icons**

There are times when you need insert an icon and you don't want it showing up in the markup. You can just do it by using the ::before and ::after pseudo classes. 

**3. Titles**

Titles have really interesting usage with different visual designs out there, I've seen before and after pseudo elements used to emphasise or just style some visual elements. Here is an example.
