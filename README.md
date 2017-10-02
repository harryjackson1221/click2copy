# Click2Copy
Basic [WordPress](https://wordpress.org/) [Shortcode](https://codex.wordpress.org/Shortcode) [Plugin](https://codex.wordpress.org/Plugins) to use [clipboard.js](https://clipboardjs.com) for copying content, such as HTML and CSS code snippets with the click of a button. 

## Screenshot
![ScreenShot](/screenshot.png?raw=true "ScreenShot")

## Prerequisites

[WordPress](https://wordpress.org/) should be installed on your website, then you can grab the latest copy from [our GitHub release page](https://github.com/harryjackson1221/click2copy/releases/)

## Browser Support

This library relies on both [Selection](https://developer.mozilla.org/en-US/docs/Web/API/Selection) and [execCommand](https://developer.mozilla.org/en-US/docs/Web/API/Document/execCommand) APIs. The first one is [supported by all browsers](http://caniuse.com/#search=selection) while the second one is supported in the following browsers.

| <img src="https://clipboardjs.com/assets/images/chrome.png" width="48px" height="48px" alt="Chrome logo"> | <img src="https://clipboardjs.com/assets/images/edge.png" width="48px" height="48px" alt="Edge logo"> | <img src="https://clipboardjs.com/assets/images/firefox.png" width="48px" height="48px" alt="Firefox logo"> | <img src="https://clipboardjs.com/assets/images/ie.png" width="48px" height="48px" alt="Internet Explorer logo"> | <img src="https://clipboardjs.com/assets/images/opera.png" width="48px" height="48px" alt="Opera logo"> | <img src="https://clipboardjs.com/assets/images/safari.png" width="48px" height="48px" alt="Safari logo"> |
|:---:|:---:|:---:|:---:|:---:|:---:|
| 42+ ✔ | 12+ ✔ | 41+ ✔ | 9+ ✔ | 29+ ✔ | 10+ ✔ |

The good news is that clipboard.js gracefully degrades if you need to support older browsers.

## Installing

Download the [latest release](https://github.com/harryjackson1221/click2copy/releases/)

Install the plugin using the [following guide](https://codex.wordpress.org/Managing_Plugins#Manual_Plugin_Installation) for installing a WordPress plugin manually.

Activate the plugin

## Usage
The shortcode can be applied in either the Page or Post Editor using the following syntax: [c2c]content[/c2c]

The options are as follows
* **id:** This identifies the code being copied, and only needs to be used if you have more than one instance on the page/post
* **pclass:** This applies a custom class to the `<pre>` HTML tag for styling purposes
* **bclass:** This applies a custom CSS class to the `<button>` HTML tag for styling purposes
* **button-text:** This allows you to set the button text

### *Example Use*
```
[c2c id="code1" pclass="pre2" bclass="btn" button-text="Copy"]
<div class="row">
<div class="col-md-9 col-xs-12 col-sm-12">
<div class="mod-blockquote">
A blockquote highlights &quot; important information, " which may or may not be an actual quote. A blockquote highlights &quot; important information, " which may or may not be an actual quote.  A blockquote highlights &quot; important information, " which may or may not be an actual quote. 
It uses distinct styling to set it apart from other content on the page
</div>
</div>
</div>
[/c2c]
```

# Built With
* [clipboard.js](https://clipboardjs.com) - The Javascript Library
* [PHP](http://php.net/) - The Language
* [WordPress](https://wp.org/) - The CMS
* [HarryJ.us](http://harryj.us/) - The Person
* [Coffee](https://en.wikipedia.org/wiki/Coffee) - The Fuel
