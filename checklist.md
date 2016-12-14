# Checklist 2017

1. Progressive Enhancement as the main principles
2. Break down assets in 3 groups: Core / Enhancement / Extras
3. Load Core immediately, Enhancement on DomContentLoaded, Extras on Load.
4. HTTP/2 (modular architecture/concatenate/compress) in use
5. Monitor mixed content warnings (https://report-uri.io/)
6. CDN in use (supporting HTTP2, check https://istlsfastyet.com)
7. HPACK compression in use
8. Zapfli/Brotli compression in use
9. Service Worker in use
10. Critical CSS in use / potentially Server Push in HTTP/2 world
11. Web font subsetting + loading (check https://github.com/thomaspink/js-inline-helper)
12. Responsive images / progressive JPEGs / mozJPEG, tinyPNG
13. Optimize start render for React/Angular/Ember etc.
14. Progressive Web App / AMP / PWA+AMP?
15. WebPageTest Instance running
16. Grunt/Gulp/Webpack build in place
17. Resource hints: dns-prefetch, prefetch, prerender, preload
18. Improve perceived perf. (skeleton screens, lazy-loaded fonts and expensive JavaScript, e.g. carousels, video, iframes)
19. Only animate `transform` and `opacity`
20. Check the devtools render tab for render performance (Paint flashing, fps)
21. Code is linted with tslint (https://github.com/Netural/frontend-resources/blob/master/dotfiles)
22. Use editorconfig (https://github.com/Netural/frontend-resources/blob/master/dotfiles)
23. Coding guidlines (https://github.com/Netural/frontend-resources/tree/master/code-guidelines)
24. Goal: Start Render <1s
25. Goal: SpeedIndex ±1000


Taken from: https://plus.google.com/+SmashingMagazine/posts/UxXy9bqEXyW
