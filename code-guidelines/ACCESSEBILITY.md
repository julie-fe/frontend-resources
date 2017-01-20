# Accessebility guidlines

## Basic html structure

Important is the "Skip to main content" link. See http://a11yproject.com/posts/skip-nav-links/

```
<body>
  <a href="#main">Skip to main content</a>
  <nav role='navigation'>
    <ul>
      <li><a href="/">Home</a></li>
      <li><a href="/about">About</a></li>
      <li><a href="/blog">Blog</a></li>
    </ul>
  </nav>
  <main id="main" role="main">
    <!-- page specific content -->
  </main>
</body>
```

For the "skip to main content" link use following css to show it only for screenreaders

```
.visually-hidden { /*https://developer.yahoo.com/blogs/ydn/clip-hidden-content-better-accessibility-53456.html*/
    position: absolute !important;
    clip: rect(1px 1px 1px 1px); /* IE6, IE7 */
    clip: rect(1px, 1px, 1px, 1px);
    padding:0 !important;
    border:0 !important;
    height: 1px !important;
    width: 1px !important;
    overflow: hidden;
} 
body:hover .visually-hidden a, body:hover .visually-hidden input, body:hover .visually-hidden button { display: none !important; }
```

## Video transcribe services

```
<video class="span12 readable" poster="your-video-poster.jpg" controls tabindex="0" title="My Movie">
    <source  src="your-video.m4v" type='video/mp4; codecs="avc1.42E01E, mp4a.40.2"' />
    <source  src="your-video.ogg" type='application/ogg' />
    <source  src="your-video.webm" type='video/webm' />
    <track src="your-video-transcript.vtt" label="English Captions" kind="subtitles" srclang="en-us" default />
</video>
```

* http://verbalink.com/
* https://www.speechpad.com
* http://www.rev.com/transcription

## Useful resources
* http://a11yproject.com/


## Aria landmark roles

http://a11yproject.com/posts/getting-started-aria/
http://a11yproject.com/posts/aria-landmark-roles/

```<div role="application"></div>```

Role | Description | Analogous To |
| --- | --- | --- |
application | A region declared as a web application, as opposed to a web document.	  |
article | A section of a page that consists of a composition that forms an independent part of a document, page, or site.	 | ```<article>```
banner | A region that contains mostly site-oriented content, rather than page-specific content.	 | ```<header>,<div id="header">```
complementary | A supporting section of the document, designed to be complementary to the main content at a similar level in the DOM hierarchy, but remains meaningful when separated from the main content. | ```<aside>```
contentinfo | A large perceivable region that contains information about the parent document.	  |
directory | A list of references to members of a group, such as a static table of contents.	  |
document | A region containing related information that is declared as document content, as opposed to a web application. | ```<body>```
form | A landmark region that contains a collection of items and objects that, as a whole, combine to create a form. See related search | ```<form>```
log | A type of live region where new information is added in meaningful order and old information may disappear. See related marquee. Note: Elements with the role log have an implicit aria-live value of polite.	  |
main | A main content of a document. | ```<div id="content">```
navigation | A collection of navigational elements (usually links) for navigating the document or related documents. | ```<nav>```
note | A section whose content is parenthetic or ancillary to the main content of the resource.	  |
region | A large perceivable section of a web page or document, that the author feels is important enough to be included in a page summary or table of contents, for example, an area of the page containing live sporting event statistics. | ```<div>, <frame>, <section>```
search | A landmark region that contains a collection of items and objects that, as a whole, combine to create a search facility. See related form.	  |
status | A container whose content is advisory information for the user but is not important enough to justify an alert, often but not necessarily presented as a status bar. See related alert. Note: Elements with the role status have an implicit aria-live value of polite. | ```<output>```
