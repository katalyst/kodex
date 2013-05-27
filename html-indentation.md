---
layout: default
title: HTML - Indentation
---

Nested elements MUST be indented using 2 spaces (soft tabs):

```html
<!-- GOOD -->
<div>
  <h1>Foo Bar</h1>
</div>

<!-- BAD -->
<div>
<h1>Foo Bar</h1>
</div>

<!-- BAD -->
<div>
    <h1>Foo Bar</h1>
</div>
```

Elements with multiple child nodes (including text nodes) SHOULD be written over multiple lines:

```html
<!-- GOOD -->
<hgroup>
  <h1>Foo</h1>
  <h2>Bar</h2>
</hgroup>

<!-- BAD -->
<hgroup>
  <h1>Foo</h1><h2>Bar</h2>
</hgroup>

<!-- GOOD -->
<h1>
  Foo
  <br/>
  Bar
</h1>

<!-- BAD -->
<h1>
  Foo<br/>Bar
</h1>
```

Elements with more than 1 level of descendants (including text nodes) SHOULD be written over multiple lines:

```html
<!-- GOOD -->
<a href="#">
  <span>Foo</span>
</a>

<!-- BAD -->
<a href="#"><span>Foo</span></a>
```
