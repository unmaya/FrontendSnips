FrontendSnips
=============

This is my collection of simple Sublime Text snippets for front-end development. Mostly for me to sync across machines using sym-links from  GitHub Repos.

It includes basic HTML, Javascript and CSS which I use often to speed up development time.
_I'm just getting started, its a work in progress!_

---

# Basic usage
Drop these into your "/packages/user/" folder to get started, they can live inside their own folder (ie. "snippets"). Just type the keywords and hit the tab key immediately after, I'm using the native tabTriggers so if you are using other addons that modify the tab key then these may not work as expected. Note that most of the snippets have preset fileds with placeholders, press the Tab key to cycle over them (or Shift + Tab to go backwards).

__analytics__

```html
<!-- Google Analytics: change UA-XXXXX-X to be your site's ID. -->
<script>
    var _gaq=[['_setAccount','${1:UA-XXXXX-X}'],['_trackPageview']];
    (function(d,t){var g=d.createElement(t),s=d.getElementsByTagName(t)[0];
    g.src=('https:'==location.protocol?'//ssl':'//www')+'.google-analytics.com/ga.js';
    s.parentNode.insertBefore(g,s)}(document,'script'));
</script>
```

__favicons__

```html
<!-- Favicon.ico placeholder -->
<link rel="shortcut icon" href="${1:img}/ink-favicon.ico">

<!-- Apple icon placeholder -->
<link rel="apple-touch-icon-precomposed" href="${2:img}/touch-icon.57.png">
<link rel="apple-touch-icon-precomposed" sizes="72x72" href="${3:img}/touch-icon.72.png">
<link rel="apple-touch-icon-precomposed" sizes="114x114" href="${4:img}/touch-icon.114.png">

<!-- Apple splash screen placeholder -->
<link rel="apple-touch-startup-image" href="${5:img}/splash.320x460.png" media="screen and (min-device-width: 200px) and (max-device-width: 320px) and (orientation:portrait)">
<link rel="apple-touch-startup-image" href="${6:img}/splash.768x1004.png" media="screen and (min-device-width: 481px) and (max-device-width: 1024px) and (orientation:portrait)">
<link rel="apple-touch-startup-image" href="${7:img}/splash.1024x748.png" media="screen and (min-device-width: 481px) and (max-device-width: 1024px) and (orientation:landscape)">
```

__boxshadow__

```css
-webkit-box-shadow: {${1:0}px 1px ${1:2}px rgba(0,0,0,.2)};
   -moz-box-shadow: {${1:0}px 1px ${1:2}px rgba(0,0,0,.2)};
        box-shadow: {${1:0}px 1px ${1:2}px rgba(0,0,0,.2)};
```

__log__

```javascript
console.log("${1:message}")
```

__retinaquery__

```css
@media (min--moz-device-pixel-ratio: 1.5),
       (-o-min-device-pixel-ratio: 3/2),
       (-webkit-min-device-pixel-ratio: 1.5),
       (min-device-pixel-ratio: 1.5),
       (min-resolution: 144dpi),
       (min-resolution: 1.5dppx) {

	${1:/* Retina rules here */}

}
```
