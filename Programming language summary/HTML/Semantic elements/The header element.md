# The `header` element

## Intended usage

> [!quote]
> The `<header>` HTML element represents introductory content, typically a group of introductory or navigational aids. 
> It may contain some heading elements but also a logo, a search form, an author name, and other elements.
> 
> -- [MDN web docs' article on header element](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/header) (Retrieved on November 6th, 2023)

> [!quote]
> The `header` element represents a group of introductory or navigational aids.
> 
> -- from [HTML living standard's article on header element](https://html.spec.whatwg.org/multipage/sections.html#the-header-element) (Retrieve on November 6th, 2023)

The header element is intended to contain a heading, but other semantic elements are allowed to provide additional information.

These elements are:
- [[The time element]]
- [[The nav element]]
- [[The p element]]
- [[the hgroup element]]
- [[the address element]]
- [[the img element]]

## Usage examples

### Example 1

> [!note]
> This example was collected from [HTML living standard article on header element](https://html.spec.whatwg.org/multipage/sections.html#the-header-element) on November 6th, 2023.

A `header` element is intended to contain a heading element, but the heading does not need to be the first child.

```html
<header>
 <p>Welcome to...</p>
 <h1>Voidwars!</h1>
</header>
```

### Example 2

> [!note]
> This example was collected from [HTML living standard article on header element](https://html.spec.whatwg.org/multipage/sections.html#the-header-element) on November 6th, 2023.

As stated in [[#Intended usage]], a `header` element can contain navigational aids.

```html
<body>
 <header>
  <h1>Little Green Guys With Guns</h1>
  <nav>
   <ul>
    <li><a href="/games">Games</a>
    <li><a href="/forum">Forum</a>
    <li><a href="/download">Download</a>
   </ul>
  </nav>
  ...
```

### Example 3

> [!note]
> This example was collected from [MDN web docs' article on header element](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/header) on November 6th, 2023.

If a `header` element belongs to the `body`, it provides information about the page.

```html
<body>
  <header>
    <h1>Main Page Title</h1>
    <img src="mdn-logo-sm.png" alt="MDN logo" />
  </header>
...
```

If a `header` element belongs to an `article`, it provides information about the immediate article.

```html
<article>
  <header>
    <h2>The Planet Earth</h2>
    <p>
      Posted on Wednesday, <time datetime="2017-10-04">4 October 2017</time> by
      Jane Smith
    </p>
  </header>
  <p>
    We live on a planet that's blue and green, with so many things still unseen.
  </p>
  ...
</article>
```