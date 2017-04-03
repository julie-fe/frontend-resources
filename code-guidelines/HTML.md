# HTML

Inspired by [Codeguide](http://codeguide.co/)

## Syntax

- Use [Dotfiles](https://github.com/Netural/frontend-resources/blob/master/dotfiles/README.md)
- Nested elements should be indented once
- Always use double quotes, never single quotes, on attributes
- Don't include a trailing slash in self-closing elements—the HTML5 spec says they're optional.
- Don't omit optional closing tags (e.g. `</li>` or `</body>`)
- Use the HTML5 doctype `<!DOCTYPE html>` 

```HTML
<!DOCTYPE html>
<html>
  <head>
    <title>Page title</title>
  </head>
  <body>
    <img src="images/company-logo.png" alt="Company">
    <h1 class="hello-world">Hello, world!</h1>
  </body>
</html>
```
## Language attribute

From the [HTML5 spec](http://w3c.github.io/html/semantics.html#the-html-element)

> Authors are encouraged to specify a lang attribute on the root html element, giving the document’s language. This aids speech synthesis tools to determine what pronunciations to use, translation tools to determine what rules to use, and so forth.

Head to [Wikipedia](https://en.wikipedia.org/wiki/ISO_3166-1_alpha-2) for language codes.

```HTML
<html lang="en-us">
  <!-- ... -->
</html>
```

## IE compatibility mode

Internet Explorer supports the use of a document compatibility `<meta>` tag to specify what version of IE the page should be rendered as. Unless circumstances require otherwise, it's most useful to instruct IE to use the latest supported mode with edge mode.

For more information, read this [awesome Stack Overflow article](http://stackoverflow.com/questions/6771258/what-does-meta-http-equiv-x-ua-compatible-content-ie-edge-do).

```HTML
<meta http-equiv="X-UA-Compatible" content="IE=Edge">
```

## Character encoding

Quickly and easily ensure proper rendering of your content by declaring an explicit character encoding. When doing so, you may avoid using character entities in your HTML, provided their encoding matches that of the document (generally UTF-8).

```HTML
<head>
  <meta charset="UTF-8">
</head>
```

## CSS and JavaScript includes

Per HTML5 spec, typically there is no need to specify a `type` when including CSS and JavaScript files as `text/css` and `text/javascript` are their respective defaults.

```HTML
<!-- External CSS -->
<link rel="stylesheet" href="code-guide.css">

<!-- In-document CSS -->
<style>
  /* ... */
</style>

<!-- JavaScript -->
<script src="code-guide.js"></script>
```

### Location of includes

- Consider a above-the-fold CSS file
- *Always* include JavaScript files on the bottom of a page. 
- We try to streamline the including as good as possible in the boilerplates

## Links

- [MDN: HTML elements](https://developer.mozilla.org/en-US/docs/Web/HTML/Element): Pokedex of HTML elements
- [MDN: HTML guide](https://developer.mozilla.org/en-US/docs/Web/Guide/HTML): Guides for marking up content correctly in HTML
- [Google Developers: Forms](https://developers.google.com/web/fundamentals/design-and-ui/input/forms/label-and-name-inputs?hl=en): Create amazing forms!
