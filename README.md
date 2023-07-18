I'm mainly following this topics about perfomace, that are well categorized 

Topics: [Frontend performace roadmap](https://roadmap.sh/best-practices/frontend-performance)

### Minified CSS
The goal is removes all unnecessary things to decrease the size of the files that the browser will download
##### Tools:
  - [cssnano](https://cssnano.co/) 
  - [csso](https://github.com/css/csso)

##### Contents:
  - [Minify CSS](https://web.dev/minify-css/)
  - [Optimizing Encoding and Transfer Size of Text-Based Assets](https://web.dev/optimizing-content-efficiency-optimize-encoding-and-transfer/#minification-preprocessing--context-specific-optimizations)
  - [Brotli compression](https://github.com/google/brotli)
  - [Brotli and gzip](https://tech.oyorooms.com/how-brotli-compression-gave-us-37-latency-improvement-14d41e50fee4)
---
### Non blocking files
The ideia is to load some blocking files before the browser starts rendering the page, so as not affect the Browser to show the content.

- [Link Preload](https://developer.mozilla.org/en-US/docs/Web/HTML/Attributes/rel/preload)
- [Preload: What Is It Good For?](https://www.smashingmagazine.com/2016/02/preload-what-is-it-good-for/)
- [Eliminate render-blocking resources](https://developer.chrome.com/docs/lighthouse/performance/render-blocking-resources/)

##### Preload is not only for css and js, is very powerful to images with largest contentful
- [Preload responsive images](https://web.dev/preload-responsive-images/)
---
### Fonts
Use the `woff2` a modern format, its format use brotlin to compression and have 30% average gain over the `woff1`.

###### Contents:
  - [Woff2 google explanation](https://groups.google.com/a/chromium.org/g/chromium-dev/c/j27Ou4RtvQI)
  - [Official repository of woff2 compression](https://github.com/google/woff2)
  - [Covert to woff2](https://www.fontsquirrel.com/tools/webfont-generator)
  - [ttf to woff2](https://everythingfonts.com/ttf-to-woff2)

> Make a fallback, some browsers are not yet supported https://caniuse.com/?search=woff2
