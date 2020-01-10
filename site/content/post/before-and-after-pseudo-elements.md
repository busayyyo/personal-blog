---
title: Before and After Pseudo Elements
date: 2020-01-08T13:08:32.668Z
description: Some interesting use cases
---
Before now, I didn't really see the scenarios where the `::before` and `::after` pseudo elements could be useful. It just felt like it was some fancy piece of CSS that you may never use but you should be aware of. Well, that was before I came across a few visual design styles that didn't have a traditional markup to them. It was like seeing a pretty thing without a skeleton! I inspected these pretty skeletons of course, and  lo and behold, the `::before` and `::after` pseudo elements were used!

## A little note about  ::before and ::after

The `::before` and `::after` pseudo elements, also known as `:before` and `:after` are used to style HTML elements without the need to insert non essential elements in the markup. The objective here is to have a clean semantic markup, while still getting the desired styles. You don't need to continually insert span for icons in your semantic markup for example, if it does not provide a meaning to your document structure. That's where the before and after pseudo elements come in.

At the advent of CSS3, the markup was changed from the one colon syntax i.e `:before` to the two colon syntax `::before` to distinguish between pseudo classes and pseudo elements (to understand the difference between pseudo classes and pseudo elements, check out this [article ](https://www.d.umn.edu/~lcarlson/csswork/selectors/pseudo_dif.html)). However, the browser understands both syntaxes. So either is valid. In this article however, I will be using the updated syntax i.e `::before` and `::after`.

The `::before` and `::after` can only be activated by adding the `content` property to it, otherwise it won't work. Its default `display` is `inline`, so be aware of that while styling.

## Some Interesting Usage

**1. Quotes**

For quotes, it's as easy as using the content values `open-quote` and `close-quote` and voila, we have something like the pen below without the need to use javascript manipulated it or manually insert it in the markup.

<p class="codepen" data-height="265" data-theme-id="default" data-default-tab="css,result" data-user="Busayyyo" data-slug-hash="QWwQrEO" style="height: 265px; box-sizing: border-box; display: flex; align-items: center; justify-content: center; border: 2px solid; margin: 1em 0; padding: 1em;" data-pen-title="quote using before &amp;amp; after pseudo elements">
  <span>See the Pen <a href="https://codepen.io/Busayyyo/pen/QWwQrEO">
  quote using before &amp; after pseudo elements</a> by Busayo (<a href="https://codepen.io/Busayyyo">@Busayyyo</a>)
  on <a href="https://codepen.io">CodePen</a>.</span>
</p>
<script async src="https://static.codepen.io/assets/embed/ei.js"></script>



**2. Icons**

There are times when you need to insert an icon solely for aesthetics sake and you don't want it showing up in the markup. You can get it done by using the ::before and ::after pseudo elements. Here is an example of using the pseudo elements with fontawesome icons.

<p class="codepen" data-height="265" data-theme-id="default" data-default-tab="html,result" data-user="Busayyyo" data-slug-hash="NWPMxNR" style="height: 265px; box-sizing: border-box; display: flex; align-items: center; justify-content: center; border: 2px solid; margin: 1em 0; padding: 1em;" data-pen-title="::before pseudo element with fontawesome icons">
  <span>See the Pen <a href="https://codepen.io/Busayyyo/pen/NWPMxNR">
  ::before pseudo element with fontawesome icons</a> by Busayo (<a href="https://codepen.io/Busayyyo">@Busayyyo</a>)
  on <a href="https://codepen.io">CodePen</a>.</span>
</p>
<script async src="https://static.codepen.io/assets/embed/ei.js"></script>

**3. Titles**

Lots of titles are visually designed to stand out. You can style such titles without messing with the markup. Here is an example:
<p class="codepen" data-height="265" data-theme-id="default" data-default-tab="css,result" data-user="Busayyyo" data-slug-hash="gObzPzr" style="height: 265px; box-sizing: border-box; display: flex; align-items: center; justify-content: center; border: 2px solid; margin: 1em 0; padding: 1em;" data-pen-title="::before and ::after pseudo elements for title/headings">
  <span>See the Pen <a href="https://codepen.io/Busayyyo/pen/gObzPzr">
  ::before and ::after pseudo elements for title/headings</a> by Busayo (<a href="https://codepen.io/Busayyyo">@Busayyyo</a>)
  on <a href="https://codepen.io">CodePen</a>.</span>
</p>
<script async src="https://static.codepen.io/assets/embed/ei.js"></script>

There are many more scenarios where the `::before` and `::after` pseudo elements help you do some really neat tricks. The most important thing to understand is the role they serve -- helping you write clean semantic code while still being stylish.
