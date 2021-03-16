```html
<head><meta charset="utf-8" />

<title>Simulation</title>

<script src="https://cdnjs.cloudflare.com/ajax/libs/require.js/2.1.10/require.min.js"></script>
<script src="https://cdnjs.cloudflare.com/ajax/libs/jquery/2.0.3/jquery.min.js"></script>



<style type="text/css">
    /*!
*
* Twitter Bootstrap
*
*/
/*!
 * Bootstrap v3.3.7 (http://getbootstrap.com)
 * Copyright 2011-2016 Twitter, Inc.
 * Licensed under MIT (https://github.com/twbs/bootstrap/blob/master/LICENSE)
 */
/*! normalize.css v3.0.3 | MIT License | github.com/necolas/normalize.css */
html {
  font-family: sans-serif;
  -ms-text-size-adjust: 100%;
  -webkit-text-size-adjust: 100%;
}
body {
  margin: 0;
}
article,
aside,
details,
figcaption,
figure,
footer,
header,
hgroup,
main,
menu,
nav,
section,
summary {
  display: block;
}
audio,
canvas,
progress,
video {
  display: inline-block;
  vertical-align: baseline;
}
audio:not([controls]) {
  display: none;
  height: 0;
}
[hidden],
template {
  display: none;
}
a {
  background-color: transparent;
}
a:active,
a:hover {
  outline: 0;
}
abbr[title] {
  border-bottom: 1px dotted;
}
b,
strong {
  font-weight: bold;
}
dfn {
  font-style: italic;
}
h1 {
  font-size: 2em;
  margin: 0.67em 0;
}
mark {
  background: #ff0;
  color: #000;
}
small {
  font-size: 80%;
}
sub,
sup {
  font-size: 75%;
  line-height: 0;
  position: relative;
  vertical-align: baseline;
}
sup {
  top: -0.5em;
}
sub {
  bottom: -0.25em;
}
img {
  border: 0;
}
svg:not(:root) {
  overflow: hidden;
}
figure {
  margin: 1em 40px;
}
hr {
  box-sizing: content-box;
  height: 0;
}
pre {
  overflow: auto;
}
code,
kbd,
pre,
samp {
  font-family: monospace, monospace;
  font-size: 1em;
}
button,
input,
optgroup,
select,
textarea {
  color: inherit;
  font: inherit;
  margin: 0;
}
button {
  overflow: visible;
}
button,
select {
  text-transform: none;
}
button,
html input[type="button"],
input[type="reset"],
input[type="submit"] {
  -webkit-appearance: button;
  cursor: pointer;
}
button[disabled],
html input[disabled] {
  cursor: default;
}
button::-moz-focus-inner,
input::-moz-focus-inner {
  border: 0;
  padding: 0;
}
input {
  line-height: normal;
}
input[type="checkbox"],
input[type="radio"] {
  box-sizing: border-box;
  padding: 0;
}
input[type="number"]::-webkit-inner-spin-button,
input[type="number"]::-webkit-outer-spin-button {
  height: auto;
}
input[type="search"] {
  -webkit-appearance: textfield;
  box-sizing: content-box;
}
input[type="search"]::-webkit-search-cancel-button,
input[type="search"]::-webkit-search-decoration {
  -webkit-appearance: none;
}
fieldset {
  border: 1px solid #c0c0c0;
  margin: 0 2px;
  padding: 0.35em 0.625em 0.75em;
}
legend {
  border: 0;
  padding: 0;
}
textarea {
  overflow: auto;
}
optgroup {
  font-weight: bold;
}
table {
  border-collapse: collapse;
  border-spacing: 0;
}
td,
th {
  padding: 0;
}
/*! Source: https://github.com/h5bp/html5-boilerplate/blob/master/src/css/main.css */
@media print {
  *,
  *:before,
  *:after {
    background: transparent !important;
    box-shadow: none !important;
    text-shadow: none !important;
  }
  a,
  a:visited {
    text-decoration: underline;
  }
  a[href]:after {
    content: " (" attr(href) ")";
  }
  abbr[title]:after {
    content: " (" attr(title) ")";
  }
  a[href^="#"]:after,
  a[href^="javascript:"]:after {
    content: "";
  }
  pre,
  blockquote {
    border: 1px solid #999;
    page-break-inside: avoid;
  }
  thead {
    display: table-header-group;
  }
  tr,
  img {
    page-break-inside: avoid;
  }
  img {
    max-width: 100% !important;
  }
  p,
  h2,
  h3 {
    orphans: 3;
    widows: 3;
  }
  h2,
  h3 {
    page-break-after: avoid;
  }
  .navbar {
    display: none;
  }
  .btn > .caret,
  .dropup > .btn > .caret {
    border-top-color: #000 !important;
  }
  .label {
    border: 1px solid #000;
  }
  .table {
    border-collapse: collapse !important;
  }
  .table td,
  .table th {
    background-color: #fff !important;
  }
  .table-bordered th,
  .table-bordered td {
    border: 1px solid #ddd !important;
  }
}
@font-face {
  font-family: 'Glyphicons Halflings';
  src: url('../components/bootstrap/fonts/glyphicons-halflings-regular.eot');
  src: url('../components/bootstrap/fonts/glyphicons-halflings-regular.eot?#iefix') format('embedded-opentype'), url('../components/bootstrap/fonts/glyphicons-halflings-regular.woff2') format('woff2'), url('../components/bootstrap/fonts/glyphicons-halflings-regular.woff') format('woff'), url('../components/bootstrap/fonts/glyphicons-halflings-regular.ttf') format('truetype'), url('../components/bootstrap/fonts/glyphicons-halflings-regular.svg#glyphicons_halflingsregular') format('svg');
}
.glyphicon {
  position: relative;
  top: 1px;
  display: inline-block;
  font-family: 'Glyphicons Halflings';
  font-style: normal;
  font-weight: normal;
  line-height: 1;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}
.glyphicon-asterisk:before {
  content: "\002a";
}
.glyphicon-plus:before {
  content: "\002b";
}
.glyphicon-euro:before,
.glyphicon-eur:before {
  content: "\20ac";
}
.glyphicon-minus:before {
  content: "\2212";
}
.glyphicon-cloud:before {
  content: "\2601";
}
.glyphicon-envelope:before {
  content: "\2709";
}
.glyphicon-pencil:before {
  content: "\270f";
}
.glyphicon-glass:before {
  content: "\e001";
}
.glyphicon-music:before {
  content: "\e002";
}
.glyphicon-search:before {
  content: "\e003";
}
.glyphicon-heart:before {
  content: "\e005";
}
.glyphicon-star:before {
  content: "\e006";
}
.glyphicon-star-empty:before {
  content: "\e007";
}
.glyphicon-user:before {
  content: "\e008";
}
.glyphicon-film:before {
  content: "\e009";
}
.glyphicon-th-large:before {
  content: "\e010";
}
.glyphicon-th:before {
  content: "\e011";
}
.glyphicon-th-list:before {
  content: "\e012";
}
.glyphicon-ok:before {
  content: "\e013";
}
.glyphicon-remove:before {
  content: "\e014";
}
.glyphicon-zoom-in:before {
  content: "\e015";
}
.glyphicon-zoom-out:before {
  content: "\e016";
}
.glyphicon-off:before {
  content: "\e017";
}
.glyphicon-signal:before {
  content: "\e018";
}
.glyphicon-cog:before {
  content: "\e019";
}
.glyphicon-trash:before {
  content: "\e020";
}
.glyphicon-home:before {
  content: "\e021";
}
.glyphicon-file:before {
  content: "\e022";
}
.glyphicon-time:before {
  content: "\e023";
}
.glyphicon-road:before {
  content: "\e024";
}
.glyphicon-download-alt:before {
  content: "\e025";
}
.glyphicon-download:before {
  content: "\e026";
}
.glyphicon-upload:before {
  content: "\e027";
}
.glyphicon-inbox:before {
  content: "\e028";
}
.glyphicon-play-circle:before {
  content: "\e029";
}
.glyphicon-repeat:before {
  content: "\e030";
}
.glyphicon-refresh:before {
  content: "\e031";
}
.glyphicon-list-alt:before {
  content: "\e032";
}
.glyphicon-lock:before {
  content: "\e033";
}
.glyphicon-flag:before {
  content: "\e034";
}
.glyphicon-headphones:before {
  content: "\e035";
}
.glyphicon-volume-off:before {
  content: "\e036";
}
.glyphicon-volume-down:before {
  content: "\e037";
}
.glyphicon-volume-up:before {
  content: "\e038";
}
.glyphicon-qrcode:before {
  content: "\e039";
}
.glyphicon-barcode:before {
  content: "\e040";
}
.glyphicon-tag:before {
  content: "\e041";
}
.glyphicon-tags:before {
  content: "\e042";
}
.glyphicon-book:before {
  content: "\e043";
}
.glyphicon-bookmark:before {
  content: "\e044";
}
.glyphicon-print:before {
  content: "\e045";
}
.glyphicon-camera:before {
  content: "\e046";
}
.glyphicon-font:before {
  content: "\e047";
}
.glyphicon-bold:before {
  content: "\e048";
}
.glyphicon-italic:before {
  content: "\e049";
}
.glyphicon-text-height:before {
  content: "\e050";
}
.glyphicon-text-width:before {
  content: "\e051";
}
.glyphicon-align-left:before {
  content: "\e052";
}
.glyphicon-align-center:before {
  content: "\e053";
}
.glyphicon-align-right:before {
  content: "\e054";
}
.glyphicon-align-justify:before {
  content: "\e055";
}
.glyphicon-list:before {
  content: "\e056";
}
.glyphicon-indent-left:before {
  content: "\e057";
}
.glyphicon-indent-right:before {
  content: "\e058";
}
.glyphicon-facetime-video:before {
  content: "\e059";
}
.glyphicon-picture:before {
  content: "\e060";
}
.glyphicon-map-marker:before {
  content: "\e062";
}
.glyphicon-adjust:before {
  content: "\e063";
}
.glyphicon-tint:before {
  content: "\e064";
}
.glyphicon-edit:before {
  content: "\e065";
}
.glyphicon-share:before {
  content: "\e066";
}
.glyphicon-check:before {
  content: "\e067";
}
.glyphicon-move:before {
  content: "\e068";
}
.glyphicon-step-backward:before {
  content: "\e069";
}
.glyphicon-fast-backward:before {
  content: "\e070";
}
.glyphicon-backward:before {
  content: "\e071";
}
.glyphicon-play:before {
  content: "\e072";
}
.glyphicon-pause:before {
  content: "\e073";
}
.glyphicon-stop:before {
  content: "\e074";
}
.glyphicon-forward:before {
  content: "\e075";
}
.glyphicon-fast-forward:before {
  content: "\e076";
}
.glyphicon-step-forward:before {
  content: "\e077";
}
.glyphicon-eject:before {
  content: "\e078";
}
.glyphicon-chevron-left:before {
  content: "\e079";
}
.glyphicon-chevron-right:before {
  content: "\e080";
}
.glyphicon-plus-sign:before {
  content: "\e081";
}
.glyphicon-minus-sign:before {
  content: "\e082";
}
.glyphicon-remove-sign:before {
  content: "\e083";
}
.glyphicon-ok-sign:before {
  content: "\e084";
}
.glyphicon-question-sign:before {
  content: "\e085";
}
.glyphicon-info-sign:before {
  content: "\e086";
}
.glyphicon-screenshot:before {
  content: "\e087";
}
.glyphicon-remove-circle:before {
  content: "\e088";
}
.glyphicon-ok-circle:before {
  content: "\e089";
}
.glyphicon-ban-circle:before {
  content: "\e090";
}
.glyphicon-arrow-left:before {
  content: "\e091";
}
.glyphicon-arrow-right:before {
  content: "\e092";
}
.glyphicon-arrow-up:before {
  content: "\e093";
}
.glyphicon-arrow-down:before {
  content: "\e094";
}
.glyphicon-share-alt:before {
  content: "\e095";
}
.glyphicon-resize-full:before {
  content: "\e096";
}
.glyphicon-resize-small:before {
  content: "\e097";
}
.glyphicon-exclamation-sign:before {
  content: "\e101";
}
.glyphicon-gift:before {
  content: "\e102";
}
.glyphicon-leaf:before {
  content: "\e103";
}
.glyphicon-fire:before {
  content: "\e104";
}
.glyphicon-eye-open:before {
  content: "\e105";
}
.glyphicon-eye-close:before {
  content: "\e106";
}
.glyphicon-warning-sign:before {
  content: "\e107";
}
.glyphicon-plane:before {
  content: "\e108";
}
.glyphicon-calendar:before {
  content: "\e109";
}
.glyphicon-random:before {
  content: "\e110";
}
.glyphicon-comment:before {
  content: "\e111";
}
.glyphicon-magnet:before {
  content: "\e112";
}
.glyphicon-chevron-up:before {
  content: "\e113";
}
.glyphicon-chevron-down:before {
  content: "\e114";
}
.glyphicon-retweet:before {
  content: "\e115";
}
.glyphicon-shopping-cart:before {
  content: "\e116";
}
.glyphicon-folder-close:before {
  content: "\e117";
}
.glyphicon-folder-open:before {
  content: "\e118";
}
.glyphicon-resize-vertical:before {
  content: "\e119";
}
.glyphicon-resize-horizontal:before {
  content: "\e120";
}
.glyphicon-hdd:before {
  content: "\e121";
}
.glyphicon-bullhorn:before {
  content: "\e122";
}
.glyphicon-bell:before {
  content: "\e123";
}
.glyphicon-certificate:before {
  content: "\e124";
}
.glyphicon-thumbs-up:before {
  content: "\e125";
}
.glyphicon-thumbs-down:before {
  content: "\e126";
}
.glyphicon-hand-right:before {
  content: "\e127";
}
.glyphicon-hand-left:before {
  content: "\e128";
}
.glyphicon-hand-up:before {
  content: "\e129";
}
.glyphicon-hand-down:before {
  content: "\e130";
}
.glyphicon-circle-arrow-right:before {
  content: "\e131";
}
.glyphicon-circle-arrow-left:before {
  content: "\e132";
}
.glyphicon-circle-arrow-up:before {
  content: "\e133";
}
.glyphicon-circle-arrow-down:before {
  content: "\e134";
}
.glyphicon-globe:before {
  content: "\e135";
}
.glyphicon-wrench:before {
  content: "\e136";
}
.glyphicon-tasks:before {
  content: "\e137";
}
.glyphicon-filter:before {
  content: "\e138";
}
.glyphicon-briefcase:before {
  content: "\e139";
}
.glyphicon-fullscreen:before {
  content: "\e140";
}
.glyphicon-dashboard:before {
  content: "\e141";
}
.glyphicon-paperclip:before {
  content: "\e142";
}
.glyphicon-heart-empty:before {
  content: "\e143";
}
.glyphicon-link:before {
  content: "\e144";
}
.glyphicon-phone:before {
  content: "\e145";
}
.glyphicon-pushpin:before {
  content: "\e146";
}
.glyphicon-usd:before {
  content: "\e148";
}
.glyphicon-gbp:before {
  content: "\e149";
}
.glyphicon-sort:before {
  content: "\e150";
}
.glyphicon-sort-by-alphabet:before {
  content: "\e151";
}
.glyphicon-sort-by-alphabet-alt:before {
  content: "\e152";
}
.glyphicon-sort-by-order:before {
  content: "\e153";
}
.glyphicon-sort-by-order-alt:before {
  content: "\e154";
}
.glyphicon-sort-by-attributes:before {
  content: "\e155";
}
.glyphicon-sort-by-attributes-alt:before {
  content: "\e156";
}
.glyphicon-unchecked:before {
  content: "\e157";
}
.glyphicon-expand:before {
  content: "\e158";
}
.glyphicon-collapse-down:before {
  content: "\e159";
}
.glyphicon-collapse-up:before {
  content: "\e160";
}
.glyphicon-log-in:before {
  content: "\e161";
}
.glyphicon-flash:before {
  content: "\e162";
}
.glyphicon-log-out:before {
  content: "\e163";
}
.glyphicon-new-window:before {
  content: "\e164";
}
.glyphicon-record:before {
  content: "\e165";
}
.glyphicon-save:before {
  content: "\e166";
}
.glyphicon-open:before {
  content: "\e167";
}
.glyphicon-saved:before {
  content: "\e168";
}
.glyphicon-import:before {
  content: "\e169";
}
.glyphicon-export:before {
  content: "\e170";
}
.glyphicon-send:before {
  content: "\e171";
}
.glyphicon-floppy-disk:before {
  content: "\e172";
}
.glyphicon-floppy-saved:before {
  content: "\e173";
}
.glyphicon-floppy-remove:before {
  content: "\e174";
}
.glyphicon-floppy-save:before {
  content: "\e175";
}
.glyphicon-floppy-open:before {
  content: "\e176";
}
.glyphicon-credit-card:before {
  content: "\e177";
}
.glyphicon-transfer:before {
  content: "\e178";
}
.glyphicon-cutlery:before {
  content: "\e179";
}
.glyphicon-header:before {
  content: "\e180";
}
.glyphicon-compressed:before {
  content: "\e181";
}
.glyphicon-earphone:before {
  content: "\e182";
}
.glyphicon-phone-alt:before {
  content: "\e183";
}
.glyphicon-tower:before {
  content: "\e184";
}
.glyphicon-stats:before {
  content: "\e185";
}
.glyphicon-sd-video:before {
  content: "\e186";
}
.glyphicon-hd-video:before {
  content: "\e187";
}
.glyphicon-subtitles:before {
  content: "\e188";
}
.glyphicon-sound-stereo:before {
  content: "\e189";
}
.glyphicon-sound-dolby:before {
  content: "\e190";
}
.glyphicon-sound-5-1:before {
  content: "\e191";
}
.glyphicon-sound-6-1:before {
  content: "\e192";
}
.glyphicon-sound-7-1:before {
  content: "\e193";
}
.glyphicon-copyright-mark:before {
  content: "\e194";
}
.glyphicon-registration-mark:before {
  content: "\e195";
}
.glyphicon-cloud-download:before {
  content: "\e197";
}
.glyphicon-cloud-upload:before {
  content: "\e198";
}
.glyphicon-tree-conifer:before {
  content: "\e199";
}
.glyphicon-tree-deciduous:before {
  content: "\e200";
}
.glyphicon-cd:before {
  content: "\e201";
}
.glyphicon-save-file:before {
  content: "\e202";
}
.glyphicon-open-file:before {
  content: "\e203";
}
.glyphicon-level-up:before {
  content: "\e204";
}
.glyphicon-copy:before {
  content: "\e205";
}
.glyphicon-paste:before {
  content: "\e206";
}
.glyphicon-alert:before {
  content: "\e209";
}
.glyphicon-equalizer:before {
  content: "\e210";
}
.glyphicon-king:before {
  content: "\e211";
}
.glyphicon-queen:before {
  content: "\e212";
}
.glyphicon-pawn:before {
  content: "\e213";
}
.glyphicon-bishop:before {
  content: "\e214";
}
.glyphicon-knight:before {
  content: "\e215";
}
.glyphicon-baby-formula:before {
  content: "\e216";
}
.glyphicon-tent:before {
  content: "\26fa";
}
.glyphicon-blackboard:before {
  content: "\e218";
}
.glyphicon-bed:before {
  content: "\e219";
}
.glyphicon-apple:before {
  content: "\f8ff";
}
.glyphicon-erase:before {
  content: "\e221";
}
.glyphicon-hourglass:before {
  content: "\231b";
}
.glyphicon-lamp:before {
  content: "\e223";
}
.glyphicon-duplicate:before {
  content: "\e224";
}
.glyphicon-piggy-bank:before {
  content: "\e225";
}
.glyphicon-scissors:before {
  content: "\e226";
}
.glyphicon-bitcoin:before {
  content: "\e227";
}
.glyphicon-btc:before {
  content: "\e227";
}
.glyphicon-xbt:before {
  content: "\e227";
}
.glyphicon-yen:before {
  content: "\00a5";
}
.glyphicon-jpy:before {
  content: "\00a5";
}
.glyphicon-ruble:before {
  content: "\20bd";
}
.glyphicon-rub:before {
  content: "\20bd";
}
.glyphicon-scale:before {
  content: "\e230";
}
.glyphicon-ice-lolly:before {
  content: "\e231";
}
.glyphicon-ice-lolly-tasted:before {
  content: "\e232";
}
.glyphicon-education:before {
  content: "\e233";
}
.glyphicon-option-horizontal:before {
  content: "\e234";
}
.glyphicon-option-vertical:before {
  content: "\e235";
}
.glyphicon-menu-hamburger:before {
  content: "\e236";
}
.glyphicon-modal-window:before {
  content: "\e237";
}
.glyphicon-oil:before {
  content: "\e238";
}
.glyphicon-grain:before {
  content: "\e239";
}
.glyphicon-sunglasses:before {
  content: "\e240";
}
.glyphicon-text-size:before {
  content: "\e241";
}
.glyphicon-text-color:before {
  content: "\e242";
}
.glyphicon-text-background:before {
  content: "\e243";
}
.glyphicon-object-align-top:before {
  content: "\e244";
}
.glyphicon-object-align-bottom:before {
  content: "\e245";
}
.glyphicon-object-align-horizontal:before {
  content: "\e246";
}
.glyphicon-object-align-left:before {
  content: "\e247";
}
.glyphicon-object-align-vertical:before {
  content: "\e248";
}
.glyphicon-object-align-right:before {
  content: "\e249";
}
.glyphicon-triangle-right:before {
  content: "\e250";
}
.glyphicon-triangle-left:before {
  content: "\e251";
}
.glyphicon-triangle-bottom:before {
  content: "\e252";
}
.glyphicon-triangle-top:before {
  content: "\e253";
}
.glyphicon-console:before {
  content: "\e254";
}
.glyphicon-superscript:before {
  content: "\e255";
}
.glyphicon-subscript:before {
  content: "\e256";
}
.glyphicon-menu-left:before {
  content: "\e257";
}
.glyphicon-menu-right:before {
  content: "\e258";
}
.glyphicon-menu-down:before {
  content: "\e259";
}
.glyphicon-menu-up:before {
  content: "\e260";
}
* {
  -webkit-box-sizing: border-box;
  -moz-box-sizing: border-box;
  box-sizing: border-box;
}
*:before,
*:after {
  -webkit-box-sizing: border-box;
  -moz-box-sizing: border-box;
  box-sizing: border-box;
}
html {
  font-size: 10px;
  -webkit-tap-highlight-color: rgba(0, 0, 0, 0);
}
body {
  font-family: "Helvetica Neue", Helvetica, Arial, sans-serif;
  font-size: 13px;
  line-height: 1.42857143;
  color: #000;
  background-color: #fff;
}
input,
button,
select,
textarea {
  font-family: inherit;
  font-size: inherit;
  line-height: inherit;
}
a {
  color: #337ab7;
  text-decoration: none;
}
a:hover,
a:focus {
  color: #23527c;
  text-decoration: underline;
}
a:focus {
  outline: 5px auto -webkit-focus-ring-color;
  outline-offset: -2px;
}
figure {
  margin: 0;
}
img {
  vertical-align: middle;
}
.img-responsive,
.thumbnail > img,
.thumbnail a > img,
.carousel-inner > .item > img,
.carousel-inner > .item > a > img {
  display: block;
  max-width: 100%;
  height: auto;
}
.img-rounded {
  border-radius: 3px;
}
.img-thumbnail {
  padding: 4px;
  line-height: 1.42857143;
  background-color: #fff;
  border: 1px solid #ddd;
  border-radius: 2px;
  -webkit-transition: all 0.2s ease-in-out;
  -o-transition: all 0.2s ease-in-out;
  transition: all 0.2s ease-in-out;
  display: inline-block;
  max-width: 100%;
  height: auto;
}
.img-circle {
  border-radius: 50%;
}
hr {
  margin-top: 18px;
  margin-bottom: 18px;
  border: 0;
  border-top: 1px solid #eeeeee;
}
.sr-only {
  position: absolute;
  width: 1px;
  height: 1px;
  margin: -1px;
  padding: 0;
  overflow: hidden;
  clip: rect(0, 0, 0, 0);
  border: 0;
}
.sr-only-focusable:active,
.sr-only-focusable:focus {
  position: static;
  width: auto;
  height: auto;
  margin: 0;
  overflow: visible;
  clip: auto;
}
[role="button"] {
  cursor: pointer;
}
h1,
h2,
h3,
h4,
h5,
h6,
.h1,
.h2,
.h3,
.h4,
.h5,
.h6 {
  font-family: inherit;
  font-weight: 500;
  line-height: 1.1;
  color: inherit;
}
h1 small,
h2 small,
h3 small,
h4 small,
h5 small,
h6 small,
.h1 small,
.h2 small,
.h3 small,
.h4 small,
.h5 small,
.h6 small,
h1 .small,
h2 .small,
h3 .small,
h4 .small,
h5 .small,
h6 .small,
.h1 .small,
.h2 .small,
.h3 .small,
.h4 .small,
.h5 .small,
.h6 .small {
  font-weight: normal;
  line-height: 1;
  color: #777777;
}
h1,
.h1,
h2,
.h2,
h3,
.h3 {
  margin-top: 18px;
  margin-bottom: 9px;
}
h1 small,
.h1 small,
h2 small,
.h2 small,
h3 small,
.h3 small,
h1 .small,
.h1 .small,
h2 .small,
.h2 .small,
h3 .small,
.h3 .small {
  font-size: 65%;
}
h4,
.h4,
h5,
.h5,
h6,
.h6 {
  margin-top: 9px;
  margin-bottom: 9px;
}
h4 small,
.h4 small,
h5 small,
.h5 small,
h6 small,
.h6 small,
h4 .small,
.h4 .small,
h5 .small,
.h5 .small,
h6 .small,
.h6 .small {
  font-size: 75%;
}
h1,
.h1 {
  font-size: 33px;
}
h2,
.h2 {
  font-size: 27px;
}
h3,
.h3 {
  font-size: 23px;
}
h4,
.h4 {
  font-size: 17px;
}
h5,
.h5 {
  font-size: 13px;
}
h6,
.h6 {
  font-size: 12px;
}
p {
  margin: 0 0 9px;
}
.lead {
  margin-bottom: 18px;
  font-size: 14px;
  font-weight: 300;
  line-height: 1.4;
}
@media (min-width: 768px) {
  .lead {
    font-size: 19.5px;
  }
}
small,
.small {
  font-size: 92%;
}
mark,
.mark {
  background-color: #fcf8e3;
  padding: .2em;
}
.text-left {
  text-align: left;
}
.text-right {
  text-align: right;
}
.text-center {
  text-align: center;
}
.text-justify {
  text-align: justify;
}
.text-nowrap {
  white-space: nowrap;
}
.text-lowercase {
  text-transform: lowercase;
}
.text-uppercase {
  text-transform: uppercase;
}
.text-capitalize {
  text-transform: capitalize;
}
.text-muted {
  color: #777777;
}
.text-primary {
  color: #337ab7;
}
a.text-primary:hover,
a.text-primary:focus {
  color: #286090;
}
.text-success {
  color: #3c763d;
}
a.text-success:hover,
a.text-success:focus {
  color: #2b542c;
}
.text-info {
  color: #31708f;
}
a.text-info:hover,
a.text-info:focus {
  color: #245269;
}
.text-warning {
  color: #8a6d3b;
}
a.text-warning:hover,
a.text-warning:focus {
  color: #66512c;
}
.text-danger {
  color: #a94442;
}
a.text-danger:hover,
a.text-danger:focus {
  color: #843534;
}
.bg-primary {
  color: #fff;
  background-color: #337ab7;
}
a.bg-primary:hover,
a.bg-primary:focus {
  background-color: #286090;
}
.bg-success {
  background-color: #dff0d8;
}
a.bg-success:hover,
a.bg-success:focus {
  background-color: #c1e2b3;
}
.bg-info {
  background-color: #d9edf7;
}
a.bg-info:hover,
a.bg-info:focus {
  background-color: #afd9ee;
}
.bg-warning {
  background-color: #fcf8e3;
}
a.bg-warning:hover,
a.bg-warning:focus {
  background-color: #f7ecb5;
}
.bg-danger {
  background-color: #f2dede;
}
a.bg-danger:hover,
a.bg-danger:focus {
  background-color: #e4b9b9;
}
.page-header {
  padding-bottom: 8px;
  margin: 36px 0 18px;
  border-bottom: 1px solid #eeeeee;
}
ul,
ol {
  margin-top: 0;
  margin-bottom: 9px;
}
ul ul,
ol ul,
ul ol,
ol ol {
  margin-bottom: 0;
}
.list-unstyled {
  padding-left: 0;
  list-style: none;
}
.list-inline {
  padding-left: 0;
  list-style: none;
  margin-left: -5px;
}
.list-inline > li {
  display: inline-block;
  padding-left: 5px;
  padding-right: 5px;
}
dl {
  margin-top: 0;
  margin-bottom: 18px;
}
dt,
dd {
  line-height: 1.42857143;
}
dt {
  font-weight: bold;
}
dd {
  margin-left: 0;
}
@media (min-width: 541px) {
  .dl-horizontal dt {
    float: left;
    width: 160px;
    clear: left;
    text-align: right;
    overflow: hidden;
    text-overflow: ellipsis;
    white-space: nowrap;
  }
  .dl-horizontal dd {
    margin-left: 180px;
  }
}
abbr[title],
abbr[data-original-title] {
  cursor: help;
  border-bottom: 1px dotted #777777;
}
.initialism {
  font-size: 90%;
  text-transform: uppercase;
}
blockquote {
  padding: 9px 18px;
  margin: 0 0 18px;
  font-size: inherit;
  border-left: 5px solid #eeeeee;
}
blockquote p:last-child,
blockquote ul:last-child,
blockquote ol:last-child {
  margin-bottom: 0;
}
blockquote footer,
blockquote small,
blockquote .small {
  display: block;
  font-size: 80%;
  line-height: 1.42857143;
  color: #777777;
}
blockquote footer:before,
blockquote small:before,
blockquote .small:before {
  content: '\2014 \00A0';
}
.blockquote-reverse,
blockquote.pull-right {
  padding-right: 15px;
  padding-left: 0;
  border-right: 5px solid #eeeeee;
  border-left: 0;
  text-align: right;
}
.blockquote-reverse footer:before,
blockquote.pull-right footer:before,
.blockquote-reverse small:before,
blockquote.pull-right small:before,
.blockquote-reverse .small:before,
blockquote.pull-right .small:before {
  content: '';
}
.blockquote-reverse footer:after,
blockquote.pull-right footer:after,
.blockquote-reverse small:after,
blockquote.pull-right small:after,
.blockquote-reverse .small:after,
blockquote.pull-right .small:after {
  content: '\00A0 \2014';
}
address {
  margin-bottom: 18px;
  font-style: normal;
  line-height: 1.42857143;
}
code,
kbd,
pre,
samp {
  font-family: monospace;
}
code {
  padding: 2px 4px;
  font-size: 90%;
  color: #c7254e;
  background-color: #f9f2f4;
  border-radius: 2px;
}
kbd {
  padding: 2px 4px;
  font-size: 90%;
  color: #888;
  background-color: transparent;
  border-radius: 1px;
  box-shadow: inset 0 -1px 0 rgba(0, 0, 0, 0.25);
}
kbd kbd {
  padding: 0;
  font-size: 100%;
  font-weight: bold;
  box-shadow: none;
}
pre {
  display: block;
  padding: 8.5px;
  margin: 0 0 9px;
  font-size: 12px;
  line-height: 1.42857143;
  word-break: break-all;
  word-wrap: break-word;
  color: #333333;
  background-color: #f5f5f5;
  border: 1px solid #ccc;
  border-radius: 2px;
}
pre code {
  padding: 0;
  font-size: inherit;
  color: inherit;
  white-space: pre-wrap;
  background-color: transparent;
  border-radius: 0;
}
.pre-scrollable {
  max-height: 340px;
  overflow-y: scroll;
}
.container {
  margin-right: auto;
  margin-left: auto;
  padding-left: 0px;
  padding-right: 0px;
}
@media (min-width: 768px) {
  .container {
    width: 768px;
  }
}
@media (min-width: 992px) {
  .container {
    width: 940px;
  }
}
@media (min-width: 1200px) {
  .container {
    width: 1140px;
  }
}
.container-fluid {
  margin-right: auto;
  margin-left: auto;
  padding-left: 0px;
  padding-right: 0px;
}
.row {
  margin-left: 0px;
  margin-right: 0px;
}
.col-xs-1, .col-sm-1, .col-md-1, .col-lg-1, .col-xs-2, .col-sm-2, .col-md-2, .col-lg-2, .col-xs-3, .col-sm-3, .col-md-3, .col-lg-3, .col-xs-4, .col-sm-4, .col-md-4, .col-lg-4, .col-xs-5, .col-sm-5, .col-md-5, .col-lg-5, .col-xs-6, .col-sm-6, .col-md-6, .col-lg-6, .col-xs-7, .col-sm-7, .col-md-7, .col-lg-7, .col-xs-8, .col-sm-8, .col-md-8, .col-lg-8, .col-xs-9, .col-sm-9, .col-md-9, .col-lg-9, .col-xs-10, .col-sm-10, .col-md-10, .col-lg-10, .col-xs-11, .col-sm-11, .col-md-11, .col-lg-11, .col-xs-12, .col-sm-12, .col-md-12, .col-lg-12 {
  position: relative;
  min-height: 1px;
  padding-left: 0px;
  padding-right: 0px;
}
.col-xs-1, .col-xs-2, .col-xs-3, .col-xs-4, .col-xs-5, .col-xs-6, .col-xs-7, .col-xs-8, .col-xs-9, .col-xs-10, .col-xs-11, .col-xs-12 {
  float: left;
}
.col-xs-12 {
  width: 100%;
}
.col-xs-11 {
  width: 91.66666667%;
}
.col-xs-10 {
  width: 83.33333333%;
}
.col-xs-9 {
  width: 75%;
}
.col-xs-8 {
  width: 66.66666667%;
}
.col-xs-7 {
  width: 58.33333333%;
}
.col-xs-6 {
  width: 50%;
}
.col-xs-5 {
  width: 41.66666667%;
}
.col-xs-4 {
  width: 33.33333333%;
}
.col-xs-3 {
  width: 25%;
}
.col-xs-2 {
  width: 16.66666667%;
}
.col-xs-1 {
  width: 8.33333333%;
}
.col-xs-pull-12 {
  right: 100%;
}
.col-xs-pull-11 {
  right: 91.66666667%;
}
.col-xs-pull-10 {
  right: 83.33333333%;
}
.col-xs-pull-9 {
  right: 75%;
}
.col-xs-pull-8 {
  right: 66.66666667%;
}
.col-xs-pull-7 {
  right: 58.33333333%;
}
.col-xs-pull-6 {
  right: 50%;
}
.col-xs-pull-5 {
  right: 41.66666667%;
}
.col-xs-pull-4 {
  right: 33.33333333%;
}
.col-xs-pull-3 {
  right: 25%;
}
.col-xs-pull-2 {
  right: 16.66666667%;
}
.col-xs-pull-1 {
  right: 8.33333333%;
}
.col-xs-pull-0 {
  right: auto;
}
.col-xs-push-12 {
  left: 100%;
}
.col-xs-push-11 {
  left: 91.66666667%;
}
.col-xs-push-10 {
  left: 83.33333333%;
}
.col-xs-push-9 {
  left: 75%;
}
.col-xs-push-8 {
  left: 66.66666667%;
}
.col-xs-push-7 {
  left: 58.33333333%;
}
.col-xs-push-6 {
  left: 50%;
}
.col-xs-push-5 {
  left: 41.66666667%;
}
.col-xs-push-4 {
  left: 33.33333333%;
}
.col-xs-push-3 {
  left: 25%;
}
.col-xs-push-2 {
  left: 16.66666667%;
}
.col-xs-push-1 {
  left: 8.33333333%;
}
.col-xs-push-0 {
  left: auto;
}
.col-xs-offset-12 {
  margin-left: 100%;
}
.col-xs-offset-11 {
  margin-left: 91.66666667%;
}
.col-xs-offset-10 {
  margin-left: 83.33333333%;
}
.col-xs-offset-9 {
  margin-left: 75%;
}
.col-xs-offset-8 {
  margin-left: 66.66666667%;
}
.col-xs-offset-7 {
  margin-left: 58.33333333%;
}
.col-xs-offset-6 {
  margin-left: 50%;
}
.col-xs-offset-5 {
  margin-left: 41.66666667%;
}
.col-xs-offset-4 {
  margin-left: 33.33333333%;
}
.col-xs-offset-3 {
  margin-left: 25%;
}
.col-xs-offset-2 {
  margin-left: 16.66666667%;
}
.col-xs-offset-1 {
  margin-left: 8.33333333%;
}
.col-xs-offset-0 {
  margin-left: 0%;
}
@media (min-width: 768px) {
  .col-sm-1, .col-sm-2, .col-sm-3, .col-sm-4, .col-sm-5, .col-sm-6, .col-sm-7, .col-sm-8, .col-sm-9, .col-sm-10, .col-sm-11, .col-sm-12 {
    float: left;
  }
  .col-sm-12 {
    width: 100%;
  }
  .col-sm-11 {
    width: 91.66666667%;
  }
  .col-sm-10 {
    width: 83.33333333%;
  }
  .col-sm-9 {
    width: 75%;
  }
  .col-sm-8 {
    width: 66.66666667%;
  }
  .col-sm-7 {
    width: 58.33333333%;
  }
  .col-sm-6 {
    width: 50%;
  }
  .col-sm-5 {
    width: 41.66666667%;
  }
  .col-sm-4 {
    width: 33.33333333%;
  }
  .col-sm-3 {
    width: 25%;
  }
  .col-sm-2 {
    width: 16.66666667%;
  }
  .col-sm-1 {
    width: 8.33333333%;
  }
  .col-sm-pull-12 {
    right: 100%;
  }
  .col-sm-pull-11 {
    right: 91.66666667%;
  }
  .col-sm-pull-10 {
    right: 83.33333333%;
  }
  .col-sm-pull-9 {
    right: 75%;
  }
  .col-sm-pull-8 {
    right: 66.66666667%;
  }
  .col-sm-pull-7 {
    right: 58.33333333%;
  }
  .col-sm-pull-6 {
    right: 50%;
  }
  .col-sm-pull-5 {
    right: 41.66666667%;
  }
  .col-sm-pull-4 {
    right: 33.33333333%;
  }
  .col-sm-pull-3 {
    right: 25%;
  }
  .col-sm-pull-2 {
    right: 16.66666667%;
  }
  .col-sm-pull-1 {
    right: 8.33333333%;
  }
  .col-sm-pull-0 {
    right: auto;
  }
  .col-sm-push-12 {
    left: 100%;
  }
  .col-sm-push-11 {
    left: 91.66666667%;
  }
  .col-sm-push-10 {
    left: 83.33333333%;
  }
  .col-sm-push-9 {
    left: 75%;
  }
  .col-sm-push-8 {
    left: 66.66666667%;
  }
  .col-sm-push-7 {
    left: 58.33333333%;
  }
  .col-sm-push-6 {
    left: 50%;
  }
  .col-sm-push-5 {
    left: 41.66666667%;
  }
  .col-sm-push-4 {
    left: 33.33333333%;
  }
  .col-sm-push-3 {
    left: 25%;
  }
  .col-sm-push-2 {
    left: 16.66666667%;
  }
  .col-sm-push-1 {
    left: 8.33333333%;
  }
  .col-sm-push-0 {
    left: auto;
  }
  .col-sm-offset-12 {
    margin-left: 100%;
  }
  .col-sm-offset-11 {
    margin-left: 91.66666667%;
  }
  .col-sm-offset-10 {
    margin-left: 83.33333333%;
  }
  .col-sm-offset-9 {
    margin-left: 75%;
  }
  .col-sm-offset-8 {
    margin-left: 66.66666667%;
  }
  .col-sm-offset-7 {
    margin-left: 58.33333333%;
  }
  .col-sm-offset-6 {
    margin-left: 50%;
  }
  .col-sm-offset-5 {
    margin-left: 41.66666667%;
  }
  .col-sm-offset-4 {
    margin-left: 33.33333333%;
  }
  .col-sm-offset-3 {
    margin-left: 25%;
  }
  .col-sm-offset-2 {
    margin-left: 16.66666667%;
  }
  .col-sm-offset-1 {
    margin-left: 8.33333333%;
  }
  .col-sm-offset-0 {
    margin-left: 0%;
  }
}
@media (min-width: 992px) {
  .col-md-1, .col-md-2, .col-md-3, .col-md-4, .col-md-5, .col-md-6, .col-md-7, .col-md-8, .col-md-9, .col-md-10, .col-md-11, .col-md-12 {
    float: left;
  }
  .col-md-12 {
    width: 100%;
  }
  .col-md-11 {
    width: 91.66666667%;
  }
  .col-md-10 {
    width: 83.33333333%;
  }
  .col-md-9 {
    width: 75%;
  }
  .col-md-8 {
    width: 66.66666667%;
  }
  .col-md-7 {
    width: 58.33333333%;
  }
  .col-md-6 {
    width: 50%;
  }
  .col-md-5 {
    width: 41.66666667%;
  }
  .col-md-4 {
    width: 33.33333333%;
  }
  .col-md-3 {
    width: 25%;
  }
  .col-md-2 {
    width: 16.66666667%;
  }
  .col-md-1 {
    width: 8.33333333%;
  }
  .col-md-pull-12 {
    right: 100%;
  }
  .col-md-pull-11 {
    right: 91.66666667%;
  }
  .col-md-pull-10 {
    right: 83.33333333%;
  }
  .col-md-pull-9 {
    right: 75%;
  }
  .col-md-pull-8 {
    right: 66.66666667%;
  }
  .col-md-pull-7 {
    right: 58.33333333%;
  }
  .col-md-pull-6 {
    right: 50%;
  }
  .col-md-pull-5 {
    right: 41.66666667%;
  }
  .col-md-pull-4 {
    right: 33.33333333%;
  }
  .col-md-pull-3 {
    right: 25%;
  }
  .col-md-pull-2 {
    right: 16.66666667%;
  }
  .col-md-pull-1 {
    right: 8.33333333%;
  }
  .col-md-pull-0 {
    right: auto;
  }
  .col-md-push-12 {
    left: 100%;
  }
  .col-md-push-11 {
    left: 91.66666667%;
  }
  .col-md-push-10 {
    left: 83.33333333%;
  }
  .col-md-push-9 {
    left: 75%;
  }
  .col-md-push-8 {
    left: 66.66666667%;
  }
  .col-md-push-7 {
    left: 58.33333333%;
  }
  .col-md-push-6 {
    left: 50%;
  }
  .col-md-push-5 {
    left: 41.66666667%;
  }
  .col-md-push-4 {
    left: 33.33333333%;
  }
  .col-md-push-3 {
    left: 25%;
  }
  .col-md-push-2 {
    left: 16.66666667%;
  }
  .col-md-push-1 {
    left: 8.33333333%;
  }
  .col-md-push-0 {
    left: auto;
  }
  .col-md-offset-12 {
    margin-left: 100%;
  }
  .col-md-offset-11 {
    margin-left: 91.66666667%;
  }
  .col-md-offset-10 {
    margin-left: 83.33333333%;
  }
  .col-md-offset-9 {
    margin-left: 75%;
  }
  .col-md-offset-8 {
    margin-left: 66.66666667%;
  }
  .col-md-offset-7 {
    margin-left: 58.33333333%;
  }
  .col-md-offset-6 {
    margin-left: 50%;
  }
  .col-md-offset-5 {
    margin-left: 41.66666667%;
  }
  .col-md-offset-4 {
    margin-left: 33.33333333%;
  }
  .col-md-offset-3 {
    margin-left: 25%;
  }
  .col-md-offset-2 {
    margin-left: 16.66666667%;
  }
  .col-md-offset-1 {
    margin-left: 8.33333333%;
  }
  .col-md-offset-0 {
    margin-left: 0%;
  }
}
@media (min-width: 1200px) {
  .col-lg-1, .col-lg-2, .col-lg-3, .col-lg-4, .col-lg-5, .col-lg-6, .col-lg-7, .col-lg-8, .col-lg-9, .col-lg-10, .col-lg-11, .col-lg-12 {
    float: left;
  }
  .col-lg-12 {
    width: 100%;
  }
  .col-lg-11 {
    width: 91.66666667%;
  }
  .col-lg-10 {
    width: 83.33333333%;
  }
  .col-lg-9 {
    width: 75%;
  }
  .col-lg-8 {
    width: 66.66666667%;
  }
  .col-lg-7 {
    width: 58.33333333%;
  }
  .col-lg-6 {
    width: 50%;
  }
  .col-lg-5 {
    width: 41.66666667%;
  }
  .col-lg-4 {
    width: 33.33333333%;
  }
  .col-lg-3 {
    width: 25%;
  }
  .col-lg-2 {
    width: 16.66666667%;
  }
  .col-lg-1 {
    width: 8.33333333%;
  }
  .col-lg-pull-12 {
    right: 100%;
  }
  .col-lg-pull-11 {
    right: 91.66666667%;
  }
  .col-lg-pull-10 {
    right: 83.33333333%;
  }
  .col-lg-pull-9 {
    right: 75%;
  }
  .col-lg-pull-8 {
    right: 66.66666667%;
  }
  .col-lg-pull-7 {
    right: 58.33333333%;
  }
  .col-lg-pull-6 {
    right: 50%;
  }
  .col-lg-pull-5 {
    right: 41.66666667%;
  }
  .col-lg-pull-4 {
    right: 33.33333333%;
  }
  .col-lg-pull-3 {
    right: 25%;
  }
  .col-lg-pull-2 {
    right: 16.66666667%;
  }
  .col-lg-pull-1 {
    right: 8.33333333%;
  }
  .col-lg-pull-0 {
    right: auto;
  }
  .col-lg-push-12 {
    left: 100%;
  }
  .col-lg-push-11 {
    left: 91.66666667%;
  }
  .col-lg-push-10 {
    left: 83.33333333%;
  }
  .col-lg-push-9 {
    left: 75%;
  }
  .col-lg-push-8 {
    left: 66.66666667%;
  }
  .col-lg-push-7 {
    left: 58.33333333%;
  }
  .col-lg-push-6 {
    left: 50%;
  }
  .col-lg-push-5 {
    left: 41.66666667%;
  }
  .col-lg-push-4 {
    left: 33.33333333%;
  }
  .col-lg-push-3 {
    left: 25%;
  }
  .col-lg-push-2 {
    left: 16.66666667%;
  }
  .col-lg-push-1 {
    left: 8.33333333%;
  }
  .col-lg-push-0 {
    left: auto;
  }
  .col-lg-offset-12 {
    margin-left: 100%;
  }
  .col-lg-offset-11 {
    margin-left: 91.66666667%;
  }
  .col-lg-offset-10 {
    margin-left: 83.33333333%;
  }
  .col-lg-offset-9 {
    margin-left: 75%;
  }
  .col-lg-offset-8 {
    margin-left: 66.66666667%;
  }
  .col-lg-offset-7 {
    margin-left: 58.33333333%;
  }
  .col-lg-offset-6 {
    margin-left: 50%;
  }
  .col-lg-offset-5 {
    margin-left: 41.66666667%;
  }
  .col-lg-offset-4 {
    margin-left: 33.33333333%;
  }
  .col-lg-offset-3 {
    margin-left: 25%;
  }
  .col-lg-offset-2 {
    margin-left: 16.66666667%;
  }
  .col-lg-offset-1 {
    margin-left: 8.33333333%;
  }
  .col-lg-offset-0 {
    margin-left: 0%;
  }
}
table {
  background-color: transparent;
}
caption {
  padding-top: 8px;
  padding-bottom: 8px;
  color: #777777;
  text-align: left;
}
th {
  text-align: left;
}
.table {
  width: 100%;
  max-width: 100%;
  margin-bottom: 18px;
}
.table > thead > tr > th,
.table > tbody > tr > th,
.table > tfoot > tr > th,
.table > thead > tr > td,
.table > tbody > tr > td,
.table > tfoot > tr > td {
  padding: 8px;
  line-height: 1.42857143;
  vertical-align: top;
  border-top: 1px solid #ddd;
}
.table > thead > tr > th {
  vertical-align: bottom;
  border-bottom: 2px solid #ddd;
}
.table > caption + thead > tr:first-child > th,
.table > colgroup + thead > tr:first-child > th,
.table > thead:first-child > tr:first-child > th,
.table > caption + thead > tr:first-child > td,
.table > colgroup + thead > tr:first-child > td,
.table > thead:first-child > tr:first-child > td {
  border-top: 0;
}
.table > tbody + tbody {
  border-top: 2px solid #ddd;
}
.table .table {
  background-color: #fff;
}
.table-condensed > thead > tr > th,
.table-condensed > tbody > tr > th,
.table-condensed > tfoot > tr > th,
.table-condensed > thead > tr > td,
.table-condensed > tbody > tr > td,
.table-condensed > tfoot > tr > td {
  padding: 5px;
}
.table-bordered {
  border: 1px solid #ddd;
}
.table-bordered > thead > tr > th,
.table-bordered > tbody > tr > th,
.table-bordered > tfoot > tr > th,
.table-bordered > thead > tr > td,
.table-bordered > tbody > tr > td,
.table-bordered > tfoot > tr > td {
  border: 1px solid #ddd;
}
.table-bordered > thead > tr > th,
.table-bordered > thead > tr > td {
  border-bottom-width: 2px;
}
.table-striped > tbody > tr:nth-of-type(odd) {
  background-color: #f9f9f9;
}
.table-hover > tbody > tr:hover {
  background-color: #f5f5f5;
}
table col[class*="col-"] {
  position: static;
  float: none;
  display: table-column;
}
table td[class*="col-"],
table th[class*="col-"] {
  position: static;
  float: none;
  display: table-cell;
}
.table > thead > tr > td.active,
.table > tbody > tr > td.active,
.table > tfoot > tr > td.active,
.table > thead > tr > th.active,
.table > tbody > tr > th.active,
.table > tfoot > tr > th.active,
.table > thead > tr.active > td,
.table > tbody > tr.active > td,
.table > tfoot > tr.active > td,
.table > thead > tr.active > th,
.table > tbody > tr.active > th,
.table > tfoot > tr.active > th {
  background-color: #f5f5f5;
}
.table-hover > tbody > tr > td.active:hover,
.table-hover > tbody > tr > th.active:hover,
.table-hover > tbody > tr.active:hover > td,
.table-hover > tbody > tr:hover > .active,
.table-hover > tbody > tr.active:hover > th {
  background-color: #e8e8e8;
}
.table > thead > tr > td.success,
.table > tbody > tr > td.success,
.table > tfoot > tr > td.success,
.table > thead > tr > th.success,
.table > tbody > tr > th.success,
.table > tfoot > tr > th.success,
.table > thead > tr.success > td,
.table > tbody > tr.success > td,
.table > tfoot > tr.success > td,
.table > thead > tr.success > th,
.table > tbody > tr.success > th,
.table > tfoot > tr.success > th {
  background-color: #dff0d8;
}
.table-hover > tbody > tr > td.success:hover,
.table-hover > tbody > tr > th.success:hover,
.table-hover > tbody > tr.success:hover > td,
.table-hover > tbody > tr:hover > .success,
.table-hover > tbody > tr.success:hover > th {
  background-color: #d0e9c6;
}
.table > thead > tr > td.info,
.table > tbody > tr > td.info,
.table > tfoot > tr > td.info,
.table > thead > tr > th.info,
.table > tbody > tr > th.info,
.table > tfoot > tr > th.info,
.table > thead > tr.info > td,
.table > tbody > tr.info > td,
.table > tfoot > tr.info > td,
.table > thead > tr.info > th,
.table > tbody > tr.info > th,
.table > tfoot > tr.info > th {
  background-color: #d9edf7;
}
.table-hover > tbody > tr > td.info:hover,
.table-hover > tbody > tr > th.info:hover,
.table-hover > tbody > tr.info:hover > td,
.table-hover > tbody > tr:hover > .info,
.table-hover > tbody > tr.info:hover > th {
  background-color: #c4e3f3;
}
.table > thead > tr > td.warning,
.table > tbody > tr > td.warning,
.table > tfoot > tr > td.warning,
.table > thead > tr > th.warning,
.table > tbody > tr > th.warning,
.table > tfoot > tr > th.warning,
.table > thead > tr.warning > td,
.table > tbody > tr.warning > td,
.table > tfoot > tr.warning > td,
.table > thead > tr.warning > th,
.table > tbody > tr.warning > th,
.table > tfoot > tr.warning > th {
  background-color: #fcf8e3;
}
.table-hover > tbody > tr > td.warning:hover,
.table-hover > tbody > tr > th.warning:hover,
.table-hover > tbody > tr.warning:hover > td,
.table-hover > tbody > tr:hover > .warning,
.table-hover > tbody > tr.warning:hover > th {
  background-color: #faf2cc;
}
.table > thead > tr > td.danger,
.table > tbody > tr > td.danger,
.table > tfoot > tr > td.danger,
.table > thead > tr > th.danger,
.table > tbody > tr > th.danger,
.table > tfoot > tr > th.danger,
.table > thead > tr.danger > td,
.table > tbody > tr.danger > td,
.table > tfoot > tr.danger > td,
.table > thead > tr.danger > th,
.table > tbody > tr.danger > th,
.table > tfoot > tr.danger > th {
  background-color: #f2dede;
}
.table-hover > tbody > tr > td.danger:hover,
.table-hover > tbody > tr > th.danger:hover,
.table-hover > tbody > tr.danger:hover > td,
.table-hover > tbody > tr:hover > .danger,
.table-hover > tbody > tr.danger:hover > th {
  background-color: #ebcccc;
}
.table-responsive {
  overflow-x: auto;
  min-height: 0.01%;
}
@media screen and (max-width: 767px) {
  .table-responsive {
    width: 100%;
    margin-bottom: 13.5px;
    overflow-y: hidden;
    -ms-overflow-style: -ms-autohiding-scrollbar;
    border: 1px solid #ddd;
  }
  .table-responsive > .table {
    margin-bottom: 0;
  }
  .table-responsive > .table > thead > tr > th,
  .table-responsive > .table > tbody > tr > th,
  .table-responsive > .table > tfoot > tr > th,
  .table-responsive > .table > thead > tr > td,
  .table-responsive > .table > tbody > tr > td,
  .table-responsive > .table > tfoot > tr > td {
    white-space: nowrap;
  }
  .table-responsive > .table-bordered {
    border: 0;
  }
  .table-responsive > .table-bordered > thead > tr > th:first-child,
  .table-responsive > .table-bordered > tbody > tr > th:first-child,
  .table-responsive > .table-bordered > tfoot > tr > th:first-child,
  .table-responsive > .table-bordered > thead > tr > td:first-child,
  .table-responsive > .table-bordered > tbody > tr > td:first-child,
  .table-responsive > .table-bordered > tfoot > tr > td:first-child {
    border-left: 0;
  }
  .table-responsive > .table-bordered > thead > tr > th:last-child,
  .table-responsive > .table-bordered > tbody > tr > th:last-child,
  .table-responsive > .table-bordered > tfoot > tr > th:last-child,
  .table-responsive > .table-bordered > thead > tr > td:last-child,
  .table-responsive > .table-bordered > tbody > tr > td:last-child,
  .table-responsive > .table-bordered > tfoot > tr > td:last-child {
    border-right: 0;
  }
  .table-responsive > .table-bordered > tbody > tr:last-child > th,
  .table-responsive > .table-bordered > tfoot > tr:last-child > th,
  .table-responsive > .table-bordered > tbody > tr:last-child > td,
  .table-responsive > .table-bordered > tfoot > tr:last-child > td {
    border-bottom: 0;
  }
}
fieldset {
  padding: 0;
  margin: 0;
  border: 0;
  min-width: 0;
}
legend {
  display: block;
  width: 100%;
  padding: 0;
  margin-bottom: 18px;
  font-size: 19.5px;
  line-height: inherit;
  color: #333333;
  border: 0;
  border-bottom: 1px solid #e5e5e5;
}
label {
  display: inline-block;
  max-width: 100%;
  margin-bottom: 5px;
  font-weight: bold;
}
input[type="search"] {
  -webkit-box-sizing: border-box;
  -moz-box-sizing: border-box;
  box-sizing: border-box;
}
input[type="radio"],
input[type="checkbox"] {
  margin: 4px 0 0;
  margin-top: 1px \9;
  line-height: normal;
}
input[type="file"] {
  display: block;
}
input[type="range"] {
  display: block;
  width: 100%;
}
select[multiple],
select[size] {
  height: auto;
}
input[type="file"]:focus,
input[type="radio"]:focus,
input[type="checkbox"]:focus {
  outline: 5px auto -webkit-focus-ring-color;
  outline-offset: -2px;
}
output {
  display: block;
  padding-top: 7px;
  font-size: 13px;
  line-height: 1.42857143;
  color: #555555;
}
.form-control {
  display: block;
  width: 100%;
  height: 32px;
  padding: 6px 12px;
  font-size: 13px;
  line-height: 1.42857143;
  color: #555555;
  background-color: #fff;
  background-image: none;
  border: 1px solid #ccc;
  border-radius: 2px;
  -webkit-box-shadow: inset 0 1px 1px rgba(0, 0, 0, 0.075);
  box-shadow: inset 0 1px 1px rgba(0, 0, 0, 0.075);
  -webkit-transition: border-color ease-in-out .15s, box-shadow ease-in-out .15s;
  -o-transition: border-color ease-in-out .15s, box-shadow ease-in-out .15s;
  transition: border-color ease-in-out .15s, box-shadow ease-in-out .15s;
}
.form-control:focus {
  border-color: #66afe9;
  outline: 0;
  -webkit-box-shadow: inset 0 1px 1px rgba(0,0,0,.075), 0 0 8px rgba(102, 175, 233, 0.6);
  box-shadow: inset 0 1px 1px rgba(0,0,0,.075), 0 0 8px rgba(102, 175, 233, 0.6);
}
.form-control::-moz-placeholder {
  color: #999;
  opacity: 1;
}
.form-control:-ms-input-placeholder {
  color: #999;
}
.form-control::-webkit-input-placeholder {
  color: #999;
}
.form-control::-ms-expand {
  border: 0;
  background-color: transparent;
}
.form-control[disabled],
.form-control[readonly],
fieldset[disabled] .form-control {
  background-color: #eeeeee;
  opacity: 1;
}
.form-control[disabled],
fieldset[disabled] .form-control {
  cursor: not-allowed;
}
textarea.form-control {
  height: auto;
}
input[type="search"] {
  -webkit-appearance: none;
}
@media screen and (-webkit-min-device-pixel-ratio: 0) {
  input[type="date"].form-control,
  input[type="time"].form-control,
  input[type="datetime-local"].form-control,
  input[type="month"].form-control {
    line-height: 32px;
  }
  input[type="date"].input-sm,
  input[type="time"].input-sm,
  input[type="datetime-local"].input-sm,
  input[type="month"].input-sm,
  .input-group-sm input[type="date"],
  .input-group-sm input[type="time"],
  .input-group-sm input[type="datetime-local"],
  .input-group-sm input[type="month"] {
    line-height: 30px;
  }
  input[type="date"].input-lg,
  input[type="time"].input-lg,
  input[type="datetime-local"].input-lg,
  input[type="month"].input-lg,
  .input-group-lg input[type="date"],
  .input-group-lg input[type="time"],
  .input-group-lg input[type="datetime-local"],
  .input-group-lg input[type="month"] {
    line-height: 45px;
  }
}
.form-group {
  margin-bottom: 15px;
}
.radio,
.checkbox {
  position: relative;
  display: block;
  margin-top: 10px;
  margin-bottom: 10px;
}
.radio label,
.checkbox label {
  min-height: 18px;
  padding-left: 20px;
  margin-bottom: 0;
  font-weight: normal;
  cursor: pointer;
}
.radio input[type="radio"],
.radio-inline input[type="radio"],
.checkbox input[type="checkbox"],
.checkbox-inline input[type="checkbox"] {
  position: absolute;
  margin-left: -20px;
  margin-top: 4px \9;
}
.radio + .radio,
.checkbox + .checkbox {
  margin-top: -5px;
}
.radio-inline,
.checkbox-inline {
  position: relative;
  display: inline-block;
  padding-left: 20px;
  margin-bottom: 0;
  vertical-align: middle;
  font-weight: normal;
  cursor: pointer;
}
.radio-inline + .radio-inline,
.checkbox-inline + .checkbox-inline {
  margin-top: 0;
  margin-left: 10px;
}
input[type="radio"][disabled],
input[type="checkbox"][disabled],
input[type="radio"].disabled,
input[type="checkbox"].disabled,
fieldset[disabled] input[type="radio"],
fieldset[disabled] input[type="checkbox"] {
  cursor: not-allowed;
}
.radio-inline.disabled,
.checkbox-inline.disabled,
fieldset[disabled] .radio-inline,
fieldset[disabled] .checkbox-inline {
  cursor: not-allowed;
}
.radio.disabled label,
.checkbox.disabled label,
fieldset[disabled] .radio label,
fieldset[disabled] .checkbox label {
  cursor: not-allowed;
}
.form-control-static {
  padding-top: 7px;
  padding-bottom: 7px;
  margin-bottom: 0;
  min-height: 31px;
}
.form-control-static.input-lg,
.form-control-static.input-sm {
  padding-left: 0;
  padding-right: 0;
}
.input-sm {
  height: 30px;
  padding: 5px 10px;
  font-size: 12px;
  line-height: 1.5;
  border-radius: 1px;
}
select.input-sm {
  height: 30px;
  line-height: 30px;
}
textarea.input-sm,
select[multiple].input-sm {
  height: auto;
}
.form-group-sm .form-control {
  height: 30px;
  padding: 5px 10px;
  font-size: 12px;
  line-height: 1.5;
  border-radius: 1px;
}
.form-group-sm select.form-control {
  height: 30px;
  line-height: 30px;
}
.form-group-sm textarea.form-control,
.form-group-sm select[multiple].form-control {
  height: auto;
}
.form-group-sm .form-control-static {
  height: 30px;
  min-height: 30px;
  padding: 6px 10px;
  font-size: 12px;
  line-height: 1.5;
}
.input-lg {
  height: 45px;
  padding: 10px 16px;
  font-size: 17px;
  line-height: 1.3333333;
  border-radius: 3px;
}
select.input-lg {
  height: 45px;
  line-height: 45px;
}
textarea.input-lg,
select[multiple].input-lg {
  height: auto;
}
.form-group-lg .form-control {
  height: 45px;
  padding: 10px 16px;
  font-size: 17px;
  line-height: 1.3333333;
  border-radius: 3px;
}
.form-group-lg select.form-control {
  height: 45px;
  line-height: 45px;
}
.form-group-lg textarea.form-control,
.form-group-lg select[multiple].form-control {
  height: auto;
}
.form-group-lg .form-control-static {
  height: 45px;
  min-height: 35px;
  padding: 11px 16px;
  font-size: 17px;
  line-height: 1.3333333;
}
.has-feedback {
  position: relative;
}
.has-feedback .form-control {
  padding-right: 40px;
}
.form-control-feedback {
  position: absolute;
  top: 0;
  right: 0;
  z-index: 2;
  display: block;
  width: 32px;
  height: 32px;
  line-height: 32px;
  text-align: center;
  pointer-events: none;
}
.input-lg + .form-control-feedback,
.input-group-lg + .form-control-feedback,
.form-group-lg .form-control + .form-control-feedback {
  width: 45px;
  height: 45px;
  line-height: 45px;
}
.input-sm + .form-control-feedback,
.input-group-sm + .form-control-feedback,
.form-group-sm .form-control + .form-control-feedback {
  width: 30px;
  height: 30px;
  line-height: 30px;
}
.has-success .help-block,
.has-success .control-label,
.has-success .radio,
.has-success .checkbox,
.has-success .radio-inline,
.has-success .checkbox-inline,
.has-success.radio label,
.has-success.checkbox label,
.has-success.radio-inline label,
.has-success.checkbox-inline label {
  color: #3c763d;
}
.has-success .form-control {
  border-color: #3c763d;
  -webkit-box-shadow: inset 0 1px 1px rgba(0, 0, 0, 0.075);
  box-shadow: inset 0 1px 1px rgba(0, 0, 0, 0.075);
}
.has-success .form-control:focus {
  border-color: #2b542c;
  -webkit-box-shadow: inset 0 1px 1px rgba(0, 0, 0, 0.075), 0 0 6px #67b168;
  box-shadow: inset 0 1px 1px rgba(0, 0, 0, 0.075), 0 0 6px #67b168;
}
.has-success .input-group-addon {
  color: #3c763d;
  border-color: #3c763d;
  background-color: #dff0d8;
}
.has-success .form-control-feedback {
  color: #3c763d;
}
.has-warning .help-block,
.has-warning .control-label,
.has-warning .radio,
.has-warning .checkbox,
.has-warning .radio-inline,
.has-warning .checkbox-inline,
.has-warning.radio label,
.has-warning.checkbox label,
.has-warning.radio-inline label,
.has-warning.checkbox-inline label {
  color: #8a6d3b;
}
.has-warning .form-control {
  border-color: #8a6d3b;
  -webkit-box-shadow: inset 0 1px 1px rgba(0, 0, 0, 0.075);
  box-shadow: inset 0 1px 1px rgba(0, 0, 0, 0.075);
}
.has-warning .form-control:focus {
  border-color: #66512c;
  -webkit-box-shadow: inset 0 1px 1px rgba(0, 0, 0, 0.075), 0 0 6px #c0a16b;
  box-shadow: inset 0 1px 1px rgba(0, 0, 0, 0.075), 0 0 6px #c0a16b;
}
.has-warning .input-group-addon {
  color: #8a6d3b;
  border-color: #8a6d3b;
  background-color: #fcf8e3;
}
.has-warning .form-control-feedback {
  color: #8a6d3b;
}
.has-error .help-block,
.has-error .control-label,
.has-error .radio,
.has-error .checkbox,
.has-error .radio-inline,
.has-error .checkbox-inline,
.has-error.radio label,
.has-error.checkbox label,
.has-error.radio-inline label,
.has-error.checkbox-inline label {
  color: #a94442;
}
.has-error .form-control {
  border-color: #a94442;
  -webkit-box-shadow: inset 0 1px 1px rgba(0, 0, 0, 0.075);
  box-shadow: inset 0 1px 1px rgba(0, 0, 0, 0.075);
}
.has-error .form-control:focus {
  border-color: #843534;
  -webkit-box-shadow: inset 0 1px 1px rgba(0, 0, 0, 0.075), 0 0 6px #ce8483;
  box-shadow: inset 0 1px 1px rgba(0, 0, 0, 0.075), 0 0 6px #ce8483;
}
.has-error .input-group-addon {
  color: #a94442;
  border-color: #a94442;
  background-color: #f2dede;
}
.has-error .form-control-feedback {
  color: #a94442;
}
.has-feedback label ~ .form-control-feedback {
  top: 23px;
}
.has-feedback label.sr-only ~ .form-control-feedback {
  top: 0;
}
.help-block {
  display: block;
  margin-top: 5px;
  margin-bottom: 10px;
  color: #404040;
}
@media (min-width: 768px) {
  .form-inline .form-group {
    display: inline-block;
    margin-bottom: 0;
    vertical-align: middle;
  }
  .form-inline .form-control {
    display: inline-block;
    width: auto;
    vertical-align: middle;
  }
  .form-inline .form-control-static {
    display: inline-block;
  }
  .form-inline .input-group {
    display: inline-table;
    vertical-align: middle;
  }
  .form-inline .input-group .input-group-addon,
  .form-inline .input-group .input-group-btn,
  .form-inline .input-group .form-control {
    width: auto;
  }
  .form-inline .input-group > .form-control {
    width: 100%;
  }
  .form-inline .control-label {
    margin-bottom: 0;
    vertical-align: middle;
  }
  .form-inline .radio,
  .form-inline .checkbox {
    display: inline-block;
    margin-top: 0;
    margin-bottom: 0;
    vertical-align: middle;
  }
  .form-inline .radio label,
  .form-inline .checkbox label {
    padding-left: 0;
  }
  .form-inline .radio input[type="radio"],
  .form-inline .checkbox input[type="checkbox"] {
    position: relative;
    margin-left: 0;
  }
  .form-inline .has-feedback .form-control-feedback {
    top: 0;
  }
}
.form-horizontal .radio,
.form-horizontal .checkbox,
.form-horizontal .radio-inline,
.form-horizontal .checkbox-inline {
  margin-top: 0;
  margin-bottom: 0;
  padding-top: 7px;
}
.form-horizontal .radio,
.form-horizontal .checkbox {
  min-height: 25px;
}
.form-horizontal .form-group {
  margin-left: 0px;
  margin-right: 0px;
}
@media (min-width: 768px) {
  .form-horizontal .control-label {
    text-align: right;
    margin-bottom: 0;
    padding-top: 7px;
  }
}
.form-horizontal .has-feedback .form-control-feedback {
  right: 0px;
}
@media (min-width: 768px) {
  .form-horizontal .form-group-lg .control-label {
    padding-top: 11px;
    font-size: 17px;
  }
}
@media (min-width: 768px) {
  .form-horizontal .form-group-sm .control-label {
    padding-top: 6px;
    font-size: 12px;
  }
}
.btn {
  display: inline-block;
  margin-bottom: 0;
  font-weight: normal;
  text-align: center;
  vertical-align: middle;
  touch-action: manipulation;
  cursor: pointer;
  background-image: none;
  border: 1px solid transparent;
  white-space: nowrap;
  padding: 6px 12px;
  font-size: 13px;
  line-height: 1.42857143;
  border-radius: 2px;
  -webkit-user-select: none;
  -moz-user-select: none;
  -ms-user-select: none;
  user-select: none;
}
.btn:focus,
.btn:active:focus,
.btn.active:focus,
.btn.focus,
.btn:active.focus,
.btn.active.focus {
  outline: 5px auto -webkit-focus-ring-color;
  outline-offset: -2px;
}
.btn:hover,
.btn:focus,
.btn.focus {
  color: #333;
  text-decoration: none;
}
.btn:active,
.btn.active {
  outline: 0;
  background-image: none;
  -webkit-box-shadow: inset 0 3px 5px rgba(0, 0, 0, 0.125);
  box-shadow: inset 0 3px 5px rgba(0, 0, 0, 0.125);
}
.btn.disabled,
.btn[disabled],
fieldset[disabled] .btn {
  cursor: not-allowed;
  opacity: 0.65;
  filter: alpha(opacity=65);
  -webkit-box-shadow: none;
  box-shadow: none;
}
a.btn.disabled,
fieldset[disabled] a.btn {
  pointer-events: none;
}
.btn-default {
  color: #333;
  background-color: #fff;
  border-color: #ccc;
}
.btn-default:focus,
.btn-default.focus {
  color: #333;
  background-color: #e6e6e6;
  border-color: #8c8c8c;
}
.btn-default:hover {
  color: #333;
  background-color: #e6e6e6;
  border-color: #adadad;
}
.btn-default:active,
.btn-default.active,
.open > .dropdown-toggle.btn-default {
  color: #333;
  background-color: #e6e6e6;
  border-color: #adadad;
}
.btn-default:active:hover,
.btn-default.active:hover,
.open > .dropdown-toggle.btn-default:hover,
.btn-default:active:focus,
.btn-default.active:focus,
.open > .dropdown-toggle.btn-default:focus,
.btn-default:active.focus,
.btn-default.active.focus,
.open > .dropdown-toggle.btn-default.focus {
  color: #333;
  background-color: #d4d4d4;
  border-color: #8c8c8c;
}
.btn-default:active,
.btn-default.active,
.open > .dropdown-toggle.btn-default {
  background-image: none;
}
.btn-default.disabled:hover,
.btn-default[disabled]:hover,
fieldset[disabled] .btn-default:hover,
.btn-default.disabled:focus,
.btn-default[disabled]:focus,
fieldset[disabled] .btn-default:focus,
.btn-default.disabled.focus,
.btn-default[disabled].focus,
fieldset[disabled] .btn-default.focus {
  background-color: #fff;
  border-color: #ccc;
}
.btn-default .badge {
  color: #fff;
  background-color: #333;
}
.btn-primary {
  color: #fff;
  background-color: #337ab7;
  border-color: #2e6da4;
}
.btn-primary:focus,
.btn-primary.focus {
  color: #fff;
  background-color: #286090;
  border-color: #122b40;
}
.btn-primary:hover {
  color: #fff;
  background-color: #286090;
  border-color: #204d74;
}
.btn-primary:active,
.btn-primary.active,
.open > .dropdown-toggle.btn-primary {
  color: #fff;
  background-color: #286090;
  border-color: #204d74;
}
.btn-primary:active:hover,
.btn-primary.active:hover,
.open > .dropdown-toggle.btn-primary:hover,
.btn-primary:active:focus,
.btn-primary.active:focus,
.open > .dropdown-toggle.btn-primary:focus,
.btn-primary:active.focus,
.btn-primary.active.focus,
.open > .dropdown-toggle.btn-primary.focus {
  color: #fff;
  background-color: #204d74;
  border-color: #122b40;
}
.btn-primary:active,
.btn-primary.active,
.open > .dropdown-toggle.btn-primary {
  background-image: none;
}
.btn-primary.disabled:hover,
.btn-primary[disabled]:hover,
fieldset[disabled] .btn-primary:hover,
.btn-primary.disabled:focus,
.btn-primary[disabled]:focus,
fieldset[disabled] .btn-primary:focus,
.btn-primary.disabled.focus,
.btn-primary[disabled].focus,
fieldset[disabled] .btn-primary.focus {
  background-color: #337ab7;
  border-color: #2e6da4;
}
.btn-primary .badge {
  color: #337ab7;
  background-color: #fff;
}
.btn-success {
  color: #fff;
  background-color: #5cb85c;
  border-color: #4cae4c;
}
.btn-success:focus,
.btn-success.focus {
  color: #fff;
  background-color: #449d44;
  border-color: #255625;
}
.btn-success:hover {
  color: #fff;
  background-color: #449d44;
  border-color: #398439;
}
.btn-success:active,
.btn-success.active,
.open > .dropdown-toggle.btn-success {
  color: #fff;
  background-color: #449d44;
  border-color: #398439;
}
.btn-success:active:hover,
.btn-success.active:hover,
.open > .dropdown-toggle.btn-success:hover,
.btn-success:active:focus,
.btn-success.active:focus,
.open > .dropdown-toggle.btn-success:focus,
.btn-success:active.focus,
.btn-success.active.focus,
.open > .dropdown-toggle.btn-success.focus {
  color: #fff;
  background-color: #398439;
  border-color: #255625;
}
.btn-success:active,
.btn-success.active,
.open > .dropdown-toggle.btn-success {
  background-image: none;
}
.btn-success.disabled:hover,
.btn-success[disabled]:hover,
fieldset[disabled] .btn-success:hover,
.btn-success.disabled:focus,
.btn-success[disabled]:focus,
fieldset[disabled] .btn-success:focus,
.btn-success.disabled.focus,
.btn-success[disabled].focus,
fieldset[disabled] .btn-success.focus {
  background-color: #5cb85c;
  border-color: #4cae4c;
}
.btn-success .badge {
  color: #5cb85c;
  background-color: #fff;
}
.btn-info {
  color: #fff;
  background-color: #5bc0de;
  border-color: #46b8da;
}
.btn-info:focus,
.btn-info.focus {
  color: #fff;
  background-color: #31b0d5;
  border-color: #1b6d85;
}
.btn-info:hover {
  color: #fff;
  background-color: #31b0d5;
  border-color: #269abc;
}
.btn-info:active,
.btn-info.active,
.open > .dropdown-toggle.btn-info {
  color: #fff;
  background-color: #31b0d5;
  border-color: #269abc;
}
.btn-info:active:hover,
.btn-info.active:hover,
.open > .dropdown-toggle.btn-info:hover,
.btn-info:active:focus,
.btn-info.active:focus,
.open > .dropdown-toggle.btn-info:focus,
.btn-info:active.focus,
.btn-info.active.focus,
.open > .dropdown-toggle.btn-info.focus {
  color: #fff;
  background-color: #269abc;
  border-color: #1b6d85;
}
.btn-info:active,
.btn-info.active,
.open > .dropdown-toggle.btn-info {
  background-image: none;
}
.btn-info.disabled:hover,
.btn-info[disabled]:hover,
fieldset[disabled] .btn-info:hover,
.btn-info.disabled:focus,
.btn-info[disabled]:focus,
fieldset[disabled] .btn-info:focus,
.btn-info.disabled.focus,
.btn-info[disabled].focus,
fieldset[disabled] .btn-info.focus {
  background-color: #5bc0de;
  border-color: #46b8da;
}
.btn-info .badge {
  color: #5bc0de;
  background-color: #fff;
}
.btn-warning {
  color: #fff;
  background-color: #f0ad4e;
  border-color: #eea236;
}
.btn-warning:focus,
.btn-warning.focus {
  color: #fff;
  background-color: #ec971f;
  border-color: #985f0d;
}
.btn-warning:hover {
  color: #fff;
  background-color: #ec971f;
  border-color: #d58512;
}
.btn-warning:active,
.btn-warning.active,
.open > .dropdown-toggle.btn-warning {
  color: #fff;
  background-color: #ec971f;
  border-color: #d58512;
}
.btn-warning:active:hover,
.btn-warning.active:hover,
.open > .dropdown-toggle.btn-warning:hover,
.btn-warning:active:focus,
.btn-warning.active:focus,
.open > .dropdown-toggle.btn-warning:focus,
.btn-warning:active.focus,
.btn-warning.active.focus,
.open > .dropdown-toggle.btn-warning.focus {
  color: #fff;
  background-color: #d58512;
  border-color: #985f0d;
}
.btn-warning:active,
.btn-warning.active,
.open > .dropdown-toggle.btn-warning {
  background-image: none;
}
.btn-warning.disabled:hover,
.btn-warning[disabled]:hover,
fieldset[disabled] .btn-warning:hover,
.btn-warning.disabled:focus,
.btn-warning[disabled]:focus,
fieldset[disabled] .btn-warning:focus,
.btn-warning.disabled.focus,
.btn-warning[disabled].focus,
fieldset[disabled] .btn-warning.focus {
  background-color: #f0ad4e;
  border-color: #eea236;
}
.btn-warning .badge {
  color: #f0ad4e;
  background-color: #fff;
}
.btn-danger {
  color: #fff;
  background-color: #d9534f;
  border-color: #d43f3a;
}
.btn-danger:focus,
.btn-danger.focus {
  color: #fff;
  background-color: #c9302c;
  border-color: #761c19;
}
.btn-danger:hover {
  color: #fff;
  background-color: #c9302c;
  border-color: #ac2925;
}
.btn-danger:active,
.btn-danger.active,
.open > .dropdown-toggle.btn-danger {
  color: #fff;
  background-color: #c9302c;
  border-color: #ac2925;
}
.btn-danger:active:hover,
.btn-danger.active:hover,
.open > .dropdown-toggle.btn-danger:hover,
.btn-danger:active:focus,
.btn-danger.active:focus,
.open > .dropdown-toggle.btn-danger:focus,
.btn-danger:active.focus,
.btn-danger.active.focus,
.open > .dropdown-toggle.btn-danger.focus {
  color: #fff;
  background-color: #ac2925;
  border-color: #761c19;
}
.btn-danger:active,
.btn-danger.active,
.open > .dropdown-toggle.btn-danger {
  background-image: none;
}
.btn-danger.disabled:hover,
.btn-danger[disabled]:hover,
fieldset[disabled] .btn-danger:hover,
.btn-danger.disabled:focus,
.btn-danger[disabled]:focus,
fieldset[disabled] .btn-danger:focus,
.btn-danger.disabled.focus,
.btn-danger[disabled].focus,
fieldset[disabled] .btn-danger.focus {
  background-color: #d9534f;
  border-color: #d43f3a;
}
.btn-danger .badge {
  color: #d9534f;
  background-color: #fff;
}
.btn-link {
  color: #337ab7;
  font-weight: normal;
  border-radius: 0;
}
.btn-link,
.btn-link:active,
.btn-link.active,
.btn-link[disabled],
fieldset[disabled] .btn-link {
  background-color: transparent;
  -webkit-box-shadow: none;
  box-shadow: none;
}
.btn-link,
.btn-link:hover,
.btn-link:focus,
.btn-link:active {
  border-color: transparent;
}
.btn-link:hover,
.btn-link:focus {
  color: #23527c;
  text-decoration: underline;
  background-color: transparent;
}
.btn-link[disabled]:hover,
fieldset[disabled] .btn-link:hover,
.btn-link[disabled]:focus,
fieldset[disabled] .btn-link:focus {
  color: #777777;
  text-decoration: none;
}
.btn-lg,
.btn-group-lg > .btn {
  padding: 10px 16px;
  font-size: 17px;
  line-height: 1.3333333;
  border-radius: 3px;
}
.btn-sm,
.btn-group-sm > .btn {
  padding: 5px 10px;
  font-size: 12px;
  line-height: 1.5;
  border-radius: 1px;
}
.btn-xs,
.btn-group-xs > .btn {
  padding: 1px 5px;
  font-size: 12px;
  line-height: 1.5;
  border-radius: 1px;
}
.btn-block {
  display: block;
  width: 100%;
}
.btn-block + .btn-block {
  margin-top: 5px;
}
input[type="submit"].btn-block,
input[type="reset"].btn-block,
input[type="button"].btn-block {
  width: 100%;
}
.fade {
  opacity: 0;
  -webkit-transition: opacity 0.15s linear;
  -o-transition: opacity 0.15s linear;
  transition: opacity 0.15s linear;
}
.fade.in {
  opacity: 1;
}
.collapse {
  display: none;
}
.collapse.in {
  display: block;
}
tr.collapse.in {
  display: table-row;
}
tbody.collapse.in {
  display: table-row-group;
}
.collapsing {
  position: relative;
  height: 0;
  overflow: hidden;
  -webkit-transition-property: height, visibility;
  transition-property: height, visibility;
  -webkit-transition-duration: 0.35s;
  transition-duration: 0.35s;
  -webkit-transition-timing-function: ease;
  transition-timing-function: ease;
}
.caret {
  display: inline-block;
  width: 0;
  height: 0;
  margin-left: 2px;
  vertical-align: middle;
  border-top: 4px dashed;
  border-top: 4px solid \9;
  border-right: 4px solid transparent;
  border-left: 4px solid transparent;
}
.dropup,
.dropdown {
  position: relative;
}
.dropdown-toggle:focus {
  outline: 0;
}
.dropdown-menu {
  position: absolute;
  top: 100%;
  left: 0;
  z-index: 1000;
  display: none;
  float: left;
  min-width: 160px;
  padding: 5px 0;
  margin: 2px 0 0;
  list-style: none;
  font-size: 13px;
  text-align: left;
  background-color: #fff;
  border: 1px solid #ccc;
  border: 1px solid rgba(0, 0, 0, 0.15);
  border-radius: 2px;
  -webkit-box-shadow: 0 6px 12px rgba(0, 0, 0, 0.175);
  box-shadow: 0 6px 12px rgba(0, 0, 0, 0.175);
  background-clip: padding-box;
}
.dropdown-menu.pull-right {
  right: 0;
  left: auto;
}
.dropdown-menu .divider {
  height: 1px;
  margin: 8px 0;
  overflow: hidden;
  background-color: #e5e5e5;
}
.dropdown-menu > li > a {
  display: block;
  padding: 3px 20px;
  clear: both;
  font-weight: normal;
  line-height: 1.42857143;
  color: #333333;
  white-space: nowrap;
}
.dropdown-menu > li > a:hover,
.dropdown-menu > li > a:focus {
  text-decoration: none;
  color: #262626;
  background-color: #f5f5f5;
}
.dropdown-menu > .active > a,
.dropdown-menu > .active > a:hover,
.dropdown-menu > .active > a:focus {
  color: #fff;
  text-decoration: none;
  outline: 0;
  background-color: #337ab7;
}
.dropdown-menu > .disabled > a,
.dropdown-menu > .disabled > a:hover,
.dropdown-menu > .disabled > a:focus {
  color: #777777;
}
.dropdown-menu > .disabled > a:hover,
.dropdown-menu > .disabled > a:focus {
  text-decoration: none;
  background-color: transparent;
  background-image: none;
  filter: progid:DXImageTransform.Microsoft.gradient(enabled = false);
  cursor: not-allowed;
}
.open > .dropdown-menu {
  display: block;
}
.open > a {
  outline: 0;
}
.dropdown-menu-right {
  left: auto;
  right: 0;
}
.dropdown-menu-left {
  left: 0;
  right: auto;
}
.dropdown-header {
  display: block;
  padding: 3px 20px;
  font-size: 12px;
  line-height: 1.42857143;
  color: #777777;
  white-space: nowrap;
}
.dropdown-backdrop {
  position: fixed;
  left: 0;
  right: 0;
  bottom: 0;
  top: 0;
  z-index: 990;
}
.pull-right > .dropdown-menu {
  right: 0;
  left: auto;
}
.dropup .caret,
.navbar-fixed-bottom .dropdown .caret {
  border-top: 0;
  border-bottom: 4px dashed;
  border-bottom: 4px solid \9;
  content: "";
}
.dropup .dropdown-menu,
.navbar-fixed-bottom .dropdown .dropdown-menu {
  top: auto;
  bottom: 100%;
  margin-bottom: 2px;
}
@media (min-width: 541px) {
  .navbar-right .dropdown-menu {
    left: auto;
    right: 0;
  }
  .navbar-right .dropdown-menu-left {
    left: 0;
    right: auto;
  }
}
.btn-group,
.btn-group-vertical {
  position: relative;
  display: inline-block;
  vertical-align: middle;
}
.btn-group > .btn,
.btn-group-vertical > .btn {
  position: relative;
  float: left;
}
.btn-group > .btn:hover,
.btn-group-vertical > .btn:hover,
.btn-group > .btn:focus,
.btn-group-vertical > .btn:focus,
.btn-group > .btn:active,
.btn-group-vertical > .btn:active,
.btn-group > .btn.active,
.btn-group-vertical > .btn.active {
  z-index: 2;
}
.btn-group .btn + .btn,
.btn-group .btn + .btn-group,
.btn-group .btn-group + .btn,
.btn-group .btn-group + .btn-group {
  margin-left: -1px;
}
.btn-toolbar {
  margin-left: -5px;
}
.btn-toolbar .btn,
.btn-toolbar .btn-group,
.btn-toolbar .input-group {
  float: left;
}
.btn-toolbar > .btn,
.btn-toolbar > .btn-group,
.btn-toolbar > .input-group {
  margin-left: 5px;
}
.btn-group > .btn:not(:first-child):not(:last-child):not(.dropdown-toggle) {
  border-radius: 0;
}
.btn-group > .btn:first-child {
  margin-left: 0;
}
.btn-group > .btn:first-child:not(:last-child):not(.dropdown-toggle) {
  border-bottom-right-radius: 0;
  border-top-right-radius: 0;
}
.btn-group > .btn:last-child:not(:first-child),
.btn-group > .dropdown-toggle:not(:first-child) {
  border-bottom-left-radius: 0;
  border-top-left-radius: 0;
}
.btn-group > .btn-group {
  float: left;
}
.btn-group > .btn-group:not(:first-child):not(:last-child) > .btn {
  border-radius: 0;
}
.btn-group > .btn-group:first-child:not(:last-child) > .btn:last-child,
.btn-group > .btn-group:first-child:not(:last-child) > .dropdown-toggle {
  border-bottom-right-radius: 0;
  border-top-right-radius: 0;
}
.btn-group > .btn-group:last-child:not(:first-child) > .btn:first-child {
  border-bottom-left-radius: 0;
  border-top-left-radius: 0;
}
.btn-group .dropdown-toggle:active,
.btn-group.open .dropdown-toggle {
  outline: 0;
}
.btn-group > .btn + .dropdown-toggle {
  padding-left: 8px;
  padding-right: 8px;
}
.btn-group > .btn-lg + .dropdown-toggle {
  padding-left: 12px;
  padding-right: 12px;
}
.btn-group.open .dropdown-toggle {
  -webkit-box-shadow: inset 0 3px 5px rgba(0, 0, 0, 0.125);
  box-shadow: inset 0 3px 5px rgba(0, 0, 0, 0.125);
}
.btn-group.open .dropdown-toggle.btn-link {
  -webkit-box-shadow: none;
  box-shadow: none;
}
.btn .caret {
  margin-left: 0;
}
.btn-lg .caret {
  border-width: 5px 5px 0;
  border-bottom-width: 0;
}
.dropup .btn-lg .caret {
  border-width: 0 5px 5px;
}
.btn-group-vertical > .btn,
.btn-group-vertical > .btn-group,
.btn-group-vertical > .btn-group > .btn {
  display: block;
  float: none;
  width: 100%;
  max-width: 100%;
}
.btn-group-vertical > .btn-group > .btn {
  float: none;
}
.btn-group-vertical > .btn + .btn,
.btn-group-vertical > .btn + .btn-group,
.btn-group-vertical > .btn-group + .btn,
.btn-group-vertical > .btn-group + .btn-group {
  margin-top: -1px;
  margin-left: 0;
}
.btn-group-vertical > .btn:not(:first-child):not(:last-child) {
  border-radius: 0;
}
.btn-group-vertical > .btn:first-child:not(:last-child) {
  border-top-right-radius: 2px;
  border-top-left-radius: 2px;
  border-bottom-right-radius: 0;
  border-bottom-left-radius: 0;
}
.btn-group-vertical > .btn:last-child:not(:first-child) {
  border-top-right-radius: 0;
  border-top-left-radius: 0;
  border-bottom-right-radius: 2px;
  border-bottom-left-radius: 2px;
}
.btn-group-vertical > .btn-group:not(:first-child):not(:last-child) > .btn {
  border-radius: 0;
}
.btn-group-vertical > .btn-group:first-child:not(:last-child) > .btn:last-child,
.btn-group-vertical > .btn-group:first-child:not(:last-child) > .dropdown-toggle {
  border-bottom-right-radius: 0;
  border-bottom-left-radius: 0;
}
.btn-group-vertical > .btn-group:last-child:not(:first-child) > .btn:first-child {
  border-top-right-radius: 0;
  border-top-left-radius: 0;
}
.btn-group-justified {
  display: table;
  width: 100%;
  table-layout: fixed;
  border-collapse: separate;
}
.btn-group-justified > .btn,
.btn-group-justified > .btn-group {
  float: none;
  display: table-cell;
  width: 1%;
}
.btn-group-justified > .btn-group .btn {
  width: 100%;
}
.btn-group-justified > .btn-group .dropdown-menu {
  left: auto;
}
[data-toggle="buttons"] > .btn input[type="radio"],
[data-toggle="buttons"] > .btn-group > .btn input[type="radio"],
[data-toggle="buttons"] > .btn input[type="checkbox"],
[data-toggle="buttons"] > .btn-group > .btn input[type="checkbox"] {
  position: absolute;
  clip: rect(0, 0, 0, 0);
  pointer-events: none;
}
.input-group {
  position: relative;
  display: table;
  border-collapse: separate;
}
.input-group[class*="col-"] {
  float: none;
  padding-left: 0;
  padding-right: 0;
}
.input-group .form-control {
  position: relative;
  z-index: 2;
  float: left;
  width: 100%;
  margin-bottom: 0;
}
.input-group .form-control:focus {
  z-index: 3;
}
.input-group-lg > .form-control,
.input-group-lg > .input-group-addon,
.input-group-lg > .input-group-btn > .btn {
  height: 45px;
  padding: 10px 16px;
  font-size: 17px;
  line-height: 1.3333333;
  border-radius: 3px;
}
select.input-group-lg > .form-control,
select.input-group-lg > .input-group-addon,
select.input-group-lg > .input-group-btn > .btn {
  height: 45px;
  line-height: 45px;
}
textarea.input-group-lg > .form-control,
textarea.input-group-lg > .input-group-addon,
textarea.input-group-lg > .input-group-btn > .btn,
select[multiple].input-group-lg > .form-control,
select[multiple].input-group-lg > .input-group-addon,
select[multiple].input-group-lg > .input-group-btn > .btn {
  height: auto;
}
.input-group-sm > .form-control,
.input-group-sm > .input-group-addon,
.input-group-sm > .input-group-btn > .btn {
  height: 30px;
  padding: 5px 10px;
  font-size: 12px;
  line-height: 1.5;
  border-radius: 1px;
}
select.input-group-sm > .form-control,
select.input-group-sm > .input-group-addon,
select.input-group-sm > .input-group-btn > .btn {
  height: 30px;
  line-height: 30px;
}
textarea.input-group-sm > .form-control,
textarea.input-group-sm > .input-group-addon,
textarea.input-group-sm > .input-group-btn > .btn,
select[multiple].input-group-sm > .form-control,
select[multiple].input-group-sm > .input-group-addon,
select[multiple].input-group-sm > .input-group-btn > .btn {
  height: auto;
}
.input-group-addon,
.input-group-btn,
.input-group .form-control {
  display: table-cell;
}
.input-group-addon:not(:first-child):not(:last-child),
.input-group-btn:not(:first-child):not(:last-child),
.input-group .form-control:not(:first-child):not(:last-child) {
  border-radius: 0;
}
.input-group-addon,
.input-group-btn {
  width: 1%;
  white-space: nowrap;
  vertical-align: middle;
}
.input-group-addon {
  padding: 6px 12px;
  font-size: 13px;
  font-weight: normal;
  line-height: 1;
  color: #555555;
  text-align: center;
  background-color: #eeeeee;
  border: 1px solid #ccc;
  border-radius: 2px;
}
.input-group-addon.input-sm {
  padding: 5px 10px;
  font-size: 12px;
  border-radius: 1px;
}
.input-group-addon.input-lg {
  padding: 10px 16px;
  font-size: 17px;
  border-radius: 3px;
}
.input-group-addon input[type="radio"],
.input-group-addon input[type="checkbox"] {
  margin-top: 0;
}
.input-group .form-control:first-child,
.input-group-addon:first-child,
.input-group-btn:first-child > .btn,
.input-group-btn:first-child > .btn-group > .btn,
.input-group-btn:first-child > .dropdown-toggle,
.input-group-btn:last-child > .btn:not(:last-child):not(.dropdown-toggle),
.input-group-btn:last-child > .btn-group:not(:last-child) > .btn {
  border-bottom-right-radius: 0;
  border-top-right-radius: 0;
}
.input-group-addon:first-child {
  border-right: 0;
}
.input-group .form-control:last-child,
.input-group-addon:last-child,
.input-group-btn:last-child > .btn,
.input-group-btn:last-child > .btn-group > .btn,
.input-group-btn:last-child > .dropdown-toggle,
.input-group-btn:first-child > .btn:not(:first-child),
.input-group-btn:first-child > .btn-group:not(:first-child) > .btn {
  border-bottom-left-radius: 0;
  border-top-left-radius: 0;
}
.input-group-addon:last-child {
  border-left: 0;
}
.input-group-btn {
  position: relative;
  font-size: 0;
  white-space: nowrap;
}
.input-group-btn > .btn {
  position: relative;
}
.input-group-btn > .btn + .btn {
  margin-left: -1px;
}
.input-group-btn > .btn:hover,
.input-group-btn > .btn:focus,
.input-group-btn > .btn:active {
  z-index: 2;
}
.input-group-btn:first-child > .btn,
.input-group-btn:first-child > .btn-group {
  margin-right: -1px;
}
.input-group-btn:last-child > .btn,
.input-group-btn:last-child > .btn-group {
  z-index: 2;
  margin-left: -1px;
}
.nav {
  margin-bottom: 0;
  padding-left: 0;
  list-style: none;
}
.nav > li {
  position: relative;
  display: block;
}
.nav > li > a {
  position: relative;
  display: block;
  padding: 10px 15px;
}
.nav > li > a:hover,
.nav > li > a:focus {
  text-decoration: none;
  background-color: #eeeeee;
}
.nav > li.disabled > a {
  color: #777777;
}
.nav > li.disabled > a:hover,
.nav > li.disabled > a:focus {
  color: #777777;
  text-decoration: none;
  background-color: transparent;
  cursor: not-allowed;
}
.nav .open > a,
.nav .open > a:hover,
.nav .open > a:focus {
  background-color: #eeeeee;
  border-color: #337ab7;
}
.nav .nav-divider {
  height: 1px;
  margin: 8px 0;
  overflow: hidden;
  background-color: #e5e5e5;
}
.nav > li > a > img {
  max-width: none;
}
.nav-tabs {
  border-bottom: 1px solid #ddd;
}
.nav-tabs > li {
  float: left;
  margin-bottom: -1px;
}
.nav-tabs > li > a {
  margin-right: 2px;
  line-height: 1.42857143;
  border: 1px solid transparent;
  border-radius: 2px 2px 0 0;
}
.nav-tabs > li > a:hover {
  border-color: #eeeeee #eeeeee #ddd;
}
.nav-tabs > li.active > a,
.nav-tabs > li.active > a:hover,
.nav-tabs > li.active > a:focus {
  color: #555555;
  background-color: #fff;
  border: 1px solid #ddd;
  border-bottom-color: transparent;
  cursor: default;
}
.nav-tabs.nav-justified {
  width: 100%;
  border-bottom: 0;
}
.nav-tabs.nav-justified > li {
  float: none;
}
.nav-tabs.nav-justified > li > a {
  text-align: center;
  margin-bottom: 5px;
}
.nav-tabs.nav-justified > .dropdown .dropdown-menu {
  top: auto;
  left: auto;
}
@media (min-width: 768px) {
  .nav-tabs.nav-justified > li {
    display: table-cell;
    width: 1%;
  }
  .nav-tabs.nav-justified > li > a {
    margin-bottom: 0;
  }
}
.nav-tabs.nav-justified > li > a {
  margin-right: 0;
  border-radius: 2px;
}
.nav-tabs.nav-justified > .active > a,
.nav-tabs.nav-justified > .active > a:hover,
.nav-tabs.nav-justified > .active > a:focus {
  border: 1px solid #ddd;
}
@media (min-width: 768px) {
  .nav-tabs.nav-justified > li > a {
    border-bottom: 1px solid #ddd;
    border-radius: 2px 2px 0 0;
  }
  .nav-tabs.nav-justified > .active > a,
  .nav-tabs.nav-justified > .active > a:hover,
  .nav-tabs.nav-justified > .active > a:focus {
    border-bottom-color: #fff;
  }
}
.nav-pills > li {
  float: left;
}
.nav-pills > li > a {
  border-radius: 2px;
}
.nav-pills > li + li {
  margin-left: 2px;
}
.nav-pills > li.active > a,
.nav-pills > li.active > a:hover,
.nav-pills > li.active > a:focus {
  color: #fff;
  background-color: #337ab7;
}
.nav-stacked > li {
  float: none;
}
.nav-stacked > li + li {
  margin-top: 2px;
  margin-left: 0;
}
.nav-justified {
  width: 100%;
}
.nav-justified > li {
  float: none;
}
.nav-justified > li > a {
  text-align: center;
  margin-bottom: 5px;
}
.nav-justified > .dropdown .dropdown-menu {
  top: auto;
  left: auto;
}
@media (min-width: 768px) {
  .nav-justified > li {
    display: table-cell;
    width: 1%;
  }
  .nav-justified > li > a {
    margin-bottom: 0;
  }
}
.nav-tabs-justified {
  border-bottom: 0;
}
.nav-tabs-justified > li > a {
  margin-right: 0;
  border-radius: 2px;
}
.nav-tabs-justified > .active > a,
.nav-tabs-justified > .active > a:hover,
.nav-tabs-justified > .active > a:focus {
  border: 1px solid #ddd;
}
@media (min-width: 768px) {
  .nav-tabs-justified > li > a {
    border-bottom: 1px solid #ddd;
    border-radius: 2px 2px 0 0;
  }
  .nav-tabs-justified > .active > a,
  .nav-tabs-justified > .active > a:hover,
  .nav-tabs-justified > .active > a:focus {
    border-bottom-color: #fff;
  }
}
.tab-content > .tab-pane {
  display: none;
}
.tab-content > .active {
  display: block;
}
.nav-tabs .dropdown-menu {
  margin-top: -1px;
  border-top-right-radius: 0;
  border-top-left-radius: 0;
}
.navbar {
  position: relative;
  min-height: 30px;
  margin-bottom: 18px;
  border: 1px solid transparent;
}
@media (min-width: 541px) {
  .navbar {
    border-radius: 2px;
  }
}
@media (min-width: 541px) {
  .navbar-header {
    float: left;
  }
}
.navbar-collapse {
  overflow-x: visible;
  padding-right: 0px;
  padding-left: 0px;
  border-top: 1px solid transparent;
  box-shadow: inset 0 1px 0 rgba(255, 255, 255, 0.1);
  -webkit-overflow-scrolling: touch;
}
.navbar-collapse.in {
  overflow-y: auto;
}
@media (min-width: 541px) {
  .navbar-collapse {
    width: auto;
    border-top: 0;
    box-shadow: none;
  }
  .navbar-collapse.collapse {
    display: block !important;
    height: auto !important;
    padding-bottom: 0;
    overflow: visible !important;
  }
  .navbar-collapse.in {
    overflow-y: visible;
  }
  .navbar-fixed-top .navbar-collapse,
  .navbar-static-top .navbar-collapse,
  .navbar-fixed-bottom .navbar-collapse {
    padding-left: 0;
    padding-right: 0;
  }
}
.navbar-fixed-top .navbar-collapse,
.navbar-fixed-bottom .navbar-collapse {
  max-height: 340px;
}
@media (max-device-width: 540px) and (orientation: landscape) {
  .navbar-fixed-top .navbar-collapse,
  .navbar-fixed-bottom .navbar-collapse {
    max-height: 200px;
  }
}
.container > .navbar-header,
.container-fluid > .navbar-header,
.container > .navbar-collapse,
.container-fluid > .navbar-collapse {
  margin-right: 0px;
  margin-left: 0px;
}
@media (min-width: 541px) {
  .container > .navbar-header,
  .container-fluid > .navbar-header,
  .container > .navbar-collapse,
  .container-fluid > .navbar-collapse {
    margin-right: 0;
    margin-left: 0;
  }
}
.navbar-static-top {
  z-index: 1000;
  border-width: 0 0 1px;
}
@media (min-width: 541px) {
  .navbar-static-top {
    border-radius: 0;
  }
}
.navbar-fixed-top,
.navbar-fixed-bottom {
  position: fixed;
  right: 0;
  left: 0;
  z-index: 1030;
}
@media (min-width: 541px) {
  .navbar-fixed-top,
  .navbar-fixed-bottom {
    border-radius: 0;
  }
}
.navbar-fixed-top {
  top: 0;
  border-width: 0 0 1px;
}
.navbar-fixed-bottom {
  bottom: 0;
  margin-bottom: 0;
  border-width: 1px 0 0;
}
.navbar-brand {
  float: left;
  padding: 6px 0px;
  font-size: 17px;
  line-height: 18px;
  height: 30px;
}
.navbar-brand:hover,
.navbar-brand:focus {
  text-decoration: none;
}
.navbar-brand > img {
  display: block;
}
@media (min-width: 541px) {
  .navbar > .container .navbar-brand,
  .navbar > .container-fluid .navbar-brand {
    margin-left: 0px;
  }
}
.navbar-toggle {
  position: relative;
  float: right;
  margin-right: 0px;
  padding: 9px 10px;
  margin-top: -2px;
  margin-bottom: -2px;
  background-color: transparent;
  background-image: none;
  border: 1px solid transparent;
  border-radius: 2px;
}
.navbar-toggle:focus {
  outline: 0;
}
.navbar-toggle .icon-bar {
  display: block;
  width: 22px;
  height: 2px;
  border-radius: 1px;
}
.navbar-toggle .icon-bar + .icon-bar {
  margin-top: 4px;
}
@media (min-width: 541px) {
  .navbar-toggle {
    display: none;
  }
}
.navbar-nav {
  margin: 3px 0px;
}
.navbar-nav > li > a {
  padding-top: 10px;
  padding-bottom: 10px;
  line-height: 18px;
}
@media (max-width: 540px) {
  .navbar-nav .open .dropdown-menu {
    position: static;
    float: none;
    width: auto;
    margin-top: 0;
    background-color: transparent;
    border: 0;
    box-shadow: none;
  }
  .navbar-nav .open .dropdown-menu > li > a,
  .navbar-nav .open .dropdown-menu .dropdown-header {
    padding: 5px 15px 5px 25px;
  }
  .navbar-nav .open .dropdown-menu > li > a {
    line-height: 18px;
  }
  .navbar-nav .open .dropdown-menu > li > a:hover,
  .navbar-nav .open .dropdown-menu > li > a:focus {
    background-image: none;
  }
}
@media (min-width: 541px) {
  .navbar-nav {
    float: left;
    margin: 0;
  }
  .navbar-nav > li {
    float: left;
  }
  .navbar-nav > li > a {
    padding-top: 6px;
    padding-bottom: 6px;
  }
}
.navbar-form {
  margin-left: 0px;
  margin-right: 0px;
  padding: 10px 0px;
  border-top: 1px solid transparent;
  border-bottom: 1px solid transparent;
  -webkit-box-shadow: inset 0 1px 0 rgba(255, 255, 255, 0.1), 0 1px 0 rgba(255, 255, 255, 0.1);
  box-shadow: inset 0 1px 0 rgba(255, 255, 255, 0.1), 0 1px 0 rgba(255, 255, 255, 0.1);
  margin-top: -1px;
  margin-bottom: -1px;
}
@media (min-width: 768px) {
  .navbar-form .form-group {
    display: inline-block;
    margin-bottom: 0;
    vertical-align: middle;
  }
  .navbar-form .form-control {
    display: inline-block;
    width: auto;
    vertical-align: middle;
  }
  .navbar-form .form-control-static {
    display: inline-block;
  }
  .navbar-form .input-group {
    display: inline-table;
    vertical-align: middle;
  }
  .navbar-form .input-group .input-group-addon,
  .navbar-form .input-group .input-group-btn,
  .navbar-form .input-group .form-control {
    width: auto;
  }
  .navbar-form .input-group > .form-control {
    width: 100%;
  }
  .navbar-form .control-label {
    margin-bottom: 0;
    vertical-align: middle;
  }
  .navbar-form .radio,
  .navbar-form .checkbox {
    display: inline-block;
    margin-top: 0;
    margin-bottom: 0;
    vertical-align: middle;
  }
  .navbar-form .radio label,
  .navbar-form .checkbox label {
    padding-left: 0;
  }
  .navbar-form .radio input[type="radio"],
  .navbar-form .checkbox input[type="checkbox"] {
    position: relative;
    margin-left: 0;
  }
  .navbar-form .has-feedback .form-control-feedback {
    top: 0;
  }
}
@media (max-width: 540px) {
  .navbar-form .form-group {
    margin-bottom: 5px;
  }
  .navbar-form .form-group:last-child {
    margin-bottom: 0;
  }
}
@media (min-width: 541px) {
  .navbar-form {
    width: auto;
    border: 0;
    margin-left: 0;
    margin-right: 0;
    padding-top: 0;
    padding-bottom: 0;
    -webkit-box-shadow: none;
    box-shadow: none;
  }
}
.navbar-nav > li > .dropdown-menu {
  margin-top: 0;
  border-top-right-radius: 0;
  border-top-left-radius: 0;
}
.navbar-fixed-bottom .navbar-nav > li > .dropdown-menu {
  margin-bottom: 0;
  border-top-right-radius: 2px;
  border-top-left-radius: 2px;
  border-bottom-right-radius: 0;
  border-bottom-left-radius: 0;
}
.navbar-btn {
  margin-top: -1px;
  margin-bottom: -1px;
}
.navbar-btn.btn-sm {
  margin-top: 0px;
  margin-bottom: 0px;
}
.navbar-btn.btn-xs {
  margin-top: 4px;
  margin-bottom: 4px;
}
.navbar-text {
  margin-top: 6px;
  margin-bottom: 6px;
}
@media (min-width: 541px) {
  .navbar-text {
    float: left;
    margin-left: 0px;
    margin-right: 0px;
  }
}
@media (min-width: 541px) {
  .navbar-left {
    float: left !important;
    float: left;
  }
  .navbar-right {
    float: right !important;
    float: right;
    margin-right: 0px;
  }
  .navbar-right ~ .navbar-right {
    margin-right: 0;
  }
}
.navbar-default {
  background-color: #f8f8f8;
  border-color: #e7e7e7;
}
.navbar-default .navbar-brand {
  color: #777;
}
.navbar-default .navbar-brand:hover,
.navbar-default .navbar-brand:focus {
  color: #5e5e5e;
  background-color: transparent;
}
.navbar-default .navbar-text {
  color: #777;
}
.navbar-default .navbar-nav > li > a {
  color: #777;
}
.navbar-default .navbar-nav > li > a:hover,
.navbar-default .navbar-nav > li > a:focus {
  color: #333;
  background-color: transparent;
}
.navbar-default .navbar-nav > .active > a,
.navbar-default .navbar-nav > .active > a:hover,
.navbar-default .navbar-nav > .active > a:focus {
  color: #555;
  background-color: #e7e7e7;
}
.navbar-default .navbar-nav > .disabled > a,
.navbar-default .navbar-nav > .disabled > a:hover,
.navbar-default .navbar-nav > .disabled > a:focus {
  color: #ccc;
  background-color: transparent;
}
.navbar-default .navbar-toggle {
  border-color: #ddd;
}
.navbar-default .navbar-toggle:hover,
.navbar-default .navbar-toggle:focus {
  background-color: #ddd;
}
.navbar-default .navbar-toggle .icon-bar {
  background-color: #888;
}
.navbar-default .navbar-collapse,
.navbar-default .navbar-form {
  border-color: #e7e7e7;
}
.navbar-default .navbar-nav > .open > a,
.navbar-default .navbar-nav > .open > a:hover,
.navbar-default .navbar-nav > .open > a:focus {
  background-color: #e7e7e7;
  color: #555;
}
@media (max-width: 540px) {
  .navbar-default .navbar-nav .open .dropdown-menu > li > a {
    color: #777;
  }
  .navbar-default .navbar-nav .open .dropdown-menu > li > a:hover,
  .navbar-default .navbar-nav .open .dropdown-menu > li > a:focus {
    color: #333;
    background-color: transparent;
  }
  .navbar-default .navbar-nav .open .dropdown-menu > .active > a,
  .navbar-default .navbar-nav .open .dropdown-menu > .active > a:hover,
  .navbar-default .navbar-nav .open .dropdown-menu > .active > a:focus {
    color: #555;
    background-color: #e7e7e7;
  }
  .navbar-default .navbar-nav .open .dropdown-menu > .disabled > a,
  .navbar-default .navbar-nav .open .dropdown-menu > .disabled > a:hover,
  .navbar-default .navbar-nav .open .dropdown-menu > .disabled > a:focus {
    color: #ccc;
    background-color: transparent;
  }
}
.navbar-default .navbar-link {
  color: #777;
}
.navbar-default .navbar-link:hover {
  color: #333;
}
.navbar-default .btn-link {
  color: #777;
}
.navbar-default .btn-link:hover,
.navbar-default .btn-link:focus {
  color: #333;
}
.navbar-default .btn-link[disabled]:hover,
fieldset[disabled] .navbar-default .btn-link:hover,
.navbar-default .btn-link[disabled]:focus,
fieldset[disabled] .navbar-default .btn-link:focus {
  color: #ccc;
}
.navbar-inverse {
  background-color: #222;
  border-color: #080808;
}
.navbar-inverse .navbar-brand {
  color: #9d9d9d;
}
.navbar-inverse .navbar-brand:hover,
.navbar-inverse .navbar-brand:focus {
  color: #fff;
  background-color: transparent;
}
.navbar-inverse .navbar-text {
  color: #9d9d9d;
}
.navbar-inverse .navbar-nav > li > a {
  color: #9d9d9d;
}
.navbar-inverse .navbar-nav > li > a:hover,
.navbar-inverse .navbar-nav > li > a:focus {
  color: #fff;
  background-color: transparent;
}
.navbar-inverse .navbar-nav > .active > a,
.navbar-inverse .navbar-nav > .active > a:hover,
.navbar-inverse .navbar-nav > .active > a:focus {
  color: #fff;
  background-color: #080808;
}
.navbar-inverse .navbar-nav > .disabled > a,
.navbar-inverse .navbar-nav > .disabled > a:hover,
.navbar-inverse .navbar-nav > .disabled > a:focus {
  color: #444;
  background-color: transparent;
}
.navbar-inverse .navbar-toggle {
  border-color: #333;
}
.navbar-inverse .navbar-toggle:hover,
.navbar-inverse .navbar-toggle:focus {
  background-color: #333;
}
.navbar-inverse .navbar-toggle .icon-bar {
  background-color: #fff;
}
.navbar-inverse .navbar-collapse,
.navbar-inverse .navbar-form {
  border-color: #101010;
}
.navbar-inverse .navbar-nav > .open > a,
.navbar-inverse .navbar-nav > .open > a:hover,
.navbar-inverse .navbar-nav > .open > a:focus {
  background-color: #080808;
  color: #fff;
}
@media (max-width: 540px) {
  .navbar-inverse .navbar-nav .open .dropdown-menu > .dropdown-header {
    border-color: #080808;
  }
  .navbar-inverse .navbar-nav .open .dropdown-menu .divider {
    background-color: #080808;
  }
  .navbar-inverse .navbar-nav .open .dropdown-menu > li > a {
    color: #9d9d9d;
  }
  .navbar-inverse .navbar-nav .open .dropdown-menu > li > a:hover,
  .navbar-inverse .navbar-nav .open .dropdown-menu > li > a:focus {
    color: #fff;
    background-color: transparent;
  }
  .navbar-inverse .navbar-nav .open .dropdown-menu > .active > a,
  .navbar-inverse .navbar-nav .open .dropdown-menu > .active > a:hover,
  .navbar-inverse .navbar-nav .open .dropdown-menu > .active > a:focus {
    color: #fff;
    background-color: #080808;
  }
  .navbar-inverse .navbar-nav .open .dropdown-menu > .disabled > a,
  .navbar-inverse .navbar-nav .open .dropdown-menu > .disabled > a:hover,
  .navbar-inverse .navbar-nav .open .dropdown-menu > .disabled > a:focus {
    color: #444;
    background-color: transparent;
  }
}
.navbar-inverse .navbar-link {
  color: #9d9d9d;
}
.navbar-inverse .navbar-link:hover {
  color: #fff;
}
.navbar-inverse .btn-link {
  color: #9d9d9d;
}
.navbar-inverse .btn-link:hover,
.navbar-inverse .btn-link:focus {
  color: #fff;
}
.navbar-inverse .btn-link[disabled]:hover,
fieldset[disabled] .navbar-inverse .btn-link:hover,
.navbar-inverse .btn-link[disabled]:focus,
fieldset[disabled] .navbar-inverse .btn-link:focus {
  color: #444;
}
.breadcrumb {
  padding: 8px 15px;
  margin-bottom: 18px;
  list-style: none;
  background-color: #f5f5f5;
  border-radius: 2px;
}
.breadcrumb > li {
  display: inline-block;
}
.breadcrumb > li + li:before {
  content: "/\00a0";
  padding: 0 5px;
  color: #5e5e5e;
}
.breadcrumb > .active {
  color: #777777;
}
.pagination {
  display: inline-block;
  padding-left: 0;
  margin: 18px 0;
  border-radius: 2px;
}
.pagination > li {
  display: inline;
}
.pagination > li > a,
.pagination > li > span {
  position: relative;
  float: left;
  padding: 6px 12px;
  line-height: 1.42857143;
  text-decoration: none;
  color: #337ab7;
  background-color: #fff;
  border: 1px solid #ddd;
  margin-left: -1px;
}
.pagination > li:first-child > a,
.pagination > li:first-child > span {
  margin-left: 0;
  border-bottom-left-radius: 2px;
  border-top-left-radius: 2px;
}
.pagination > li:last-child > a,
.pagination > li:last-child > span {
  border-bottom-right-radius: 2px;
  border-top-right-radius: 2px;
}
.pagination > li > a:hover,
.pagination > li > span:hover,
.pagination > li > a:focus,
.pagination > li > span:focus {
  z-index: 2;
  color: #23527c;
  background-color: #eeeeee;
  border-color: #ddd;
}
.pagination > .active > a,
.pagination > .active > span,
.pagination > .active > a:hover,
.pagination > .active > span:hover,
.pagination > .active > a:focus,
.pagination > .active > span:focus {
  z-index: 3;
  color: #fff;
  background-color: #337ab7;
  border-color: #337ab7;
  cursor: default;
}
.pagination > .disabled > span,
.pagination > .disabled > span:hover,
.pagination > .disabled > span:focus,
.pagination > .disabled > a,
.pagination > .disabled > a:hover,
.pagination > .disabled > a:focus {
  color: #777777;
  background-color: #fff;
  border-color: #ddd;
  cursor: not-allowed;
}
.pagination-lg > li > a,
.pagination-lg > li > span {
  padding: 10px 16px;
  font-size: 17px;
  line-height: 1.3333333;
}
.pagination-lg > li:first-child > a,
.pagination-lg > li:first-child > span {
  border-bottom-left-radius: 3px;
  border-top-left-radius: 3px;
}
.pagination-lg > li:last-child > a,
.pagination-lg > li:last-child > span {
  border-bottom-right-radius: 3px;
  border-top-right-radius: 3px;
}
.pagination-sm > li > a,
.pagination-sm > li > span {
  padding: 5px 10px;
  font-size: 12px;
  line-height: 1.5;
}
.pagination-sm > li:first-child > a,
.pagination-sm > li:first-child > span {
  border-bottom-left-radius: 1px;
  border-top-left-radius: 1px;
}
.pagination-sm > li:last-child > a,
.pagination-sm > li:last-child > span {
  border-bottom-right-radius: 1px;
  border-top-right-radius: 1px;
}
.pager {
  padding-left: 0;
  margin: 18px 0;
  list-style: none;
  text-align: center;
}
.pager li {
  display: inline;
}
.pager li > a,
.pager li > span {
  display: inline-block;
  padding: 5px 14px;
  background-color: #fff;
  border: 1px solid #ddd;
  border-radius: 15px;
}
.pager li > a:hover,
.pager li > a:focus {
  text-decoration: none;
  background-color: #eeeeee;
}
.pager .next > a,
.pager .next > span {
  float: right;
}
.pager .previous > a,
.pager .previous > span {
  float: left;
}
.pager .disabled > a,
.pager .disabled > a:hover,
.pager .disabled > a:focus,
.pager .disabled > span {
  color: #777777;
  background-color: #fff;
  cursor: not-allowed;
}
.label {
  display: inline;
  padding: .2em .6em .3em;
  font-size: 75%;
  font-weight: bold;
  line-height: 1;
  color: #fff;
  text-align: center;
  white-space: nowrap;
  vertical-align: baseline;
  border-radius: .25em;
}
a.label:hover,
a.label:focus {
  color: #fff;
  text-decoration: none;
  cursor: pointer;
}
.label:empty {
  display: none;
}
.btn .label {
  position: relative;
  top: -1px;
}
.label-default {
  background-color: #777777;
}
.label-default[href]:hover,
.label-default[href]:focus {
  background-color: #5e5e5e;
}
.label-primary {
  background-color: #337ab7;
}
.label-primary[href]:hover,
.label-primary[href]:focus {
  background-color: #286090;
}
.label-success {
  background-color: #5cb85c;
}
.label-success[href]:hover,
.label-success[href]:focus {
  background-color: #449d44;
}
.label-info {
  background-color: #5bc0de;
}
.label-info[href]:hover,
.label-info[href]:focus {
  background-color: #31b0d5;
}
.label-warning {
  background-color: #f0ad4e;
}
.label-warning[href]:hover,
.label-warning[href]:focus {
  background-color: #ec971f;
}
.label-danger {
  background-color: #d9534f;
}
.label-danger[href]:hover,
.label-danger[href]:focus {
  background-color: #c9302c;
}
.badge {
  display: inline-block;
  min-width: 10px;
  padding: 3px 7px;
  font-size: 12px;
  font-weight: bold;
  color: #fff;
  line-height: 1;
  vertical-align: middle;
  white-space: nowrap;
  text-align: center;
  background-color: #777777;
  border-radius: 10px;
}
.badge:empty {
  display: none;
}
.btn .badge {
  position: relative;
  top: -1px;
}
.btn-xs .badge,
.btn-group-xs > .btn .badge {
  top: 0;
  padding: 1px 5px;
}
a.badge:hover,
a.badge:focus {
  color: #fff;
  text-decoration: none;
  cursor: pointer;
}
.list-group-item.active > .badge,
.nav-pills > .active > a > .badge {
  color: #337ab7;
  background-color: #fff;
}
.list-group-item > .badge {
  float: right;
}
.list-group-item > .badge + .badge {
  margin-right: 5px;
}
.nav-pills > li > a > .badge {
  margin-left: 3px;
}
.jumbotron {
  padding-top: 30px;
  padding-bottom: 30px;
  margin-bottom: 30px;
  color: inherit;
  background-color: #eeeeee;
}
.jumbotron h1,
.jumbotron .h1 {
  color: inherit;
}
.jumbotron p {
  margin-bottom: 15px;
  font-size: 20px;
  font-weight: 200;
}
.jumbotron > hr {
  border-top-color: #d5d5d5;
}
.container .jumbotron,
.container-fluid .jumbotron {
  border-radius: 3px;
  padding-left: 0px;
  padding-right: 0px;
}
.jumbotron .container {
  max-width: 100%;
}
@media screen and (min-width: 768px) {
  .jumbotron {
    padding-top: 48px;
    padding-bottom: 48px;
  }
  .container .jumbotron,
  .container-fluid .jumbotron {
    padding-left: 60px;
    padding-right: 60px;
  }
  .jumbotron h1,
  .jumbotron .h1 {
    font-size: 59px;
  }
}
.thumbnail {
  display: block;
  padding: 4px;
  margin-bottom: 18px;
  line-height: 1.42857143;
  background-color: #fff;
  border: 1px solid #ddd;
  border-radius: 2px;
  -webkit-transition: border 0.2s ease-in-out;
  -o-transition: border 0.2s ease-in-out;
  transition: border 0.2s ease-in-out;
}
.thumbnail > img,
.thumbnail a > img {
  margin-left: auto;
  margin-right: auto;
}
a.thumbnail:hover,
a.thumbnail:focus,
a.thumbnail.active {
  border-color: #337ab7;
}
.thumbnail .caption {
  padding: 9px;
  color: #000;
}
.alert {
  padding: 15px;
  margin-bottom: 18px;
  border: 1px solid transparent;
  border-radius: 2px;
}
.alert h4 {
  margin-top: 0;
  color: inherit;
}
.alert .alert-link {
  font-weight: bold;
}
.alert > p,
.alert > ul {
  margin-bottom: 0;
}
.alert > p + p {
  margin-top: 5px;
}
.alert-dismissable,
.alert-dismissible {
  padding-right: 35px;
}
.alert-dismissable .close,
.alert-dismissible .close {
  position: relative;
  top: -2px;
  right: -21px;
  color: inherit;
}
.alert-success {
  background-color: #dff0d8;
  border-color: #d6e9c6;
  color: #3c763d;
}
.alert-success hr {
  border-top-color: #c9e2b3;
}
.alert-success .alert-link {
  color: #2b542c;
}
.alert-info {
  background-color: #d9edf7;
  border-color: #bce8f1;
  color: #31708f;
}
.alert-info hr {
  border-top-color: #a6e1ec;
}
.alert-info .alert-link {
  color: #245269;
}
.alert-warning {
  background-color: #fcf8e3;
  border-color: #faebcc;
  color: #8a6d3b;
}
.alert-warning hr {
  border-top-color: #f7e1b5;
}
.alert-warning .alert-link {
  color: #66512c;
}
.alert-danger {
  background-color: #f2dede;
  border-color: #ebccd1;
  color: #a94442;
}
.alert-danger hr {
  border-top-color: #e4b9c0;
}
.alert-danger .alert-link {
  color: #843534;
}
@-webkit-keyframes progress-bar-stripes {
  from {
    background-position: 40px 0;
  }
  to {
    background-position: 0 0;
  }
}
@keyframes progress-bar-stripes {
  from {
    background-position: 40px 0;
  }
  to {
    background-position: 0 0;
  }
}
.progress {
  overflow: hidden;
  height: 18px;
  margin-bottom: 18px;
  background-color: #f5f5f5;
  border-radius: 2px;
  -webkit-box-shadow: inset 0 1px 2px rgba(0, 0, 0, 0.1);
  box-shadow: inset 0 1px 2px rgba(0, 0, 0, 0.1);
}
.progress-bar {
  float: left;
  width: 0%;
  height: 100%;
  font-size: 12px;
  line-height: 18px;
  color: #fff;
  text-align: center;
  background-color: #337ab7;
  -webkit-box-shadow: inset 0 -1px 0 rgba(0, 0, 0, 0.15);
  box-shadow: inset 0 -1px 0 rgba(0, 0, 0, 0.15);
  -webkit-transition: width 0.6s ease;
  -o-transition: width 0.6s ease;
  transition: width 0.6s ease;
}
.progress-striped .progress-bar,
.progress-bar-striped {
  background-image: -webkit-linear-gradient(45deg, rgba(255, 255, 255, 0.15) 25%, transparent 25%, transparent 50%, rgba(255, 255, 255, 0.15) 50%, rgba(255, 255, 255, 0.15) 75%, transparent 75%, transparent);
  background-image: -o-linear-gradient(45deg, rgba(255, 255, 255, 0.15) 25%, transparent 25%, transparent 50%, rgba(255, 255, 255, 0.15) 50%, rgba(255, 255, 255, 0.15) 75%, transparent 75%, transparent);
  background-image: linear-gradient(45deg, rgba(255, 255, 255, 0.15) 25%, transparent 25%, transparent 50%, rgba(255, 255, 255, 0.15) 50%, rgba(255, 255, 255, 0.15) 75%, transparent 75%, transparent);
  background-size: 40px 40px;
}
.progress.active .progress-bar,
.progress-bar.active {
  -webkit-animation: progress-bar-stripes 2s linear infinite;
  -o-animation: progress-bar-stripes 2s linear infinite;
  animation: progress-bar-stripes 2s linear infinite;
}
.progress-bar-success {
  background-color: #5cb85c;
}
.progress-striped .progress-bar-success {
  background-image: -webkit-linear-gradient(45deg, rgba(255, 255, 255, 0.15) 25%, transparent 25%, transparent 50%, rgba(255, 255, 255, 0.15) 50%, rgba(255, 255, 255, 0.15) 75%, transparent 75%, transparent);
  background-image: -o-linear-gradient(45deg, rgba(255, 255, 255, 0.15) 25%, transparent 25%, transparent 50%, rgba(255, 255, 255, 0.15) 50%, rgba(255, 255, 255, 0.15) 75%, transparent 75%, transparent);
  background-image: linear-gradient(45deg, rgba(255, 255, 255, 0.15) 25%, transparent 25%, transparent 50%, rgba(255, 255, 255, 0.15) 50%, rgba(255, 255, 255, 0.15) 75%, transparent 75%, transparent);
}
.progress-bar-info {
  background-color: #5bc0de;
}
.progress-striped .progress-bar-info {
  background-image: -webkit-linear-gradient(45deg, rgba(255, 255, 255, 0.15) 25%, transparent 25%, transparent 50%, rgba(255, 255, 255, 0.15) 50%, rgba(255, 255, 255, 0.15) 75%, transparent 75%, transparent);
  background-image: -o-linear-gradient(45deg, rgba(255, 255, 255, 0.15) 25%, transparent 25%, transparent 50%, rgba(255, 255, 255, 0.15) 50%, rgba(255, 255, 255, 0.15) 75%, transparent 75%, transparent);
  background-image: linear-gradient(45deg, rgba(255, 255, 255, 0.15) 25%, transparent 25%, transparent 50%, rgba(255, 255, 255, 0.15) 50%, rgba(255, 255, 255, 0.15) 75%, transparent 75%, transparent);
}
.progress-bar-warning {
  background-color: #f0ad4e;
}
.progress-striped .progress-bar-warning {
  background-image: -webkit-linear-gradient(45deg, rgba(255, 255, 255, 0.15) 25%, transparent 25%, transparent 50%, rgba(255, 255, 255, 0.15) 50%, rgba(255, 255, 255, 0.15) 75%, transparent 75%, transparent);
  background-image: -o-linear-gradient(45deg, rgba(255, 255, 255, 0.15) 25%, transparent 25%, transparent 50%, rgba(255, 255, 255, 0.15) 50%, rgba(255, 255, 255, 0.15) 75%, transparent 75%, transparent);
  background-image: linear-gradient(45deg, rgba(255, 255, 255, 0.15) 25%, transparent 25%, transparent 50%, rgba(255, 255, 255, 0.15) 50%, rgba(255, 255, 255, 0.15) 75%, transparent 75%, transparent);
}
.progress-bar-danger {
  background-color: #d9534f;
}
.progress-striped .progress-bar-danger {
  background-image: -webkit-linear-gradient(45deg, rgba(255, 255, 255, 0.15) 25%, transparent 25%, transparent 50%, rgba(255, 255, 255, 0.15) 50%, rgba(255, 255, 255, 0.15) 75%, transparent 75%, transparent);
  background-image: -o-linear-gradient(45deg, rgba(255, 255, 255, 0.15) 25%, transparent 25%, transparent 50%, rgba(255, 255, 255, 0.15) 50%, rgba(255, 255, 255, 0.15) 75%, transparent 75%, transparent);
  background-image: linear-gradient(45deg, rgba(255, 255, 255, 0.15) 25%, transparent 25%, transparent 50%, rgba(255, 255, 255, 0.15) 50%, rgba(255, 255, 255, 0.15) 75%, transparent 75%, transparent);
}
.media {
  margin-top: 15px;
}
.media:first-child {
  margin-top: 0;
}
.media,
.media-body {
  zoom: 1;
  overflow: hidden;
}
.media-body {
  width: 10000px;
}
.media-object {
  display: block;
}
.media-object.img-thumbnail {
  max-width: none;
}
.media-right,
.media > .pull-right {
  padding-left: 10px;
}
.media-left,
.media > .pull-left {
  padding-right: 10px;
}
.media-left,
.media-right,
.media-body {
  display: table-cell;
  vertical-align: top;
}
.media-middle {
  vertical-align: middle;
}
.media-bottom {
  vertical-align: bottom;
}
.media-heading {
  margin-top: 0;
  margin-bottom: 5px;
}
.media-list {
  padding-left: 0;
  list-style: none;
}
.list-group {
  margin-bottom: 20px;
  padding-left: 0;
}
.list-group-item {
  position: relative;
  display: block;
  padding: 10px 15px;
  margin-bottom: -1px;
  background-color: #fff;
  border: 1px solid #ddd;
}
.list-group-item:first-child {
  border-top-right-radius: 2px;
  border-top-left-radius: 2px;
}
.list-group-item:last-child {
  margin-bottom: 0;
  border-bottom-right-radius: 2px;
  border-bottom-left-radius: 2px;
}
a.list-group-item,
button.list-group-item {
  color: #555;
}
a.list-group-item .list-group-item-heading,
button.list-group-item .list-group-item-heading {
  color: #333;
}
a.list-group-item:hover,
button.list-group-item:hover,
a.list-group-item:focus,
button.list-group-item:focus {
  text-decoration: none;
  color: #555;
  background-color: #f5f5f5;
}
button.list-group-item {
  width: 100%;
  text-align: left;
}
.list-group-item.disabled,
.list-group-item.disabled:hover,
.list-group-item.disabled:focus {
  background-color: #eeeeee;
  color: #777777;
  cursor: not-allowed;
}
.list-group-item.disabled .list-group-item-heading,
.list-group-item.disabled:hover .list-group-item-heading,
.list-group-item.disabled:focus .list-group-item-heading {
  color: inherit;
}
.list-group-item.disabled .list-group-item-text,
.list-group-item.disabled:hover .list-group-item-text,
.list-group-item.disabled:focus .list-group-item-text {
  color: #777777;
}
.list-group-item.active,
.list-group-item.active:hover,
.list-group-item.active:focus {
  z-index: 2;
  color: #fff;
  background-color: #337ab7;
  border-color: #337ab7;
}
.list-group-item.active .list-group-item-heading,
.list-group-item.active:hover .list-group-item-heading,
.list-group-item.active:focus .list-group-item-heading,
.list-group-item.active .list-group-item-heading > small,
.list-group-item.active:hover .list-group-item-heading > small,
.list-group-item.active:focus .list-group-item-heading > small,
.list-group-item.active .list-group-item-heading > .small,
.list-group-item.active:hover .list-group-item-heading > .small,
.list-group-item.active:focus .list-group-item-heading > .small {
  color: inherit;
}
.list-group-item.active .list-group-item-text,
.list-group-item.active:hover .list-group-item-text,
.list-group-item.active:focus .list-group-item-text {
  color: #c7ddef;
}
.list-group-item-success {
  color: #3c763d;
  background-color: #dff0d8;
}
a.list-group-item-success,
button.list-group-item-success {
  color: #3c763d;
}
a.list-group-item-success .list-group-item-heading,
button.list-group-item-success .list-group-item-heading {
  color: inherit;
}
a.list-group-item-success:hover,
button.list-group-item-success:hover,
a.list-group-item-success:focus,
button.list-group-item-success:focus {
  color: #3c763d;
  background-color: #d0e9c6;
}
a.list-group-item-success.active,
button.list-group-item-success.active,
a.list-group-item-success.active:hover,
button.list-group-item-success.active:hover,
a.list-group-item-success.active:focus,
button.list-group-item-success.active:focus {
  color: #fff;
  background-color: #3c763d;
  border-color: #3c763d;
}
.list-group-item-info {
  color: #31708f;
  background-color: #d9edf7;
}
a.list-group-item-info,
button.list-group-item-info {
  color: #31708f;
}
a.list-group-item-info .list-group-item-heading,
button.list-group-item-info .list-group-item-heading {
  color: inherit;
}
a.list-group-item-info:hover,
button.list-group-item-info:hover,
a.list-group-item-info:focus,
button.list-group-item-info:focus {
  color: #31708f;
  background-color: #c4e3f3;
}
a.list-group-item-info.active,
button.list-group-item-info.active,
a.list-group-item-info.active:hover,
button.list-group-item-info.active:hover,
a.list-group-item-info.active:focus,
button.list-group-item-info.active:focus {
  color: #fff;
  background-color: #31708f;
  border-color: #31708f;
}
.list-group-item-warning {
  color: #8a6d3b;
  background-color: #fcf8e3;
}
a.list-group-item-warning,
button.list-group-item-warning {
  color: #8a6d3b;
}
a.list-group-item-warning .list-group-item-heading,
button.list-group-item-warning .list-group-item-heading {
  color: inherit;
}
a.list-group-item-warning:hover,
button.list-group-item-warning:hover,
a.list-group-item-warning:focus,
button.list-group-item-warning:focus {
  color: #8a6d3b;
  background-color: #faf2cc;
}
a.list-group-item-warning.active,
button.list-group-item-warning.active,
a.list-group-item-warning.active:hover,
button.list-group-item-warning.active:hover,
a.list-group-item-warning.active:focus,
button.list-group-item-warning.active:focus {
  color: #fff;
  background-color: #8a6d3b;
  border-color: #8a6d3b;
}
.list-group-item-danger {
  color: #a94442;
  background-color: #f2dede;
}
a.list-group-item-danger,
button.list-group-item-danger {
  color: #a94442;
}
a.list-group-item-danger .list-group-item-heading,
button.list-group-item-danger .list-group-item-heading {
  color: inherit;
}
a.list-group-item-danger:hover,
button.list-group-item-danger:hover,
a.list-group-item-danger:focus,
button.list-group-item-danger:focus {
  color: #a94442;
  background-color: #ebcccc;
}
a.list-group-item-danger.active,
button.list-group-item-danger.active,
a.list-group-item-danger.active:hover,
button.list-group-item-danger.active:hover,
a.list-group-item-danger.active:focus,
button.list-group-item-danger.active:focus {
  color: #fff;
  background-color: #a94442;
  border-color: #a94442;
}
.list-group-item-heading {
  margin-top: 0;
  margin-bottom: 5px;
}
.list-group-item-text {
  margin-bottom: 0;
  line-height: 1.3;
}
.panel {
  margin-bottom: 18px;
  background-color: #fff;
  border: 1px solid transparent;
  border-radius: 2px;
  -webkit-box-shadow: 0 1px 1px rgba(0, 0, 0, 0.05);
  box-shadow: 0 1px 1px rgba(0, 0, 0, 0.05);
}
.panel-body {
  padding: 15px;
}
.panel-heading {
  padding: 10px 15px;
  border-bottom: 1px solid transparent;
  border-top-right-radius: 1px;
  border-top-left-radius: 1px;
}
.panel-heading > .dropdown .dropdown-toggle {
  color: inherit;
}
.panel-title {
  margin-top: 0;
  margin-bottom: 0;
  font-size: 15px;
  color: inherit;
}
.panel-title > a,
.panel-title > small,
.panel-title > .small,
.panel-title > small > a,
.panel-title > .small > a {
  color: inherit;
}
.panel-footer {
  padding: 10px 15px;
  background-color: #f5f5f5;
  border-top: 1px solid #ddd;
  border-bottom-right-radius: 1px;
  border-bottom-left-radius: 1px;
}
.panel > .list-group,
.panel > .panel-collapse > .list-group {
  margin-bottom: 0;
}
.panel > .list-group .list-group-item,
.panel > .panel-collapse > .list-group .list-group-item {
  border-width: 1px 0;
  border-radius: 0;
}
.panel > .list-group:first-child .list-group-item:first-child,
.panel > .panel-collapse > .list-group:first-child .list-group-item:first-child {
  border-top: 0;
  border-top-right-radius: 1px;
  border-top-left-radius: 1px;
}
.panel > .list-group:last-child .list-group-item:last-child,
.panel > .panel-collapse > .list-group:last-child .list-group-item:last-child {
  border-bottom: 0;
  border-bottom-right-radius: 1px;
  border-bottom-left-radius: 1px;
}
.panel > .panel-heading + .panel-collapse > .list-group .list-group-item:first-child {
  border-top-right-radius: 0;
  border-top-left-radius: 0;
}
.panel-heading + .list-group .list-group-item:first-child {
  border-top-width: 0;
}
.list-group + .panel-footer {
  border-top-width: 0;
}
.panel > .table,
.panel > .table-responsive > .table,
.panel > .panel-collapse > .table {
  margin-bottom: 0;
}
.panel > .table caption,
.panel > .table-responsive > .table caption,
.panel > .panel-collapse > .table caption {
  padding-left: 15px;
  padding-right: 15px;
}
.panel > .table:first-child,
.panel > .table-responsive:first-child > .table:first-child {
  border-top-right-radius: 1px;
  border-top-left-radius: 1px;
}
.panel > .table:first-child > thead:first-child > tr:first-child,
.panel > .table-responsive:first-child > .table:first-child > thead:first-child > tr:first-child,
.panel > .table:first-child > tbody:first-child > tr:first-child,
.panel > .table-responsive:first-child > .table:first-child > tbody:first-child > tr:first-child {
  border-top-left-radius: 1px;
  border-top-right-radius: 1px;
}
.panel > .table:first-child > thead:first-child > tr:first-child td:first-child,
.panel > .table-responsive:first-child > .table:first-child > thead:first-child > tr:first-child td:first-child,
.panel > .table:first-child > tbody:first-child > tr:first-child td:first-child,
.panel > .table-responsive:first-child > .table:first-child > tbody:first-child > tr:first-child td:first-child,
.panel > .table:first-child > thead:first-child > tr:first-child th:first-child,
.panel > .table-responsive:first-child > .table:first-child > thead:first-child > tr:first-child th:first-child,
.panel > .table:first-child > tbody:first-child > tr:first-child th:first-child,
.panel > .table-responsive:first-child > .table:first-child > tbody:first-child > tr:first-child th:first-child {
  border-top-left-radius: 1px;
}
.panel > .table:first-child > thead:first-child > tr:first-child td:last-child,
.panel > .table-responsive:first-child > .table:first-child > thead:first-child > tr:first-child td:last-child,
.panel > .table:first-child > tbody:first-child > tr:first-child td:last-child,
.panel > .table-responsive:first-child > .table:first-child > tbody:first-child > tr:first-child td:last-child,
.panel > .table:first-child > thead:first-child > tr:first-child th:last-child,
.panel > .table-responsive:first-child > .table:first-child > thead:first-child > tr:first-child th:last-child,
.panel > .table:first-child > tbody:first-child > tr:first-child th:last-child,
.panel > .table-responsive:first-child > .table:first-child > tbody:first-child > tr:first-child th:last-child {
  border-top-right-radius: 1px;
}
.panel > .table:last-child,
.panel > .table-responsive:last-child > .table:last-child {
  border-bottom-right-radius: 1px;
  border-bottom-left-radius: 1px;
}
.panel > .table:last-child > tbody:last-child > tr:last-child,
.panel > .table-responsive:last-child > .table:last-child > tbody:last-child > tr:last-child,
.panel > .table:last-child > tfoot:last-child > tr:last-child,
.panel > .table-responsive:last-child > .table:last-child > tfoot:last-child > tr:last-child {
  border-bottom-left-radius: 1px;
  border-bottom-right-radius: 1px;
}
.panel > .table:last-child > tbody:last-child > tr:last-child td:first-child,
.panel > .table-responsive:last-child > .table:last-child > tbody:last-child > tr:last-child td:first-child,
.panel > .table:last-child > tfoot:last-child > tr:last-child td:first-child,
.panel > .table-responsive:last-child > .table:last-child > tfoot:last-child > tr:last-child td:first-child,
.panel > .table:last-child > tbody:last-child > tr:last-child th:first-child,
.panel > .table-responsive:last-child > .table:last-child > tbody:last-child > tr:last-child th:first-child,
.panel > .table:last-child > tfoot:last-child > tr:last-child th:first-child,
.panel > .table-responsive:last-child > .table:last-child > tfoot:last-child > tr:last-child th:first-child {
  border-bottom-left-radius: 1px;
}
.panel > .table:last-child > tbody:last-child > tr:last-child td:last-child,
.panel > .table-responsive:last-child > .table:last-child > tbody:last-child > tr:last-child td:last-child,
.panel > .table:last-child > tfoot:last-child > tr:last-child td:last-child,
.panel > .table-responsive:last-child > .table:last-child > tfoot:last-child > tr:last-child td:last-child,
.panel > .table:last-child > tbody:last-child > tr:last-child th:last-child,
.panel > .table-responsive:last-child > .table:last-child > tbody:last-child > tr:last-child th:last-child,
.panel > .table:last-child > tfoot:last-child > tr:last-child th:last-child,
.panel > .table-responsive:last-child > .table:last-child > tfoot:last-child > tr:last-child th:last-child {
  border-bottom-right-radius: 1px;
}
.panel > .panel-body + .table,
.panel > .panel-body + .table-responsive,
.panel > .table + .panel-body,
.panel > .table-responsive + .panel-body {
  border-top: 1px solid #ddd;
}
.panel > .table > tbody:first-child > tr:first-child th,
.panel > .table > tbody:first-child > tr:first-child td {
  border-top: 0;
}
.panel > .table-bordered,
.panel > .table-responsive > .table-bordered {
  border: 0;
}
.panel > .table-bordered > thead > tr > th:first-child,
.panel > .table-responsive > .table-bordered > thead > tr > th:first-child,
.panel > .table-bordered > tbody > tr > th:first-child,
.panel > .table-responsive > .table-bordered > tbody > tr > th:first-child,
.panel > .table-bordered > tfoot > tr > th:first-child,
.panel > .table-responsive > .table-bordered > tfoot > tr > th:first-child,
.panel > .table-bordered > thead > tr > td:first-child,
.panel > .table-responsive > .table-bordered > thead > tr > td:first-child,
.panel > .table-bordered > tbody > tr > td:first-child,
.panel > .table-responsive > .table-bordered > tbody > tr > td:first-child,
.panel > .table-bordered > tfoot > tr > td:first-child,
.panel > .table-responsive > .table-bordered > tfoot > tr > td:first-child {
  border-left: 0;
}
.panel > .table-bordered > thead > tr > th:last-child,
.panel > .table-responsive > .table-bordered > thead > tr > th:last-child,
.panel > .table-bordered > tbody > tr > th:last-child,
.panel > .table-responsive > .table-bordered > tbody > tr > th:last-child,
.panel > .table-bordered > tfoot > tr > th:last-child,
.panel > .table-responsive > .table-bordered > tfoot > tr > th:last-child,
.panel > .table-bordered > thead > tr > td:last-child,
.panel > .table-responsive > .table-bordered > thead > tr > td:last-child,
.panel > .table-bordered > tbody > tr > td:last-child,
.panel > .table-responsive > .table-bordered > tbody > tr > td:last-child,
.panel > .table-bordered > tfoot > tr > td:last-child,
.panel > .table-responsive > .table-bordered > tfoot > tr > td:last-child {
  border-right: 0;
}
.panel > .table-bordered > thead > tr:first-child > td,
.panel > .table-responsive > .table-bordered > thead > tr:first-child > td,
.panel > .table-bordered > tbody > tr:first-child > td,
.panel > .table-responsive > .table-bordered > tbody > tr:first-child > td,
.panel > .table-bordered > thead > tr:first-child > th,
.panel > .table-responsive > .table-bordered > thead > tr:first-child > th,
.panel > .table-bordered > tbody > tr:first-child > th,
.panel > .table-responsive > .table-bordered > tbody > tr:first-child > th {
  border-bottom: 0;
}
.panel > .table-bordered > tbody > tr:last-child > td,
.panel > .table-responsive > .table-bordered > tbody > tr:last-child > td,
.panel > .table-bordered > tfoot > tr:last-child > td,
.panel > .table-responsive > .table-bordered > tfoot > tr:last-child > td,
.panel > .table-bordered > tbody > tr:last-child > th,
.panel > .table-responsive > .table-bordered > tbody > tr:last-child > th,
.panel > .table-bordered > tfoot > tr:last-child > th,
.panel > .table-responsive > .table-bordered > tfoot > tr:last-child > th {
  border-bottom: 0;
}
.panel > .table-responsive {
  border: 0;
  margin-bottom: 0;
}
.panel-group {
  margin-bottom: 18px;
}
.panel-group .panel {
  margin-bottom: 0;
  border-radius: 2px;
}
.panel-group .panel + .panel {
  margin-top: 5px;
}
.panel-group .panel-heading {
  border-bottom: 0;
}
.panel-group .panel-heading + .panel-collapse > .panel-body,
.panel-group .panel-heading + .panel-collapse > .list-group {
  border-top: 1px solid #ddd;
}
.panel-group .panel-footer {
  border-top: 0;
}
.panel-group .panel-footer + .panel-collapse .panel-body {
  border-bottom: 1px solid #ddd;
}
.panel-default {
  border-color: #ddd;
}
.panel-default > .panel-heading {
  color: #333333;
  background-color: #f5f5f5;
  border-color: #ddd;
}
.panel-default > .panel-heading + .panel-collapse > .panel-body {
  border-top-color: #ddd;
}
.panel-default > .panel-heading .badge {
  color: #f5f5f5;
  background-color: #333333;
}
.panel-default > .panel-footer + .panel-collapse > .panel-body {
  border-bottom-color: #ddd;
}
.panel-primary {
  border-color: #337ab7;
}
.panel-primary > .panel-heading {
  color: #fff;
  background-color: #337ab7;
  border-color: #337ab7;
}
.panel-primary > .panel-heading + .panel-collapse > .panel-body {
  border-top-color: #337ab7;
}
.panel-primary > .panel-heading .badge {
  color: #337ab7;
  background-color: #fff;
}
.panel-primary > .panel-footer + .panel-collapse > .panel-body {
  border-bottom-color: #337ab7;
}
.panel-success {
  border-color: #d6e9c6;
}
.panel-success > .panel-heading {
  color: #3c763d;
  background-color: #dff0d8;
  border-color: #d6e9c6;
}
.panel-success > .panel-heading + .panel-collapse > .panel-body {
  border-top-color: #d6e9c6;
}
.panel-success > .panel-heading .badge {
  color: #dff0d8;
  background-color: #3c763d;
}
.panel-success > .panel-footer + .panel-collapse > .panel-body {
  border-bottom-color: #d6e9c6;
}
.panel-info {
  border-color: #bce8f1;
}
.panel-info > .panel-heading {
  color: #31708f;
  background-color: #d9edf7;
  border-color: #bce8f1;
}
.panel-info > .panel-heading + .panel-collapse > .panel-body {
  border-top-color: #bce8f1;
}
.panel-info > .panel-heading .badge {
  color: #d9edf7;
  background-color: #31708f;
}
.panel-info > .panel-footer + .panel-collapse > .panel-body {
  border-bottom-color: #bce8f1;
}
.panel-warning {
  border-color: #faebcc;
}
.panel-warning > .panel-heading {
  color: #8a6d3b;
  background-color: #fcf8e3;
  border-color: #faebcc;
}
.panel-warning > .panel-heading + .panel-collapse > .panel-body {
  border-top-color: #faebcc;
}
.panel-warning > .panel-heading .badge {
  color: #fcf8e3;
  background-color: #8a6d3b;
}
.panel-warning > .panel-footer + .panel-collapse > .panel-body {
  border-bottom-color: #faebcc;
}
.panel-danger {
  border-color: #ebccd1;
}
.panel-danger > .panel-heading {
  color: #a94442;
  background-color: #f2dede;
  border-color: #ebccd1;
}
.panel-danger > .panel-heading + .panel-collapse > .panel-body {
  border-top-color: #ebccd1;
}
.panel-danger > .panel-heading .badge {
  color: #f2dede;
  background-color: #a94442;
}
.panel-danger > .panel-footer + .panel-collapse > .panel-body {
  border-bottom-color: #ebccd1;
}
.embed-responsive {
  position: relative;
  display: block;
  height: 0;
  padding: 0;
  overflow: hidden;
}
.embed-responsive .embed-responsive-item,
.embed-responsive iframe,
.embed-responsive embed,
.embed-responsive object,
.embed-responsive video {
  position: absolute;
  top: 0;
  left: 0;
  bottom: 0;
  height: 100%;
  width: 100%;
  border: 0;
}
.embed-responsive-16by9 {
  padding-bottom: 56.25%;
}
.embed-responsive-4by3 {
  padding-bottom: 75%;
}
.well {
  min-height: 20px;
  padding: 19px;
  margin-bottom: 20px;
  background-color: #f5f5f5;
  border: 1px solid #e3e3e3;
  border-radius: 2px;
  -webkit-box-shadow: inset 0 1px 1px rgba(0, 0, 0, 0.05);
  box-shadow: inset 0 1px 1px rgba(0, 0, 0, 0.05);
}
.well blockquote {
  border-color: #ddd;
  border-color: rgba(0, 0, 0, 0.15);
}
.well-lg {
  padding: 24px;
  border-radius: 3px;
}
.well-sm {
  padding: 9px;
  border-radius: 1px;
}
.close {
  float: right;
  font-size: 19.5px;
  font-weight: bold;
  line-height: 1;
  color: #000;
  text-shadow: 0 1px 0 #fff;
  opacity: 0.2;
  filter: alpha(opacity=20);
}
.close:hover,
.close:focus {
  color: #000;
  text-decoration: none;
  cursor: pointer;
  opacity: 0.5;
  filter: alpha(opacity=50);
}
button.close {
  padding: 0;
  cursor: pointer;
  background: transparent;
  border: 0;
  -webkit-appearance: none;
}
.modal-open {
  overflow: hidden;
}
.modal {
  display: none;
  overflow: hidden;
  position: fixed;
  top: 0;
  right: 0;
  bottom: 0;
  left: 0;
  z-index: 1050;
  -webkit-overflow-scrolling: touch;
  outline: 0;
}
.modal.fade .modal-dialog {
  -webkit-transform: translate(0, -25%);
  -ms-transform: translate(0, -25%);
  -o-transform: translate(0, -25%);
  transform: translate(0, -25%);
  -webkit-transition: -webkit-transform 0.3s ease-out;
  -moz-transition: -moz-transform 0.3s ease-out;
  -o-transition: -o-transform 0.3s ease-out;
  transition: transform 0.3s ease-out;
}
.modal.in .modal-dialog {
  -webkit-transform: translate(0, 0);
  -ms-transform: translate(0, 0);
  -o-transform: translate(0, 0);
  transform: translate(0, 0);
}
.modal-open .modal {
  overflow-x: hidden;
  overflow-y: auto;
}
.modal-dialog {
  position: relative;
  width: auto;
  margin: 10px;
}
.modal-content {
  position: relative;
  background-color: #fff;
  border: 1px solid #999;
  border: 1px solid rgba(0, 0, 0, 0.2);
  border-radius: 3px;
  -webkit-box-shadow: 0 3px 9px rgba(0, 0, 0, 0.5);
  box-shadow: 0 3px 9px rgba(0, 0, 0, 0.5);
  background-clip: padding-box;
  outline: 0;
}
.modal-backdrop {
  position: fixed;
  top: 0;
  right: 0;
  bottom: 0;
  left: 0;
  z-index: 1040;
  background-color: #000;
}
.modal-backdrop.fade {
  opacity: 0;
  filter: alpha(opacity=0);
}
.modal-backdrop.in {
  opacity: 0.5;
  filter: alpha(opacity=50);
}
.modal-header {
  padding: 15px;
  border-bottom: 1px solid #e5e5e5;
}
.modal-header .close {
  margin-top: -2px;
}
.modal-title {
  margin: 0;
  line-height: 1.42857143;
}
.modal-body {
  position: relative;
  padding: 15px;
}
.modal-footer {
  padding: 15px;
  text-align: right;
  border-top: 1px solid #e5e5e5;
}
.modal-footer .btn + .btn {
  margin-left: 5px;
  margin-bottom: 0;
}
.modal-footer .btn-group .btn + .btn {
  margin-left: -1px;
}
.modal-footer .btn-block + .btn-block {
  margin-left: 0;
}
.modal-scrollbar-measure {
  position: absolute;
  top: -9999px;
  width: 50px;
  height: 50px;
  overflow: scroll;
}
@media (min-width: 768px) {
  .modal-dialog {
    width: 600px;
    margin: 30px auto;
  }
  .modal-content {
    -webkit-box-shadow: 0 5px 15px rgba(0, 0, 0, 0.5);
    box-shadow: 0 5px 15px rgba(0, 0, 0, 0.5);
  }
  .modal-sm {
    width: 300px;
  }
}
@media (min-width: 992px) {
  .modal-lg {
    width: 900px;
  }
}
.tooltip {
  position: absolute;
  z-index: 1070;
  display: block;
  font-family: "Helvetica Neue", Helvetica, Arial, sans-serif;
  font-style: normal;
  font-weight: normal;
  letter-spacing: normal;
  line-break: auto;
  line-height: 1.42857143;
  text-align: left;
  text-align: start;
  text-decoration: none;
  text-shadow: none;
  text-transform: none;
  white-space: normal;
  word-break: normal;
  word-spacing: normal;
  word-wrap: normal;
  font-size: 12px;
  opacity: 0;
  filter: alpha(opacity=0);
}
.tooltip.in {
  opacity: 0.9;
  filter: alpha(opacity=90);
}
.tooltip.top {
  margin-top: -3px;
  padding: 5px 0;
}
.tooltip.right {
  margin-left: 3px;
  padding: 0 5px;
}
.tooltip.bottom {
  margin-top: 3px;
  padding: 5px 0;
}
.tooltip.left {
  margin-left: -3px;
  padding: 0 5px;
}
.tooltip-inner {
  max-width: 200px;
  padding: 3px 8px;
  color: #fff;
  text-align: center;
  background-color: #000;
  border-radius: 2px;
}
.tooltip-arrow {
  position: absolute;
  width: 0;
  height: 0;
  border-color: transparent;
  border-style: solid;
}
.tooltip.top .tooltip-arrow {
  bottom: 0;
  left: 50%;
  margin-left: -5px;
  border-width: 5px 5px 0;
  border-top-color: #000;
}
.tooltip.top-left .tooltip-arrow {
  bottom: 0;
  right: 5px;
  margin-bottom: -5px;
  border-width: 5px 5px 0;
  border-top-color: #000;
}
.tooltip.top-right .tooltip-arrow {
  bottom: 0;
  left: 5px;
  margin-bottom: -5px;
  border-width: 5px 5px 0;
  border-top-color: #000;
}
.tooltip.right .tooltip-arrow {
  top: 50%;
  left: 0;
  margin-top: -5px;
  border-width: 5px 5px 5px 0;
  border-right-color: #000;
}
.tooltip.left .tooltip-arrow {
  top: 50%;
  right: 0;
  margin-top: -5px;
  border-width: 5px 0 5px 5px;
  border-left-color: #000;
}
.tooltip.bottom .tooltip-arrow {
  top: 0;
  left: 50%;
  margin-left: -5px;
  border-width: 0 5px 5px;
  border-bottom-color: #000;
}
.tooltip.bottom-left .tooltip-arrow {
  top: 0;
  right: 5px;
  margin-top: -5px;
  border-width: 0 5px 5px;
  border-bottom-color: #000;
}
.tooltip.bottom-right .tooltip-arrow {
  top: 0;
  left: 5px;
  margin-top: -5px;
  border-width: 0 5px 5px;
  border-bottom-color: #000;
}
.popover {
  position: absolute;
  top: 0;
  left: 0;
  z-index: 1060;
  display: none;
  max-width: 276px;
  padding: 1px;
  font-family: "Helvetica Neue", Helvetica, Arial, sans-serif;
  font-style: normal;
  font-weight: normal;
  letter-spacing: normal;
  line-break: auto;
  line-height: 1.42857143;
  text-align: left;
  text-align: start;
  text-decoration: none;
  text-shadow: none;
  text-transform: none;
  white-space: normal;
  word-break: normal;
  word-spacing: normal;
  word-wrap: normal;
  font-size: 13px;
  background-color: #fff;
  background-clip: padding-box;
  border: 1px solid #ccc;
  border: 1px solid rgba(0, 0, 0, 0.2);
  border-radius: 3px;
  -webkit-box-shadow: 0 5px 10px rgba(0, 0, 0, 0.2);
  box-shadow: 0 5px 10px rgba(0, 0, 0, 0.2);
}
.popover.top {
  margin-top: -10px;
}
.popover.right {
  margin-left: 10px;
}
.popover.bottom {
  margin-top: 10px;
}
.popover.left {
  margin-left: -10px;
}
.popover-title {
  margin: 0;
  padding: 8px 14px;
  font-size: 13px;
  background-color: #f7f7f7;
  border-bottom: 1px solid #ebebeb;
  border-radius: 2px 2px 0 0;
}
.popover-content {
  padding: 9px 14px;
}
.popover > .arrow,
.popover > .arrow:after {
  position: absolute;
  display: block;
  width: 0;
  height: 0;
  border-color: transparent;
  border-style: solid;
}
.popover > .arrow {
  border-width: 11px;
}
.popover > .arrow:after {
  border-width: 10px;
  content: "";
}
.popover.top > .arrow {
  left: 50%;
  margin-left: -11px;
  border-bottom-width: 0;
  border-top-color: #999999;
  border-top-color: rgba(0, 0, 0, 0.25);
  bottom: -11px;
}
.popover.top > .arrow:after {
  content: " ";
  bottom: 1px;
  margin-left: -10px;
  border-bottom-width: 0;
  border-top-color: #fff;
}
.popover.right > .arrow {
  top: 50%;
  left: -11px;
  margin-top: -11px;
  border-left-width: 0;
  border-right-color: #999999;
  border-right-color: rgba(0, 0, 0, 0.25);
}
.popover.right > .arrow:after {
  content: " ";
  left: 1px;
  bottom: -10px;
  border-left-width: 0;
  border-right-color: #fff;
}
.popover.bottom > .arrow {
  left: 50%;
  margin-left: -11px;
  border-top-width: 0;
  border-bottom-color: #999999;
  border-bottom-color: rgba(0, 0, 0, 0.25);
  top: -11px;
}
.popover.bottom > .arrow:after {
  content: " ";
  top: 1px;
  margin-left: -10px;
  border-top-width: 0;
  border-bottom-color: #fff;
}
.popover.left > .arrow {
  top: 50%;
  right: -11px;
  margin-top: -11px;
  border-right-width: 0;
  border-left-color: #999999;
  border-left-color: rgba(0, 0, 0, 0.25);
}
.popover.left > .arrow:after {
  content: " ";
  right: 1px;
  border-right-width: 0;
  border-left-color: #fff;
  bottom: -10px;
}
.carousel {
  position: relative;
}
.carousel-inner {
  position: relative;
  overflow: hidden;
  width: 100%;
}
.carousel-inner > .item {
  display: none;
  position: relative;
  -webkit-transition: 0.6s ease-in-out left;
  -o-transition: 0.6s ease-in-out left;
  transition: 0.6s ease-in-out left;
}
.carousel-inner > .item > img,
.carousel-inner > .item > a > img {
  line-height: 1;
}
@media all and (transform-3d), (-webkit-transform-3d) {
  .carousel-inner > .item {
    -webkit-transition: -webkit-transform 0.6s ease-in-out;
    -moz-transition: -moz-transform 0.6s ease-in-out;
    -o-transition: -o-transform 0.6s ease-in-out;
    transition: transform 0.6s ease-in-out;
    -webkit-backface-visibility: hidden;
    -moz-backface-visibility: hidden;
    backface-visibility: hidden;
    -webkit-perspective: 1000px;
    -moz-perspective: 1000px;
    perspective: 1000px;
  }
  .carousel-inner > .item.next,
  .carousel-inner > .item.active.right {
    -webkit-transform: translate3d(100%, 0, 0);
    transform: translate3d(100%, 0, 0);
    left: 0;
  }
  .carousel-inner > .item.prev,
  .carousel-inner > .item.active.left {
    -webkit-transform: translate3d(-100%, 0, 0);
    transform: translate3d(-100%, 0, 0);
    left: 0;
  }
  .carousel-inner > .item.next.left,
  .carousel-inner > .item.prev.right,
  .carousel-inner > .item.active {
    -webkit-transform: translate3d(0, 0, 0);
    transform: translate3d(0, 0, 0);
    left: 0;
  }
}
.carousel-inner > .active,
.carousel-inner > .next,
.carousel-inner > .prev {
  display: block;
}
.carousel-inner > .active {
  left: 0;
}
.carousel-inner > .next,
.carousel-inner > .prev {
  position: absolute;
  top: 0;
  width: 100%;
}
.carousel-inner > .next {
  left: 100%;
}
.carousel-inner > .prev {
  left: -100%;
}
.carousel-inner > .next.left,
.carousel-inner > .prev.right {
  left: 0;
}
.carousel-inner > .active.left {
  left: -100%;
}
.carousel-inner > .active.right {
  left: 100%;
}
.carousel-control {
  position: absolute;
  top: 0;
  left: 0;
  bottom: 0;
  width: 15%;
  opacity: 0.5;
  filter: alpha(opacity=50);
  font-size: 20px;
  color: #fff;
  text-align: center;
  text-shadow: 0 1px 2px rgba(0, 0, 0, 0.6);
  background-color: rgba(0, 0, 0, 0);
}
.carousel-control.left {
  background-image: -webkit-linear-gradient(left, rgba(0, 0, 0, 0.5) 0%, rgba(0, 0, 0, 0.0001) 100%);
  background-image: -o-linear-gradient(left, rgba(0, 0, 0, 0.5) 0%, rgba(0, 0, 0, 0.0001) 100%);
  background-image: linear-gradient(to right, rgba(0, 0, 0, 0.5) 0%, rgba(0, 0, 0, 0.0001) 100%);
  background-repeat: repeat-x;
  filter: progid:DXImageTransform.Microsoft.gradient(startColorstr='#80000000', endColorstr='#00000000', GradientType=1);
}
.carousel-control.right {
  left: auto;
  right: 0;
  background-image: -webkit-linear-gradient(left, rgba(0, 0, 0, 0.0001) 0%, rgba(0, 0, 0, 0.5) 100%);
  background-image: -o-linear-gradient(left, rgba(0, 0, 0, 0.0001) 0%, rgba(0, 0, 0, 0.5) 100%);
  background-image: linear-gradient(to right, rgba(0, 0, 0, 0.0001) 0%, rgba(0, 0, 0, 0.5) 100%);
  background-repeat: repeat-x;
  filter: progid:DXImageTransform.Microsoft.gradient(startColorstr='#00000000', endColorstr='#80000000', GradientType=1);
}
.carousel-control:hover,
.carousel-control:focus {
  outline: 0;
  color: #fff;
  text-decoration: none;
  opacity: 0.9;
  filter: alpha(opacity=90);
}
.carousel-control .icon-prev,
.carousel-control .icon-next,
.carousel-control .glyphicon-chevron-left,
.carousel-control .glyphicon-chevron-right {
  position: absolute;
  top: 50%;
  margin-top: -10px;
  z-index: 5;
  display: inline-block;
}
.carousel-control .icon-prev,
.carousel-control .glyphicon-chevron-left {
  left: 50%;
  margin-left: -10px;
}
.carousel-control .icon-next,
.carousel-control .glyphicon-chevron-right {
  right: 50%;
  margin-right: -10px;
}
.carousel-control .icon-prev,
.carousel-control .icon-next {
  width: 20px;
  height: 20px;
  line-height: 1;
  font-family: serif;
}
.carousel-control .icon-prev:before {
  content: '\2039';
}
.carousel-control .icon-next:before {
  content: '\203a';
}
.carousel-indicators {
  position: absolute;
  bottom: 10px;
  left: 50%;
  z-index: 15;
  width: 60%;
  margin-left: -30%;
  padding-left: 0;
  list-style: none;
  text-align: center;
}
.carousel-indicators li {
  display: inline-block;
  width: 10px;
  height: 10px;
  margin: 1px;
  text-indent: -999px;
  border: 1px solid #fff;
  border-radius: 10px;
  cursor: pointer;
  background-color: #000 \9;
  background-color: rgba(0, 0, 0, 0);
}
.carousel-indicators .active {
  margin: 0;
  width: 12px;
  height: 12px;
  background-color: #fff;
}
.carousel-caption {
  position: absolute;
  left: 15%;
  right: 15%;
  bottom: 20px;
  z-index: 10;
  padding-top: 20px;
  padding-bottom: 20px;
  color: #fff;
  text-align: center;
  text-shadow: 0 1px 2px rgba(0, 0, 0, 0.6);
}
.carousel-caption .btn {
  text-shadow: none;
}
@media screen and (min-width: 768px) {
  .carousel-control .glyphicon-chevron-left,
  .carousel-control .glyphicon-chevron-right,
  .carousel-control .icon-prev,
  .carousel-control .icon-next {
    width: 30px;
    height: 30px;
    margin-top: -10px;
    font-size: 30px;
  }
  .carousel-control .glyphicon-chevron-left,
  .carousel-control .icon-prev {
    margin-left: -10px;
  }
  .carousel-control .glyphicon-chevron-right,
  .carousel-control .icon-next {
    margin-right: -10px;
  }
  .carousel-caption {
    left: 20%;
    right: 20%;
    padding-bottom: 30px;
  }
  .carousel-indicators {
    bottom: 20px;
  }
}
.clearfix:before,
.clearfix:after,
.dl-horizontal dd:before,
.dl-horizontal dd:after,
.container:before,
.container:after,
.container-fluid:before,
.container-fluid:after,
.row:before,
.row:after,
.form-horizontal .form-group:before,
.form-horizontal .form-group:after,
.btn-toolbar:before,
.btn-toolbar:after,
.btn-group-vertical > .btn-group:before,
.btn-group-vertical > .btn-group:after,
.nav:before,
.nav:after,
.navbar:before,
.navbar:after,
.navbar-header:before,
.navbar-header:after,
.navbar-collapse:before,
.navbar-collapse:after,
.pager:before,
.pager:after,
.panel-body:before,
.panel-body:after,
.modal-header:before,
.modal-header:after,
.modal-footer:before,
.modal-footer:after,
.item_buttons:before,
.item_buttons:after {
  content: " ";
  display: table;
}
.clearfix:after,
.dl-horizontal dd:after,
.container:after,
.container-fluid:after,
.row:after,
.form-horizontal .form-group:after,
.btn-toolbar:after,
.btn-group-vertical > .btn-group:after,
.nav:after,
.navbar:after,
.navbar-header:after,
.navbar-collapse:after,
.pager:after,
.panel-body:after,
.modal-header:after,
.modal-footer:after,
.item_buttons:after {
  clear: both;
}
.center-block {
  display: block;
  margin-left: auto;
  margin-right: auto;
}
.pull-right {
  float: right !important;
}
.pull-left {
  float: left !important;
}
.hide {
  display: none !important;
}
.show {
  display: block !important;
}
.invisible {
  visibility: hidden;
}
.text-hide {
  font: 0/0 a;
  color: transparent;
  text-shadow: none;
  background-color: transparent;
  border: 0;
}
.hidden {
  display: none !important;
}
.affix {
  position: fixed;
}
@-ms-viewport {
  width: device-width;
}
.visible-xs,
.visible-sm,
.visible-md,
.visible-lg {
  display: none !important;
}
.visible-xs-block,
.visible-xs-inline,
.visible-xs-inline-block,
.visible-sm-block,
.visible-sm-inline,
.visible-sm-inline-block,
.visible-md-block,
.visible-md-inline,
.visible-md-inline-block,
.visible-lg-block,
.visible-lg-inline,
.visible-lg-inline-block {
  display: none !important;
}
@media (max-width: 767px) {
  .visible-xs {
    display: block !important;
  }
  table.visible-xs {
    display: table !important;
  }
  tr.visible-xs {
    display: table-row !important;
  }
  th.visible-xs,
  td.visible-xs {
    display: table-cell !important;
  }
}
@media (max-width: 767px) {
  .visible-xs-block {
    display: block !important;
  }
}
@media (max-width: 767px) {
  .visible-xs-inline {
    display: inline !important;
  }
}
@media (max-width: 767px) {
  .visible-xs-inline-block {
    display: inline-block !important;
  }
}
@media (min-width: 768px) and (max-width: 991px) {
  .visible-sm {
    display: block !important;
  }
  table.visible-sm {
    display: table !important;
  }
  tr.visible-sm {
    display: table-row !important;
  }
  th.visible-sm,
  td.visible-sm {
    display: table-cell !important;
  }
}
@media (min-width: 768px) and (max-width: 991px) {
  .visible-sm-block {
    display: block !important;
  }
}
@media (min-width: 768px) and (max-width: 991px) {
  .visible-sm-inline {
    display: inline !important;
  }
}
@media (min-width: 768px) and (max-width: 991px) {
  .visible-sm-inline-block {
    display: inline-block !important;
  }
}
@media (min-width: 992px) and (max-width: 1199px) {
  .visible-md {
    display: block !important;
  }
  table.visible-md {
    display: table !important;
  }
  tr.visible-md {
    display: table-row !important;
  }
  th.visible-md,
  td.visible-md {
    display: table-cell !important;
  }
}
@media (min-width: 992px) and (max-width: 1199px) {
  .visible-md-block {
    display: block !important;
  }
}
@media (min-width: 992px) and (max-width: 1199px) {
  .visible-md-inline {
    display: inline !important;
  }
}
@media (min-width: 992px) and (max-width: 1199px) {
  .visible-md-inline-block {
    display: inline-block !important;
  }
}
@media (min-width: 1200px) {
  .visible-lg {
    display: block !important;
  }
  table.visible-lg {
    display: table !important;
  }
  tr.visible-lg {
    display: table-row !important;
  }
  th.visible-lg,
  td.visible-lg {
    display: table-cell !important;
  }
}
@media (min-width: 1200px) {
  .visible-lg-block {
    display: block !important;
  }
}
@media (min-width: 1200px) {
  .visible-lg-inline {
    display: inline !important;
  }
}
@media (min-width: 1200px) {
  .visible-lg-inline-block {
    display: inline-block !important;
  }
}
@media (max-width: 767px) {
  .hidden-xs {
    display: none !important;
  }
}
@media (min-width: 768px) and (max-width: 991px) {
  .hidden-sm {
    display: none !important;
  }
}
@media (min-width: 992px) and (max-width: 1199px) {
  .hidden-md {
    display: none !important;
  }
}
@media (min-width: 1200px) {
  .hidden-lg {
    display: none !important;
  }
}
.visible-print {
  display: none !important;
}
@media print {
  .visible-print {
    display: block !important;
  }
  table.visible-print {
    display: table !important;
  }
  tr.visible-print {
    display: table-row !important;
  }
  th.visible-print,
  td.visible-print {
    display: table-cell !important;
  }
}
.visible-print-block {
  display: none !important;
}
@media print {
  .visible-print-block {
    display: block !important;
  }
}
.visible-print-inline {
  display: none !important;
}
@media print {
  .visible-print-inline {
    display: inline !important;
  }
}
.visible-print-inline-block {
  display: none !important;
}
@media print {
  .visible-print-inline-block {
    display: inline-block !important;
  }
}
@media print {
  .hidden-print {
    display: none !important;
  }
}
/*!
*
* Font Awesome
*
*/
/*!
 *  Font Awesome 4.7.0 by @davegandy - http://fontawesome.io - @fontawesome
 *  License - http://fontawesome.io/license (Font: SIL OFL 1.1, CSS: MIT License)
 */
/* FONT PATH
 * -------------------------- */
@font-face {
  font-family: 'FontAwesome';
  src: url('../components/font-awesome/fonts/fontawesome-webfont.eot?v=4.7.0');
  src: url('../components/font-awesome/fonts/fontawesome-webfont.eot?#iefix&v=4.7.0') format('embedded-opentype'), url('../components/font-awesome/fonts/fontawesome-webfont.woff2?v=4.7.0') format('woff2'), url('../components/font-awesome/fonts/fontawesome-webfont.woff?v=4.7.0') format('woff'), url('../components/font-awesome/fonts/fontawesome-webfont.ttf?v=4.7.0') format('truetype'), url('../components/font-awesome/fonts/fontawesome-webfont.svg?v=4.7.0#fontawesomeregular') format('svg');
  font-weight: normal;
  font-style: normal;
}
.fa {
  display: inline-block;
  font: normal normal normal 14px/1 FontAwesome;
  font-size: inherit;
  text-rendering: auto;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}
/* makes the font 33% larger relative to the icon container */
.fa-lg {
  font-size: 1.33333333em;
  line-height: 0.75em;
  vertical-align: -15%;
}
.fa-2x {
  font-size: 2em;
}
.fa-3x {
  font-size: 3em;
}
.fa-4x {
  font-size: 4em;
}
.fa-5x {
  font-size: 5em;
}
.fa-fw {
  width: 1.28571429em;
  text-align: center;
}
.fa-ul {
  padding-left: 0;
  margin-left: 2.14285714em;
  list-style-type: none;
}
.fa-ul > li {
  position: relative;
}
.fa-li {
  position: absolute;
  left: -2.14285714em;
  width: 2.14285714em;
  top: 0.14285714em;
  text-align: center;
}
.fa-li.fa-lg {
  left: -1.85714286em;
}
.fa-border {
  padding: .2em .25em .15em;
  border: solid 0.08em #eee;
  border-radius: .1em;
}
.fa-pull-left {
  float: left;
}
.fa-pull-right {
  float: right;
}
.fa.fa-pull-left {
  margin-right: .3em;
}
.fa.fa-pull-right {
  margin-left: .3em;
}
/* Deprecated as of 4.4.0 */
.pull-right {
  float: right;
}
.pull-left {
  float: left;
}
.fa.pull-left {
  margin-right: .3em;
}
.fa.pull-right {
  margin-left: .3em;
}
.fa-spin {
  -webkit-animation: fa-spin 2s infinite linear;
  animation: fa-spin 2s infinite linear;
}
.fa-pulse {
  -webkit-animation: fa-spin 1s infinite steps(8);
  animation: fa-spin 1s infinite steps(8);
}
@-webkit-keyframes fa-spin {
  0% {
    -webkit-transform: rotate(0deg);
    transform: rotate(0deg);
  }
  100% {
    -webkit-transform: rotate(359deg);
    transform: rotate(359deg);
  }
}
@keyframes fa-spin {
  0% {
    -webkit-transform: rotate(0deg);
    transform: rotate(0deg);
  }
  100% {
    -webkit-transform: rotate(359deg);
    transform: rotate(359deg);
  }
}
.fa-rotate-90 {
  -ms-filter: "progid:DXImageTransform.Microsoft.BasicImage(rotation=1)";
  -webkit-transform: rotate(90deg);
  -ms-transform: rotate(90deg);
  transform: rotate(90deg);
}
.fa-rotate-180 {
  -ms-filter: "progid:DXImageTransform.Microsoft.BasicImage(rotation=2)";
  -webkit-transform: rotate(180deg);
  -ms-transform: rotate(180deg);
  transform: rotate(180deg);
}
.fa-rotate-270 {
  -ms-filter: "progid:DXImageTransform.Microsoft.BasicImage(rotation=3)";
  -webkit-transform: rotate(270deg);
  -ms-transform: rotate(270deg);
  transform: rotate(270deg);
}
.fa-flip-horizontal {
  -ms-filter: "progid:DXImageTransform.Microsoft.BasicImage(rotation=0, mirror=1)";
  -webkit-transform: scale(-1, 1);
  -ms-transform: scale(-1, 1);
  transform: scale(-1, 1);
}
.fa-flip-vertical {
  -ms-filter: "progid:DXImageTransform.Microsoft.BasicImage(rotation=2, mirror=1)";
  -webkit-transform: scale(1, -1);
  -ms-transform: scale(1, -1);
  transform: scale(1, -1);
}
:root .fa-rotate-90,
:root .fa-rotate-180,
:root .fa-rotate-270,
:root .fa-flip-horizontal,
:root .fa-flip-vertical {
  filter: none;
}
.fa-stack {
  position: relative;
  display: inline-block;
  width: 2em;
  height: 2em;
  line-height: 2em;
  vertical-align: middle;
}
.fa-stack-1x,
.fa-stack-2x {
  position: absolute;
  left: 0;
  width: 100%;
  text-align: center;
}
.fa-stack-1x {
  line-height: inherit;
}
.fa-stack-2x {
  font-size: 2em;
}
.fa-inverse {
  color: #fff;
}
/* Font Awesome uses the Unicode Private Use Area (PUA) to ensure screen
   readers do not read off random characters that represent icons */
.fa-glass:before {
  content: "\f000";
}
.fa-music:before {
  content: "\f001";
}
.fa-search:before {
  content: "\f002";
}
.fa-envelope-o:before {
  content: "\f003";
}
.fa-heart:before {
  content: "\f004";
}
.fa-star:before {
  content: "\f005";
}
.fa-star-o:before {
  content: "\f006";
}
.fa-user:before {
  content: "\f007";
}
.fa-film:before {
  content: "\f008";
}
.fa-th-large:before {
  content: "\f009";
}
.fa-th:before {
  content: "\f00a";
}
.fa-th-list:before {
  content: "\f00b";
}
.fa-check:before {
  content: "\f00c";
}
.fa-remove:before,
.fa-close:before,
.fa-times:before {
  content: "\f00d";
}
.fa-search-plus:before {
  content: "\f00e";
}
.fa-search-minus:before {
  content: "\f010";
}
.fa-power-off:before {
  content: "\f011";
}
.fa-signal:before {
  content: "\f012";
}
.fa-gear:before,
.fa-cog:before {
  content: "\f013";
}
.fa-trash-o:before {
  content: "\f014";
}
.fa-home:before {
  content: "\f015";
}
.fa-file-o:before {
  content: "\f016";
}
.fa-clock-o:before {
  content: "\f017";
}
.fa-road:before {
  content: "\f018";
}
.fa-download:before {
  content: "\f019";
}
.fa-arrow-circle-o-down:before {
  content: "\f01a";
}
.fa-arrow-circle-o-up:before {
  content: "\f01b";
}
.fa-inbox:before {
  content: "\f01c";
}
.fa-play-circle-o:before {
  content: "\f01d";
}
.fa-rotate-right:before,
.fa-repeat:before {
  content: "\f01e";
}
.fa-refresh:before {
  content: "\f021";
}
.fa-list-alt:before {
  content: "\f022";
}
.fa-lock:before {
  content: "\f023";
}
.fa-flag:before {
  content: "\f024";
}
.fa-headphones:before {
  content: "\f025";
}
.fa-volume-off:before {
  content: "\f026";
}
.fa-volume-down:before {
  content: "\f027";
}
.fa-volume-up:before {
  content: "\f028";
}
.fa-qrcode:before {
  content: "\f029";
}
.fa-barcode:before {
  content: "\f02a";
}
.fa-tag:before {
  content: "\f02b";
}
.fa-tags:before {
  content: "\f02c";
}
.fa-book:before {
  content: "\f02d";
}
.fa-bookmark:before {
  content: "\f02e";
}
.fa-print:before {
  content: "\f02f";
}
.fa-camera:before {
  content: "\f030";
}
.fa-font:before {
  content: "\f031";
}
.fa-bold:before {
  content: "\f032";
}
.fa-italic:before {
  content: "\f033";
}
.fa-text-height:before {
  content: "\f034";
}
.fa-text-width:before {
  content: "\f035";
}
.fa-align-left:before {
  content: "\f036";
}
.fa-align-center:before {
  content: "\f037";
}
.fa-align-right:before {
  content: "\f038";
}
.fa-align-justify:before {
  content: "\f039";
}
.fa-list:before {
  content: "\f03a";
}
.fa-dedent:before,
.fa-outdent:before {
  content: "\f03b";
}
.fa-indent:before {
  content: "\f03c";
}
.fa-video-camera:before {
  content: "\f03d";
}
.fa-photo:before,
.fa-image:before,
.fa-picture-o:before {
  content: "\f03e";
}
.fa-pencil:before {
  content: "\f040";
}
.fa-map-marker:before {
  content: "\f041";
}
.fa-adjust:before {
  content: "\f042";
}
.fa-tint:before {
  content: "\f043";
}
.fa-edit:before,
.fa-pencil-square-o:before {
  content: "\f044";
}
.fa-share-square-o:before {
  content: "\f045";
}
.fa-check-square-o:before {
  content: "\f046";
}
.fa-arrows:before {
  content: "\f047";
}
.fa-step-backward:before {
  content: "\f048";
}
.fa-fast-backward:before {
  content: "\f049";
}
.fa-backward:before {
  content: "\f04a";
}
.fa-play:before {
  content: "\f04b";
}
.fa-pause:before {
  content: "\f04c";
}
.fa-stop:before {
  content: "\f04d";
}
.fa-forward:before {
  content: "\f04e";
}
.fa-fast-forward:before {
  content: "\f050";
}
.fa-step-forward:before {
  content: "\f051";
}
.fa-eject:before {
  content: "\f052";
}
.fa-chevron-left:before {
  content: "\f053";
}
.fa-chevron-right:before {
  content: "\f054";
}
.fa-plus-circle:before {
  content: "\f055";
}
.fa-minus-circle:before {
  content: "\f056";
}
.fa-times-circle:before {
  content: "\f057";
}
.fa-check-circle:before {
  content: "\f058";
}
.fa-question-circle:before {
  content: "\f059";
}
.fa-info-circle:before {
  content: "\f05a";
}
.fa-crosshairs:before {
  content: "\f05b";
}
.fa-times-circle-o:before {
  content: "\f05c";
}
.fa-check-circle-o:before {
  content: "\f05d";
}
.fa-ban:before {
  content: "\f05e";
}
.fa-arrow-left:before {
  content: "\f060";
}
.fa-arrow-right:before {
  content: "\f061";
}
.fa-arrow-up:before {
  content: "\f062";
}
.fa-arrow-down:before {
  content: "\f063";
}
.fa-mail-forward:before,
.fa-share:before {
  content: "\f064";
}
.fa-expand:before {
  content: "\f065";
}
.fa-compress:before {
  content: "\f066";
}
.fa-plus:before {
  content: "\f067";
}
.fa-minus:before {
  content: "\f068";
}
.fa-asterisk:before {
  content: "\f069";
}
.fa-exclamation-circle:before {
  content: "\f06a";
}
.fa-gift:before {
  content: "\f06b";
}
.fa-leaf:before {
  content: "\f06c";
}
.fa-fire:before {
  content: "\f06d";
}
.fa-eye:before {
  content: "\f06e";
}
.fa-eye-slash:before {
  content: "\f070";
}
.fa-warning:before,
.fa-exclamation-triangle:before {
  content: "\f071";
}
.fa-plane:before {
  content: "\f072";
}
.fa-calendar:before {
  content: "\f073";
}
.fa-random:before {
  content: "\f074";
}
.fa-comment:before {
  content: "\f075";
}
.fa-magnet:before {
  content: "\f076";
}
.fa-chevron-up:before {
  content: "\f077";
}
.fa-chevron-down:before {
  content: "\f078";
}
.fa-retweet:before {
  content: "\f079";
}
.fa-shopping-cart:before {
  content: "\f07a";
}
.fa-folder:before {
  content: "\f07b";
}
.fa-folder-open:before {
  content: "\f07c";
}
.fa-arrows-v:before {
  content: "\f07d";
}
.fa-arrows-h:before {
  content: "\f07e";
}
.fa-bar-chart-o:before,
.fa-bar-chart:before {
  content: "\f080";
}
.fa-twitter-square:before {
  content: "\f081";
}
.fa-facebook-square:before {
  content: "\f082";
}
.fa-camera-retro:before {
  content: "\f083";
}
.fa-key:before {
  content: "\f084";
}
.fa-gears:before,
.fa-cogs:before {
  content: "\f085";
}
.fa-comments:before {
  content: "\f086";
}
.fa-thumbs-o-up:before {
  content: "\f087";
}
.fa-thumbs-o-down:before {
  content: "\f088";
}
.fa-star-half:before {
  content: "\f089";
}
.fa-heart-o:before {
  content: "\f08a";
}
.fa-sign-out:before {
  content: "\f08b";
}
.fa-linkedin-square:before {
  content: "\f08c";
}
.fa-thumb-tack:before {
  content: "\f08d";
}
.fa-external-link:before {
  content: "\f08e";
}
.fa-sign-in:before {
  content: "\f090";
}
.fa-trophy:before {
  content: "\f091";
}
.fa-github-square:before {
  content: "\f092";
}
.fa-upload:before {
  content: "\f093";
}
.fa-lemon-o:before {
  content: "\f094";
}
.fa-phone:before {
  content: "\f095";
}
.fa-square-o:before {
  content: "\f096";
}
.fa-bookmark-o:before {
  content: "\f097";
}
.fa-phone-square:before {
  content: "\f098";
}
.fa-twitter:before {
  content: "\f099";
}
.fa-facebook-f:before,
.fa-facebook:before {
  content: "\f09a";
}
.fa-github:before {
  content: "\f09b";
}
.fa-unlock:before {
  content: "\f09c";
}
.fa-credit-card:before {
  content: "\f09d";
}
.fa-feed:before,
.fa-rss:before {
  content: "\f09e";
}
.fa-hdd-o:before {
  content: "\f0a0";
}
.fa-bullhorn:before {
  content: "\f0a1";
}
.fa-bell:before {
  content: "\f0f3";
}
.fa-certificate:before {
  content: "\f0a3";
}
.fa-hand-o-right:before {
  content: "\f0a4";
}
.fa-hand-o-left:before {
  content: "\f0a5";
}
.fa-hand-o-up:before {
  content: "\f0a6";
}
.fa-hand-o-down:before {
  content: "\f0a7";
}
.fa-arrow-circle-left:before {
  content: "\f0a8";
}
.fa-arrow-circle-right:before {
  content: "\f0a9";
}
.fa-arrow-circle-up:before {
  content: "\f0aa";
}
.fa-arrow-circle-down:before {
  content: "\f0ab";
}
.fa-globe:before {
  content: "\f0ac";
}
.fa-wrench:before {
  content: "\f0ad";
}
.fa-tasks:before {
  content: "\f0ae";
}
.fa-filter:before {
  content: "\f0b0";
}
.fa-briefcase:before {
  content: "\f0b1";
}
.fa-arrows-alt:before {
  content: "\f0b2";
}
.fa-group:before,
.fa-users:before {
  content: "\f0c0";
}
.fa-chain:before,
.fa-link:before {
  content: "\f0c1";
}
.fa-cloud:before {
  content: "\f0c2";
}
.fa-flask:before {
  content: "\f0c3";
}
.fa-cut:before,
.fa-scissors:before {
  content: "\f0c4";
}
.fa-copy:before,
.fa-files-o:before {
  content: "\f0c5";
}
.fa-paperclip:before {
  content: "\f0c6";
}
.fa-save:before,
.fa-floppy-o:before {
  content: "\f0c7";
}
.fa-square:before {
  content: "\f0c8";
}
.fa-navicon:before,
.fa-reorder:before,
.fa-bars:before {
  content: "\f0c9";
}
.fa-list-ul:before {
  content: "\f0ca";
}
.fa-list-ol:before {
  content: "\f0cb";
}
.fa-strikethrough:before {
  content: "\f0cc";
}
.fa-underline:before {
  content: "\f0cd";
}
.fa-table:before {
  content: "\f0ce";
}
.fa-magic:before {
  content: "\f0d0";
}
.fa-truck:before {
  content: "\f0d1";
}
.fa-pinterest:before {
  content: "\f0d2";
}
.fa-pinterest-square:before {
  content: "\f0d3";
}
.fa-google-plus-square:before {
  content: "\f0d4";
}
.fa-google-plus:before {
  content: "\f0d5";
}
.fa-money:before {
  content: "\f0d6";
}
.fa-caret-down:before {
  content: "\f0d7";
}
.fa-caret-up:before {
  content: "\f0d8";
}
.fa-caret-left:before {
  content: "\f0d9";
}
.fa-caret-right:before {
  content: "\f0da";
}
.fa-columns:before {
  content: "\f0db";
}
.fa-unsorted:before,
.fa-sort:before {
  content: "\f0dc";
}
.fa-sort-down:before,
.fa-sort-desc:before {
  content: "\f0dd";
}
.fa-sort-up:before,
.fa-sort-asc:before {
  content: "\f0de";
}
.fa-envelope:before {
  content: "\f0e0";
}
.fa-linkedin:before {
  content: "\f0e1";
}
.fa-rotate-left:before,
.fa-undo:before {
  content: "\f0e2";
}
.fa-legal:before,
.fa-gavel:before {
  content: "\f0e3";
}
.fa-dashboard:before,
.fa-tachometer:before {
  content: "\f0e4";
}
.fa-comment-o:before {
  content: "\f0e5";
}
.fa-comments-o:before {
  content: "\f0e6";
}
.fa-flash:before,
.fa-bolt:before {
  content: "\f0e7";
}
.fa-sitemap:before {
  content: "\f0e8";
}
.fa-umbrella:before {
  content: "\f0e9";
}
.fa-paste:before,
.fa-clipboard:before {
  content: "\f0ea";
}
.fa-lightbulb-o:before {
  content: "\f0eb";
}
.fa-exchange:before {
  content: "\f0ec";
}
.fa-cloud-download:before {
  content: "\f0ed";
}
.fa-cloud-upload:before {
  content: "\f0ee";
}
.fa-user-md:before {
  content: "\f0f0";
}
.fa-stethoscope:before {
  content: "\f0f1";
}
.fa-suitcase:before {
  content: "\f0f2";
}
.fa-bell-o:before {
  content: "\f0a2";
}
.fa-coffee:before {
  content: "\f0f4";
}
.fa-cutlery:before {
  content: "\f0f5";
}
.fa-file-text-o:before {
  content: "\f0f6";
}
.fa-building-o:before {
  content: "\f0f7";
}
.fa-hospital-o:before {
  content: "\f0f8";
}
.fa-ambulance:before {
  content: "\f0f9";
}
.fa-medkit:before {
  content: "\f0fa";
}
.fa-fighter-jet:before {
  content: "\f0fb";
}
.fa-beer:before {
  content: "\f0fc";
}
.fa-h-square:before {
  content: "\f0fd";
}
.fa-plus-square:before {
  content: "\f0fe";
}
.fa-angle-double-left:before {
  content: "\f100";
}
.fa-angle-double-right:before {
  content: "\f101";
}
.fa-angle-double-up:before {
  content: "\f102";
}
.fa-angle-double-down:before {
  content: "\f103";
}
.fa-angle-left:before {
  content: "\f104";
}
.fa-angle-right:before {
  content: "\f105";
}
.fa-angle-up:before {
  content: "\f106";
}
.fa-angle-down:before {
  content: "\f107";
}
.fa-desktop:before {
  content: "\f108";
}
.fa-laptop:before {
  content: "\f109";
}
.fa-tablet:before {
  content: "\f10a";
}
.fa-mobile-phone:before,
.fa-mobile:before {
  content: "\f10b";
}
.fa-circle-o:before {
  content: "\f10c";
}
.fa-quote-left:before {
  content: "\f10d";
}
.fa-quote-right:before {
  content: "\f10e";
}
.fa-spinner:before {
  content: "\f110";
}
.fa-circle:before {
  content: "\f111";
}
.fa-mail-reply:before,
.fa-reply:before {
  content: "\f112";
}
.fa-github-alt:before {
  content: "\f113";
}
.fa-folder-o:before {
  content: "\f114";
}
.fa-folder-open-o:before {
  content: "\f115";
}
.fa-smile-o:before {
  content: "\f118";
}
.fa-frown-o:before {
  content: "\f119";
}
.fa-meh-o:before {
  content: "\f11a";
}
.fa-gamepad:before {
  content: "\f11b";
}
.fa-keyboard-o:before {
  content: "\f11c";
}
.fa-flag-o:before {
  content: "\f11d";
}
.fa-flag-checkered:before {
  content: "\f11e";
}
.fa-terminal:before {
  content: "\f120";
}
.fa-code:before {
  content: "\f121";
}
.fa-mail-reply-all:before,
.fa-reply-all:before {
  content: "\f122";
}
.fa-star-half-empty:before,
.fa-star-half-full:before,
.fa-star-half-o:before {
  content: "\f123";
}
.fa-location-arrow:before {
  content: "\f124";
}
.fa-crop:before {
  content: "\f125";
}
.fa-code-fork:before {
  content: "\f126";
}
.fa-unlink:before,
.fa-chain-broken:before {
  content: "\f127";
}
.fa-question:before {
  content: "\f128";
}
.fa-info:before {
  content: "\f129";
}
.fa-exclamation:before {
  content: "\f12a";
}
.fa-superscript:before {
  content: "\f12b";
}
.fa-subscript:before {
  content: "\f12c";
}
.fa-eraser:before {
  content: "\f12d";
}
.fa-puzzle-piece:before {
  content: "\f12e";
}
.fa-microphone:before {
  content: "\f130";
}
.fa-microphone-slash:before {
  content: "\f131";
}
.fa-shield:before {
  content: "\f132";
}
.fa-calendar-o:before {
  content: "\f133";
}
.fa-fire-extinguisher:before {
  content: "\f134";
}
.fa-rocket:before {
  content: "\f135";
}
.fa-maxcdn:before {
  content: "\f136";
}
.fa-chevron-circle-left:before {
  content: "\f137";
}
.fa-chevron-circle-right:before {
  content: "\f138";
}
.fa-chevron-circle-up:before {
  content: "\f139";
}
.fa-chevron-circle-down:before {
  content: "\f13a";
}
.fa-html5:before {
  content: "\f13b";
}
.fa-css3:before {
  content: "\f13c";
}
.fa-anchor:before {
  content: "\f13d";
}
.fa-unlock-alt:before {
  content: "\f13e";
}
.fa-bullseye:before {
  content: "\f140";
}
.fa-ellipsis-h:before {
  content: "\f141";
}
.fa-ellipsis-v:before {
  content: "\f142";
}
.fa-rss-square:before {
  content: "\f143";
}
.fa-play-circle:before {
  content: "\f144";
}
.fa-ticket:before {
  content: "\f145";
}
.fa-minus-square:before {
  content: "\f146";
}
.fa-minus-square-o:before {
  content: "\f147";
}
.fa-level-up:before {
  content: "\f148";
}
.fa-level-down:before {
  content: "\f149";
}
.fa-check-square:before {
  content: "\f14a";
}
.fa-pencil-square:before {
  content: "\f14b";
}
.fa-external-link-square:before {
  content: "\f14c";
}
.fa-share-square:before {
  content: "\f14d";
}
.fa-compass:before {
  content: "\f14e";
}
.fa-toggle-down:before,
.fa-caret-square-o-down:before {
  content: "\f150";
}
.fa-toggle-up:before,
.fa-caret-square-o-up:before {
  content: "\f151";
}
.fa-toggle-right:before,
.fa-caret-square-o-right:before {
  content: "\f152";
}
.fa-euro:before,
.fa-eur:before {
  content: "\f153";
}
.fa-gbp:before {
  content: "\f154";
}
.fa-dollar:before,
.fa-usd:before {
  content: "\f155";
}
.fa-rupee:before,
.fa-inr:before {
  content: "\f156";
}
.fa-cny:before,
.fa-rmb:before,
.fa-yen:before,
.fa-jpy:before {
  content: "\f157";
}
.fa-ruble:before,
.fa-rouble:before,
.fa-rub:before {
  content: "\f158";
}
.fa-won:before,
.fa-krw:before {
  content: "\f159";
}
.fa-bitcoin:before,
.fa-btc:before {
  content: "\f15a";
}
.fa-file:before {
  content: "\f15b";
}
.fa-file-text:before {
  content: "\f15c";
}
.fa-sort-alpha-asc:before {
  content: "\f15d";
}
.fa-sort-alpha-desc:before {
  content: "\f15e";
}
.fa-sort-amount-asc:before {
  content: "\f160";
}
.fa-sort-amount-desc:before {
  content: "\f161";
}
.fa-sort-numeric-asc:before {
  content: "\f162";
}
.fa-sort-numeric-desc:before {
  content: "\f163";
}
.fa-thumbs-up:before {
  content: "\f164";
}
.fa-thumbs-down:before {
  content: "\f165";
}
.fa-youtube-square:before {
  content: "\f166";
}
.fa-youtube:before {
  content: "\f167";
}
.fa-xing:before {
  content: "\f168";
}
.fa-xing-square:before {
  content: "\f169";
}
.fa-youtube-play:before {
  content: "\f16a";
}
.fa-dropbox:before {
  content: "\f16b";
}
.fa-stack-overflow:before {
  content: "\f16c";
}
.fa-instagram:before {
  content: "\f16d";
}
.fa-flickr:before {
  content: "\f16e";
}
.fa-adn:before {
  content: "\f170";
}
.fa-bitbucket:before {
  content: "\f171";
}
.fa-bitbucket-square:before {
  content: "\f172";
}
.fa-tumblr:before {
  content: "\f173";
}
.fa-tumblr-square:before {
  content: "\f174";
}
.fa-long-arrow-down:before {
  content: "\f175";
}
.fa-long-arrow-up:before {
  content: "\f176";
}
.fa-long-arrow-left:before {
  content: "\f177";
}
.fa-long-arrow-right:before {
  content: "\f178";
}
.fa-apple:before {
  content: "\f179";
}
.fa-windows:before {
  content: "\f17a";
}
.fa-android:before {
  content: "\f17b";
}
.fa-linux:before {
  content: "\f17c";
}
.fa-dribbble:before {
  content: "\f17d";
}
.fa-skype:before {
  content: "\f17e";
}
.fa-foursquare:before {
  content: "\f180";
}
.fa-trello:before {
  content: "\f181";
}
.fa-female:before {
  content: "\f182";
}
.fa-male:before {
  content: "\f183";
}
.fa-gittip:before,
.fa-gratipay:before {
  content: "\f184";
}
.fa-sun-o:before {
  content: "\f185";
}
.fa-moon-o:before {
  content: "\f186";
}
.fa-archive:before {
  content: "\f187";
}
.fa-bug:before {
  content: "\f188";
}
.fa-vk:before {
  content: "\f189";
}
.fa-weibo:before {
  content: "\f18a";
}
.fa-renren:before {
  content: "\f18b";
}
.fa-pagelines:before {
  content: "\f18c";
}
.fa-stack-exchange:before {
  content: "\f18d";
}
.fa-arrow-circle-o-right:before {
  content: "\f18e";
}
.fa-arrow-circle-o-left:before {
  content: "\f190";
}
.fa-toggle-left:before,
.fa-caret-square-o-left:before {
  content: "\f191";
}
.fa-dot-circle-o:before {
  content: "\f192";
}
.fa-wheelchair:before {
  content: "\f193";
}
.fa-vimeo-square:before {
  content: "\f194";
}
.fa-turkish-lira:before,
.fa-try:before {
  content: "\f195";
}
.fa-plus-square-o:before {
  content: "\f196";
}
.fa-space-shuttle:before {
  content: "\f197";
}
.fa-slack:before {
  content: "\f198";
}
.fa-envelope-square:before {
  content: "\f199";
}
.fa-wordpress:before {
  content: "\f19a";
}
.fa-openid:before {
  content: "\f19b";
}
.fa-institution:before,
.fa-bank:before,
.fa-university:before {
  content: "\f19c";
}
.fa-mortar-board:before,
.fa-graduation-cap:before {
  content: "\f19d";
}
.fa-yahoo:before {
  content: "\f19e";
}
.fa-google:before {
  content: "\f1a0";
}
.fa-reddit:before {
  content: "\f1a1";
}
.fa-reddit-square:before {
  content: "\f1a2";
}
.fa-stumbleupon-circle:before {
  content: "\f1a3";
}
.fa-stumbleupon:before {
  content: "\f1a4";
}
.fa-delicious:before {
  content: "\f1a5";
}
.fa-digg:before {
  content: "\f1a6";
}
.fa-pied-piper-pp:before {
  content: "\f1a7";
}
.fa-pied-piper-alt:before {
  content: "\f1a8";
}
.fa-drupal:before {
  content: "\f1a9";
}
.fa-joomla:before {
  content: "\f1aa";
}
.fa-language:before {
  content: "\f1ab";
}
.fa-fax:before {
  content: "\f1ac";
}
.fa-building:before {
  content: "\f1ad";
}
.fa-child:before {
  content: "\f1ae";
}
.fa-paw:before {
  content: "\f1b0";
}
.fa-spoon:before {
  content: "\f1b1";
}
.fa-cube:before {
  content: "\f1b2";
}
.fa-cubes:before {
  content: "\f1b3";
}
.fa-behance:before {
  content: "\f1b4";
}
.fa-behance-square:before {
  content: "\f1b5";
}
.fa-steam:before {
  content: "\f1b6";
}
.fa-steam-square:before {
  content: "\f1b7";
}
.fa-recycle:before {
  content: "\f1b8";
}
.fa-automobile:before,
.fa-car:before {
  content: "\f1b9";
}
.fa-cab:before,
.fa-taxi:before {
  content: "\f1ba";
}
.fa-tree:before {
  content: "\f1bb";
}
.fa-spotify:before {
  content: "\f1bc";
}
.fa-deviantart:before {
  content: "\f1bd";
}
.fa-soundcloud:before {
  content: "\f1be";
}
.fa-database:before {
  content: "\f1c0";
}
.fa-file-pdf-o:before {
  content: "\f1c1";
}
.fa-file-word-o:before {
  content: "\f1c2";
}
.fa-file-excel-o:before {
  content: "\f1c3";
}
.fa-file-powerpoint-o:before {
  content: "\f1c4";
}
.fa-file-photo-o:before,
.fa-file-picture-o:before,
.fa-file-image-o:before {
  content: "\f1c5";
}
.fa-file-zip-o:before,
.fa-file-archive-o:before {
  content: "\f1c6";
}
.fa-file-sound-o:before,
.fa-file-audio-o:before {
  content: "\f1c7";
}
.fa-file-movie-o:before,
.fa-file-video-o:before {
  content: "\f1c8";
}
.fa-file-code-o:before {
  content: "\f1c9";
}
.fa-vine:before {
  content: "\f1ca";
}
.fa-codepen:before {
  content: "\f1cb";
}
.fa-jsfiddle:before {
  content: "\f1cc";
}
.fa-life-bouy:before,
.fa-life-buoy:before,
.fa-life-saver:before,
.fa-support:before,
.fa-life-ring:before {
  content: "\f1cd";
}
.fa-circle-o-notch:before {
  content: "\f1ce";
}
.fa-ra:before,
.fa-resistance:before,
.fa-rebel:before {
  content: "\f1d0";
}
.fa-ge:before,
.fa-empire:before {
  content: "\f1d1";
}
.fa-git-square:before {
  content: "\f1d2";
}
.fa-git:before {
  content: "\f1d3";
}
.fa-y-combinator-square:before,
.fa-yc-square:before,
.fa-hacker-news:before {
  content: "\f1d4";
}
.fa-tencent-weibo:before {
  content: "\f1d5";
}
.fa-qq:before {
  content: "\f1d6";
}
.fa-wechat:before,
.fa-weixin:before {
  content: "\f1d7";
}
.fa-send:before,
.fa-paper-plane:before {
  content: "\f1d8";
}
.fa-send-o:before,
.fa-paper-plane-o:before {
  content: "\f1d9";
}
.fa-history:before {
  content: "\f1da";
}
.fa-circle-thin:before {
  content: "\f1db";
}
.fa-header:before {
  content: "\f1dc";
}
.fa-paragraph:before {
  content: "\f1dd";
}
.fa-sliders:before {
  content: "\f1de";
}
.fa-share-alt:before {
  content: "\f1e0";
}
.fa-share-alt-square:before {
  content: "\f1e1";
}
.fa-bomb:before {
  content: "\f1e2";
}
.fa-soccer-ball-o:before,
.fa-futbol-o:before {
  content: "\f1e3";
}
.fa-tty:before {
  content: "\f1e4";
}
.fa-binoculars:before {
  content: "\f1e5";
}
.fa-plug:before {
  content: "\f1e6";
}
.fa-slideshare:before {
  content: "\f1e7";
}
.fa-twitch:before {
  content: "\f1e8";
}
.fa-yelp:before {
  content: "\f1e9";
}
.fa-newspaper-o:before {
  content: "\f1ea";
}
.fa-wifi:before {
  content: "\f1eb";
}
.fa-calculator:before {
  content: "\f1ec";
}
.fa-paypal:before {
  content: "\f1ed";
}
.fa-google-wallet:before {
  content: "\f1ee";
}
.fa-cc-visa:before {
  content: "\f1f0";
}
.fa-cc-mastercard:before {
  content: "\f1f1";
}
.fa-cc-discover:before {
  content: "\f1f2";
}
.fa-cc-amex:before {
  content: "\f1f3";
}
.fa-cc-paypal:before {
  content: "\f1f4";
}
.fa-cc-stripe:before {
  content: "\f1f5";
}
.fa-bell-slash:before {
  content: "\f1f6";
}
.fa-bell-slash-o:before {
  content: "\f1f7";
}
.fa-trash:before {
  content: "\f1f8";
}
.fa-copyright:before {
  content: "\f1f9";
}
.fa-at:before {
  content: "\f1fa";
}
.fa-eyedropper:before {
  content: "\f1fb";
}
.fa-paint-brush:before {
  content: "\f1fc";
}
.fa-birthday-cake:before {
  content: "\f1fd";
}
.fa-area-chart:before {
  content: "\f1fe";
}
.fa-pie-chart:before {
  content: "\f200";
}
.fa-line-chart:before {
  content: "\f201";
}
.fa-lastfm:before {
  content: "\f202";
}
.fa-lastfm-square:before {
  content: "\f203";
}
.fa-toggle-off:before {
  content: "\f204";
}
.fa-toggle-on:before {
  content: "\f205";
}
.fa-bicycle:before {
  content: "\f206";
}
.fa-bus:before {
  content: "\f207";
}
.fa-ioxhost:before {
  content: "\f208";
}
.fa-angellist:before {
  content: "\f209";
}
.fa-cc:before {
  content: "\f20a";
}
.fa-shekel:before,
.fa-sheqel:before,
.fa-ils:before {
  content: "\f20b";
}
.fa-meanpath:before {
  content: "\f20c";
}
.fa-buysellads:before {
  content: "\f20d";
}
.fa-connectdevelop:before {
  content: "\f20e";
}
.fa-dashcube:before {
  content: "\f210";
}
.fa-forumbee:before {
  content: "\f211";
}
.fa-leanpub:before {
  content: "\f212";
}
.fa-sellsy:before {
  content: "\f213";
}
.fa-shirtsinbulk:before {
  content: "\f214";
}
.fa-simplybuilt:before {
  content: "\f215";
}
.fa-skyatlas:before {
  content: "\f216";
}
.fa-cart-plus:before {
  content: "\f217";
}
.fa-cart-arrow-down:before {
  content: "\f218";
}
.fa-diamond:before {
  content: "\f219";
}
.fa-ship:before {
  content: "\f21a";
}
.fa-user-secret:before {
  content: "\f21b";
}
.fa-motorcycle:before {
  content: "\f21c";
}
.fa-street-view:before {
  content: "\f21d";
}
.fa-heartbeat:before {
  content: "\f21e";
}
.fa-venus:before {
  content: "\f221";
}
.fa-mars:before {
  content: "\f222";
}
.fa-mercury:before {
  content: "\f223";
}
.fa-intersex:before,
.fa-transgender:before {
  content: "\f224";
}
.fa-transgender-alt:before {
  content: "\f225";
}
.fa-venus-double:before {
  content: "\f226";
}
.fa-mars-double:before {
  content: "\f227";
}
.fa-venus-mars:before {
  content: "\f228";
}
.fa-mars-stroke:before {
  content: "\f229";
}
.fa-mars-stroke-v:before {
  content: "\f22a";
}
.fa-mars-stroke-h:before {
  content: "\f22b";
}
.fa-neuter:before {
  content: "\f22c";
}
.fa-genderless:before {
  content: "\f22d";
}
.fa-facebook-official:before {
  content: "\f230";
}
.fa-pinterest-p:before {
  content: "\f231";
}
.fa-whatsapp:before {
  content: "\f232";
}
.fa-server:before {
  content: "\f233";
}
.fa-user-plus:before {
  content: "\f234";
}
.fa-user-times:before {
  content: "\f235";
}
.fa-hotel:before,
.fa-bed:before {
  content: "\f236";
}
.fa-viacoin:before {
  content: "\f237";
}
.fa-train:before {
  content: "\f238";
}
.fa-subway:before {
  content: "\f239";
}
.fa-medium:before {
  content: "\f23a";
}
.fa-yc:before,
.fa-y-combinator:before {
  content: "\f23b";
}
.fa-optin-monster:before {
  content: "\f23c";
}
.fa-opencart:before {
  content: "\f23d";
}
.fa-expeditedssl:before {
  content: "\f23e";
}
.fa-battery-4:before,
.fa-battery:before,
.fa-battery-full:before {
  content: "\f240";
}
.fa-battery-3:before,
.fa-battery-three-quarters:before {
  content: "\f241";
}
.fa-battery-2:before,
.fa-battery-half:before {
  content: "\f242";
}
.fa-battery-1:before,
.fa-battery-quarter:before {
  content: "\f243";
}
.fa-battery-0:before,
.fa-battery-empty:before {
  content: "\f244";
}
.fa-mouse-pointer:before {
  content: "\f245";
}
.fa-i-cursor:before {
  content: "\f246";
}
.fa-object-group:before {
  content: "\f247";
}
.fa-object-ungroup:before {
  content: "\f248";
}
.fa-sticky-note:before {
  content: "\f249";
}
.fa-sticky-note-o:before {
  content: "\f24a";
}
.fa-cc-jcb:before {
  content: "\f24b";
}
.fa-cc-diners-club:before {
  content: "\f24c";
}
.fa-clone:before {
  content: "\f24d";
}
.fa-balance-scale:before {
  content: "\f24e";
}
.fa-hourglass-o:before {
  content: "\f250";
}
.fa-hourglass-1:before,
.fa-hourglass-start:before {
  content: "\f251";
}
.fa-hourglass-2:before,
.fa-hourglass-half:before {
  content: "\f252";
}
.fa-hourglass-3:before,
.fa-hourglass-end:before {
  content: "\f253";
}
.fa-hourglass:before {
  content: "\f254";
}
.fa-hand-grab-o:before,
.fa-hand-rock-o:before {
  content: "\f255";
}
.fa-hand-stop-o:before,
.fa-hand-paper-o:before {
  content: "\f256";
}
.fa-hand-scissors-o:before {
  content: "\f257";
}
.fa-hand-lizard-o:before {
  content: "\f258";
}
.fa-hand-spock-o:before {
  content: "\f259";
}
.fa-hand-pointer-o:before {
  content: "\f25a";
}
.fa-hand-peace-o:before {
  content: "\f25b";
}
.fa-trademark:before {
  content: "\f25c";
}
.fa-registered:before {
  content: "\f25d";
}
.fa-creative-commons:before {
  content: "\f25e";
}
.fa-gg:before {
  content: "\f260";
}
.fa-gg-circle:before {
  content: "\f261";
}
.fa-tripadvisor:before {
  content: "\f262";
}
.fa-odnoklassniki:before {
  content: "\f263";
}
.fa-odnoklassniki-square:before {
  content: "\f264";
}
.fa-get-pocket:before {
  content: "\f265";
}
.fa-wikipedia-w:before {
  content: "\f266";
}
.fa-safari:before {
  content: "\f267";
}
.fa-chrome:before {
  content: "\f268";
}
.fa-firefox:before {
  content: "\f269";
}
.fa-opera:before {
  content: "\f26a";
}
.fa-internet-explorer:before {
  content: "\f26b";
}
.fa-tv:before,
.fa-television:before {
  content: "\f26c";
}
.fa-contao:before {
  content: "\f26d";
}
.fa-500px:before {
  content: "\f26e";
}
.fa-amazon:before {
  content: "\f270";
}
.fa-calendar-plus-o:before {
  content: "\f271";
}
.fa-calendar-minus-o:before {
  content: "\f272";
}
.fa-calendar-times-o:before {
  content: "\f273";
}
.fa-calendar-check-o:before {
  content: "\f274";
}
.fa-industry:before {
  content: "\f275";
}
.fa-map-pin:before {
  content: "\f276";
}
.fa-map-signs:before {
  content: "\f277";
}
.fa-map-o:before {
  content: "\f278";
}
.fa-map:before {
  content: "\f279";
}
.fa-commenting:before {
  content: "\f27a";
}
.fa-commenting-o:before {
  content: "\f27b";
}
.fa-houzz:before {
  content: "\f27c";
}
.fa-vimeo:before {
  content: "\f27d";
}
.fa-black-tie:before {
  content: "\f27e";
}
.fa-fonticons:before {
  content: "\f280";
}
.fa-reddit-alien:before {
  content: "\f281";
}
.fa-edge:before {
  content: "\f282";
}
.fa-credit-card-alt:before {
  content: "\f283";
}
.fa-codiepie:before {
  content: "\f284";
}
.fa-modx:before {
  content: "\f285";
}
.fa-fort-awesome:before {
  content: "\f286";
}
.fa-usb:before {
  content: "\f287";
}
.fa-product-hunt:before {
  content: "\f288";
}
.fa-mixcloud:before {
  content: "\f289";
}
.fa-scribd:before {
  content: "\f28a";
}
.fa-pause-circle:before {
  content: "\f28b";
}
.fa-pause-circle-o:before {
  content: "\f28c";
}
.fa-stop-circle:before {
  content: "\f28d";
}
.fa-stop-circle-o:before {
  content: "\f28e";
}
.fa-shopping-bag:before {
  content: "\f290";
}
.fa-shopping-basket:before {
  content: "\f291";
}
.fa-hashtag:before {
  content: "\f292";
}
.fa-bluetooth:before {
  content: "\f293";
}
.fa-bluetooth-b:before {
  content: "\f294";
}
.fa-percent:before {
  content: "\f295";
}
.fa-gitlab:before {
  content: "\f296";
}
.fa-wpbeginner:before {
  content: "\f297";
}
.fa-wpforms:before {
  content: "\f298";
}
.fa-envira:before {
  content: "\f299";
}
.fa-universal-access:before {
  content: "\f29a";
}
.fa-wheelchair-alt:before {
  content: "\f29b";
}
.fa-question-circle-o:before {
  content: "\f29c";
}
.fa-blind:before {
  content: "\f29d";
}
.fa-audio-description:before {
  content: "\f29e";
}
.fa-volume-control-phone:before {
  content: "\f2a0";
}
.fa-braille:before {
  content: "\f2a1";
}
.fa-assistive-listening-systems:before {
  content: "\f2a2";
}
.fa-asl-interpreting:before,
.fa-american-sign-language-interpreting:before {
  content: "\f2a3";
}
.fa-deafness:before,
.fa-hard-of-hearing:before,
.fa-deaf:before {
  content: "\f2a4";
}
.fa-glide:before {
  content: "\f2a5";
}
.fa-glide-g:before {
  content: "\f2a6";
}
.fa-signing:before,
.fa-sign-language:before {
  content: "\f2a7";
}
.fa-low-vision:before {
  content: "\f2a8";
}
.fa-viadeo:before {
  content: "\f2a9";
}
.fa-viadeo-square:before {
  content: "\f2aa";
}
.fa-snapchat:before {
  content: "\f2ab";
}
.fa-snapchat-ghost:before {
  content: "\f2ac";
}
.fa-snapchat-square:before {
  content: "\f2ad";
}
.fa-pied-piper:before {
  content: "\f2ae";
}
.fa-first-order:before {
  content: "\f2b0";
}
.fa-yoast:before {
  content: "\f2b1";
}
.fa-themeisle:before {
  content: "\f2b2";
}
.fa-google-plus-circle:before,
.fa-google-plus-official:before {
  content: "\f2b3";
}
.fa-fa:before,
.fa-font-awesome:before {
  content: "\f2b4";
}
.fa-handshake-o:before {
  content: "\f2b5";
}
.fa-envelope-open:before {
  content: "\f2b6";
}
.fa-envelope-open-o:before {
  content: "\f2b7";
}
.fa-linode:before {
  content: "\f2b8";
}
.fa-address-book:before {
  content: "\f2b9";
}
.fa-address-book-o:before {
  content: "\f2ba";
}
.fa-vcard:before,
.fa-address-card:before {
  content: "\f2bb";
}
.fa-vcard-o:before,
.fa-address-card-o:before {
  content: "\f2bc";
}
.fa-user-circle:before {
  content: "\f2bd";
}
.fa-user-circle-o:before {
  content: "\f2be";
}
.fa-user-o:before {
  content: "\f2c0";
}
.fa-id-badge:before {
  content: "\f2c1";
}
.fa-drivers-license:before,
.fa-id-card:before {
  content: "\f2c2";
}
.fa-drivers-license-o:before,
.fa-id-card-o:before {
  content: "\f2c3";
}
.fa-quora:before {
  content: "\f2c4";
}
.fa-free-code-camp:before {
  content: "\f2c5";
}
.fa-telegram:before {
  content: "\f2c6";
}
.fa-thermometer-4:before,
.fa-thermometer:before,
.fa-thermometer-full:before {
  content: "\f2c7";
}
.fa-thermometer-3:before,
.fa-thermometer-three-quarters:before {
  content: "\f2c8";
}
.fa-thermometer-2:before,
.fa-thermometer-half:before {
  content: "\f2c9";
}
.fa-thermometer-1:before,
.fa-thermometer-quarter:before {
  content: "\f2ca";
}
.fa-thermometer-0:before,
.fa-thermometer-empty:before {
  content: "\f2cb";
}
.fa-shower:before {
  content: "\f2cc";
}
.fa-bathtub:before,
.fa-s15:before,
.fa-bath:before {
  content: "\f2cd";
}
.fa-podcast:before {
  content: "\f2ce";
}
.fa-window-maximize:before {
  content: "\f2d0";
}
.fa-window-minimize:before {
  content: "\f2d1";
}
.fa-window-restore:before {
  content: "\f2d2";
}
.fa-times-rectangle:before,
.fa-window-close:before {
  content: "\f2d3";
}
.fa-times-rectangle-o:before,
.fa-window-close-o:before {
  content: "\f2d4";
}
.fa-bandcamp:before {
  content: "\f2d5";
}
.fa-grav:before {
  content: "\f2d6";
}
.fa-etsy:before {
  content: "\f2d7";
}
.fa-imdb:before {
  content: "\f2d8";
}
.fa-ravelry:before {
  content: "\f2d9";
}
.fa-eercast:before {
  content: "\f2da";
}
.fa-microchip:before {
  content: "\f2db";
}
.fa-snowflake-o:before {
  content: "\f2dc";
}
.fa-superpowers:before {
  content: "\f2dd";
}
.fa-wpexplorer:before {
  content: "\f2de";
}
.fa-meetup:before {
  content: "\f2e0";
}
.sr-only {
  position: absolute;
  width: 1px;
  height: 1px;
  padding: 0;
  margin: -1px;
  overflow: hidden;
  clip: rect(0, 0, 0, 0);
  border: 0;
}
.sr-only-focusable:active,
.sr-only-focusable:focus {
  position: static;
  width: auto;
  height: auto;
  margin: 0;
  overflow: visible;
  clip: auto;
}
.sr-only-focusable:active,
.sr-only-focusable:focus {
  position: static;
  width: auto;
  height: auto;
  margin: 0;
  overflow: visible;
  clip: auto;
}
/*!
*
* IPython base
*
*/
.modal.fade .modal-dialog {
  -webkit-transform: translate(0, 0);
  -ms-transform: translate(0, 0);
  -o-transform: translate(0, 0);
  transform: translate(0, 0);
}
code {
  color: #000;
}
pre {
  font-size: inherit;
  line-height: inherit;
}
label {
  font-weight: normal;
}
/* Make the page background atleast 100% the height of the view port */
/* Make the page itself atleast 70% the height of the view port */
.border-box-sizing {
  box-sizing: border-box;
  -moz-box-sizing: border-box;
  -webkit-box-sizing: border-box;
}
.corner-all {
  border-radius: 2px;
}
.no-padding {
  padding: 0px;
}
/* Flexible box model classes */
/* Taken from Alex Russell http://infrequently.org/2009/08/css-3-progress/ */
/* This file is a compatability layer.  It allows the usage of flexible box 
model layouts accross multiple browsers, including older browsers.  The newest,
universal implementation of the flexible box model is used when available (see
`Modern browsers` comments below).  Browsers that are known to implement this 
new spec completely include:

    Firefox 28.0+
    Chrome 29.0+
    Internet Explorer 11+ 
    Opera 17.0+

Browsers not listed, including Safari, are supported via the styling under the
`Old browsers` comments below.
*/
.hbox {
  /* Old browsers */
  display: -webkit-box;
  -webkit-box-orient: horizontal;
  -webkit-box-align: stretch;
  display: -moz-box;
  -moz-box-orient: horizontal;
  -moz-box-align: stretch;
  display: box;
  box-orient: horizontal;
  box-align: stretch;
  /* Modern browsers */
  display: flex;
  flex-direction: row;
  align-items: stretch;
}
.hbox > * {
  /* Old browsers */
  -webkit-box-flex: 0;
  -moz-box-flex: 0;
  box-flex: 0;
  /* Modern browsers */
  flex: none;
}
.vbox {
  /* Old browsers */
  display: -webkit-box;
  -webkit-box-orient: vertical;
  -webkit-box-align: stretch;
  display: -moz-box;
  -moz-box-orient: vertical;
  -moz-box-align: stretch;
  display: box;
  box-orient: vertical;
  box-align: stretch;
  /* Modern browsers */
  display: flex;
  flex-direction: column;
  align-items: stretch;
}
.vbox > * {
  /* Old browsers */
  -webkit-box-flex: 0;
  -moz-box-flex: 0;
  box-flex: 0;
  /* Modern browsers */
  flex: none;
}
.hbox.reverse,
.vbox.reverse,
.reverse {
  /* Old browsers */
  -webkit-box-direction: reverse;
  -moz-box-direction: reverse;
  box-direction: reverse;
  /* Modern browsers */
  flex-direction: row-reverse;
}
.hbox.box-flex0,
.vbox.box-flex0,
.box-flex0 {
  /* Old browsers */
  -webkit-box-flex: 0;
  -moz-box-flex: 0;
  box-flex: 0;
  /* Modern browsers */
  flex: none;
  width: auto;
}
.hbox.box-flex1,
.vbox.box-flex1,
.box-flex1 {
  /* Old browsers */
  -webkit-box-flex: 1;
  -moz-box-flex: 1;
  box-flex: 1;
  /* Modern browsers */
  flex: 1;
}
.hbox.box-flex,
.vbox.box-flex,
.box-flex {
  /* Old browsers */
  /* Old browsers */
  -webkit-box-flex: 1;
  -moz-box-flex: 1;
  box-flex: 1;
  /* Modern browsers */
  flex: 1;
}
.hbox.box-flex2,
.vbox.box-flex2,
.box-flex2 {
  /* Old browsers */
  -webkit-box-flex: 2;
  -moz-box-flex: 2;
  box-flex: 2;
  /* Modern browsers */
  flex: 2;
}
.box-group1 {
  /*  Deprecated */
  -webkit-box-flex-group: 1;
  -moz-box-flex-group: 1;
  box-flex-group: 1;
}
.box-group2 {
  /* Deprecated */
  -webkit-box-flex-group: 2;
  -moz-box-flex-group: 2;
  box-flex-group: 2;
}
.hbox.start,
.vbox.start,
.start {
  /* Old browsers */
  -webkit-box-pack: start;
  -moz-box-pack: start;
  box-pack: start;
  /* Modern browsers */
  justify-content: flex-start;
}
.hbox.end,
.vbox.end,
.end {
  /* Old browsers */
  -webkit-box-pack: end;
  -moz-box-pack: end;
  box-pack: end;
  /* Modern browsers */
  justify-content: flex-end;
}
.hbox.center,
.vbox.center,
.center {
  /* Old browsers */
  -webkit-box-pack: center;
  -moz-box-pack: center;
  box-pack: center;
  /* Modern browsers */
  justify-content: center;
}
.hbox.baseline,
.vbox.baseline,
.baseline {
  /* Old browsers */
  -webkit-box-pack: baseline;
  -moz-box-pack: baseline;
  box-pack: baseline;
  /* Modern browsers */
  justify-content: baseline;
}
.hbox.stretch,
.vbox.stretch,
.stretch {
  /* Old browsers */
  -webkit-box-pack: stretch;
  -moz-box-pack: stretch;
  box-pack: stretch;
  /* Modern browsers */
  justify-content: stretch;
}
.hbox.align-start,
.vbox.align-start,
.align-start {
  /* Old browsers */
  -webkit-box-align: start;
  -moz-box-align: start;
  box-align: start;
  /* Modern browsers */
  align-items: flex-start;
}
.hbox.align-end,
.vbox.align-end,
.align-end {
  /* Old browsers */
  -webkit-box-align: end;
  -moz-box-align: end;
  box-align: end;
  /* Modern browsers */
  align-items: flex-end;
}
.hbox.align-center,
.vbox.align-center,
.align-center {
  /* Old browsers */
  -webkit-box-align: center;
  -moz-box-align: center;
  box-align: center;
  /* Modern browsers */
  align-items: center;
}
.hbox.align-baseline,
.vbox.align-baseline,
.align-baseline {
  /* Old browsers */
  -webkit-box-align: baseline;
  -moz-box-align: baseline;
  box-align: baseline;
  /* Modern browsers */
  align-items: baseline;
}
.hbox.align-stretch,
.vbox.align-stretch,
.align-stretch {
  /* Old browsers */
  -webkit-box-align: stretch;
  -moz-box-align: stretch;
  box-align: stretch;
  /* Modern browsers */
  align-items: stretch;
}
div.error {
  margin: 2em;
  text-align: center;
}
div.error > h1 {
  font-size: 500%;
  line-height: normal;
}
div.error > p {
  font-size: 200%;
  line-height: normal;
}
div.traceback-wrapper {
  text-align: left;
  max-width: 800px;
  margin: auto;
}
div.traceback-wrapper pre.traceback {
  max-height: 600px;
  overflow: auto;
}
/**
 * Primary styles
 *
 * Author: Jupyter Development Team
 */
body {
  background-color: #fff;
  /* This makes sure that the body covers the entire window and needs to
       be in a different element than the display: box in wrapper below */
  position: absolute;
  left: 0px;
  right: 0px;
  top: 0px;
  bottom: 0px;
  overflow: visible;
}
body > #header {
  /* Initially hidden to prevent FLOUC */
  display: none;
  background-color: #fff;
  /* Display over codemirror */
  position: relative;
  z-index: 100;
}
body > #header #header-container {
  display: flex;
  flex-direction: row;
  justify-content: space-between;
  padding: 5px;
  padding-bottom: 5px;
  padding-top: 5px;
  box-sizing: border-box;
  -moz-box-sizing: border-box;
  -webkit-box-sizing: border-box;
}
body > #header .header-bar {
  width: 100%;
  height: 1px;
  background: #e7e7e7;
  margin-bottom: -1px;
}
@media print {
  body > #header {
    display: none !important;
  }
}
#header-spacer {
  width: 100%;
  visibility: hidden;
}
@media print {
  #header-spacer {
    display: none;
  }
}
#ipython_notebook {
  padding-left: 0px;
  padding-top: 1px;
  padding-bottom: 1px;
}
[dir="rtl"] #ipython_notebook {
  margin-right: 10px;
  margin-left: 0;
}
[dir="rtl"] #ipython_notebook.pull-left {
  float: right !important;
  float: right;
}
.flex-spacer {
  flex: 1;
}
#noscript {
  width: auto;
  padding-top: 16px;
  padding-bottom: 16px;
  text-align: center;
  font-size: 22px;
  color: red;
  font-weight: bold;
}
#ipython_notebook img {
  height: 28px;
}
#site {
  width: 100%;
  display: none;
  box-sizing: border-box;
  -moz-box-sizing: border-box;
  -webkit-box-sizing: border-box;
  overflow: auto;
}
@media print {
  #site {
    height: auto !important;
  }
}
/* Smaller buttons */
.ui-button .ui-button-text {
  padding: 0.2em 0.8em;
  font-size: 77%;
}
input.ui-button {
  padding: 0.3em 0.9em;
}
span#kernel_logo_widget {
  margin: 0 10px;
}
span#login_widget {
  float: right;
}
[dir="rtl"] span#login_widget {
  float: left;
}
span#login_widget > .button,
#logout {
  color: #333;
  background-color: #fff;
  border-color: #ccc;
}
span#login_widget > .button:focus,
#logout:focus,
span#login_widget > .button.focus,
#logout.focus {
  color: #333;
  background-color: #e6e6e6;
  border-color: #8c8c8c;
}
span#login_widget > .button:hover,
#logout:hover {
  color: #333;
  background-color: #e6e6e6;
  border-color: #adadad;
}
span#login_widget > .button:active,
#logout:active,
span#login_widget > .button.active,
#logout.active,
.open > .dropdown-togglespan#login_widget > .button,
.open > .dropdown-toggle#logout {
  color: #333;
  background-color: #e6e6e6;
  border-color: #adadad;
}
span#login_widget > .button:active:hover,
#logout:active:hover,
span#login_widget > .button.active:hover,
#logout.active:hover,
.open > .dropdown-togglespan#login_widget > .button:hover,
.open > .dropdown-toggle#logout:hover,
span#login_widget > .button:active:focus,
#logout:active:focus,
span#login_widget > .button.active:focus,
#logout.active:focus,
.open > .dropdown-togglespan#login_widget > .button:focus,
.open > .dropdown-toggle#logout:focus,
span#login_widget > .button:active.focus,
#logout:active.focus,
span#login_widget > .button.active.focus,
#logout.active.focus,
.open > .dropdown-togglespan#login_widget > .button.focus,
.open > .dropdown-toggle#logout.focus {
  color: #333;
  background-color: #d4d4d4;
  border-color: #8c8c8c;
}
span#login_widget > .button:active,
#logout:active,
span#login_widget > .button.active,
#logout.active,
.open > .dropdown-togglespan#login_widget > .button,
.open > .dropdown-toggle#logout {
  background-image: none;
}
span#login_widget > .button.disabled:hover,
#logout.disabled:hover,
span#login_widget > .button[disabled]:hover,
#logout[disabled]:hover,
fieldset[disabled] span#login_widget > .button:hover,
fieldset[disabled] #logout:hover,
span#login_widget > .button.disabled:focus,
#logout.disabled:focus,
span#login_widget > .button[disabled]:focus,
#logout[disabled]:focus,
fieldset[disabled] span#login_widget > .button:focus,
fieldset[disabled] #logout:focus,
span#login_widget > .button.disabled.focus,
#logout.disabled.focus,
span#login_widget > .button[disabled].focus,
#logout[disabled].focus,
fieldset[disabled] span#login_widget > .button.focus,
fieldset[disabled] #logout.focus {
  background-color: #fff;
  border-color: #ccc;
}
span#login_widget > .button .badge,
#logout .badge {
  color: #fff;
  background-color: #333;
}
.nav-header {
  text-transform: none;
}
#header > span {
  margin-top: 10px;
}
.modal_stretch .modal-dialog {
  /* Old browsers */
  display: -webkit-box;
  -webkit-box-orient: vertical;
  -webkit-box-align: stretch;
  display: -moz-box;
  -moz-box-orient: vertical;
  -moz-box-align: stretch;
  display: box;
  box-orient: vertical;
  box-align: stretch;
  /* Modern browsers */
  display: flex;
  flex-direction: column;
  align-items: stretch;
  min-height: 80vh;
}
.modal_stretch .modal-dialog .modal-body {
  max-height: calc(100vh - 200px);
  overflow: auto;
  flex: 1;
}
.modal-header {
  cursor: move;
}
@media (min-width: 768px) {
  .modal .modal-dialog {
    width: 700px;
  }
}
@media (min-width: 768px) {
  select.form-control {
    margin-left: 12px;
    margin-right: 12px;
  }
}
/*!
*
* IPython auth
*
*/
.center-nav {
  display: inline-block;
  margin-bottom: -4px;
}
[dir="rtl"] .center-nav form.pull-left {
  float: right !important;
  float: right;
}
[dir="rtl"] .center-nav .navbar-text {
  float: right;
}
[dir="rtl"] .navbar-inner {
  text-align: right;
}
[dir="rtl"] div.text-left {
  text-align: right;
}
/*!
*
* IPython tree view
*
*/
/* We need an invisible input field on top of the sentense*/
/* "Drag file onto the list ..." */
.alternate_upload {
  background-color: none;
  display: inline;
}
.alternate_upload.form {
  padding: 0;
  margin: 0;
}
.alternate_upload input.fileinput {
  position: absolute;
  display: block;
  width: 100%;
  height: 100%;
  overflow: hidden;
  cursor: pointer;
  opacity: 0;
  z-index: 2;
}
.alternate_upload .btn-xs > input.fileinput {
  margin: -1px -5px;
}
.alternate_upload .btn-upload {
  position: relative;
  height: 22px;
}
::-webkit-file-upload-button {
  cursor: pointer;
}
/**
 * Primary styles
 *
 * Author: Jupyter Development Team
 */
ul#tabs {
  margin-bottom: 4px;
}
ul#tabs a {
  padding-top: 6px;
  padding-bottom: 4px;
}
[dir="rtl"] ul#tabs.nav-tabs > li {
  float: right;
}
[dir="rtl"] ul#tabs.nav.nav-tabs {
  padding-right: 0;
}
ul.breadcrumb a:focus,
ul.breadcrumb a:hover {
  text-decoration: none;
}
ul.breadcrumb i.icon-home {
  font-size: 16px;
  margin-right: 4px;
}
ul.breadcrumb span {
  color: #5e5e5e;
}
.list_toolbar {
  padding: 4px 0 4px 0;
  vertical-align: middle;
}
.list_toolbar .tree-buttons {
  padding-top: 1px;
}
[dir="rtl"] .list_toolbar .tree-buttons .pull-right {
  float: left !important;
  float: left;
}
[dir="rtl"] .list_toolbar .col-sm-4,
[dir="rtl"] .list_toolbar .col-sm-8 {
  float: right;
}
.dynamic-buttons {
  padding-top: 3px;
  display: inline-block;
}
.list_toolbar [class*="span"] {
  min-height: 24px;
}
.list_header {
  font-weight: bold;
  background-color: #EEE;
}
.list_placeholder {
  font-weight: bold;
  padding-top: 4px;
  padding-bottom: 4px;
  padding-left: 7px;
  padding-right: 7px;
}
.list_container {
  margin-top: 4px;
  margin-bottom: 20px;
  border: 1px solid #ddd;
  border-radius: 2px;
}
.list_container > div {
  border-bottom: 1px solid #ddd;
}
.list_container > div:hover .list-item {
  background-color: red;
}
.list_container > div:last-child {
  border: none;
}
.list_item:hover .list_item {
  background-color: #ddd;
}
.list_item a {
  text-decoration: none;
}
.list_item:hover {
  background-color: #fafafa;
}
.list_header > div,
.list_item > div {
  padding-top: 4px;
  padding-bottom: 4px;
  padding-left: 7px;
  padding-right: 7px;
  line-height: 22px;
}
.list_header > div input,
.list_item > div input {
  margin-right: 7px;
  margin-left: 14px;
  vertical-align: text-bottom;
  line-height: 22px;
  position: relative;
  top: -1px;
}
.list_header > div .item_link,
.list_item > div .item_link {
  margin-left: -1px;
  vertical-align: baseline;
  line-height: 22px;
}
[dir="rtl"] .list_item > div input {
  margin-right: 0;
}
.new-file input[type=checkbox] {
  visibility: hidden;
}
.item_name {
  line-height: 22px;
  height: 24px;
}
.item_icon {
  font-size: 14px;
  color: #5e5e5e;
  margin-right: 7px;
  margin-left: 7px;
  line-height: 22px;
  vertical-align: baseline;
}
.item_modified {
  margin-right: 7px;
  margin-left: 7px;
}
[dir="rtl"] .item_modified.pull-right {
  float: left !important;
  float: left;
}
.item_buttons {
  line-height: 1em;
  margin-left: -5px;
}
.item_buttons .btn,
.item_buttons .btn-group,
.item_buttons .input-group {
  float: left;
}
.item_buttons > .btn,
.item_buttons > .btn-group,
.item_buttons > .input-group {
  margin-left: 5px;
}
.item_buttons .btn {
  min-width: 13ex;
}
.item_buttons .running-indicator {
  padding-top: 4px;
  color: #5cb85c;
}
.item_buttons .kernel-name {
  padding-top: 4px;
  color: #5bc0de;
  margin-right: 7px;
  float: left;
}
[dir="rtl"] .item_buttons.pull-right {
  float: left !important;
  float: left;
}
[dir="rtl"] .item_buttons .kernel-name {
  margin-left: 7px;
  float: right;
}
.toolbar_info {
  height: 24px;
  line-height: 24px;
}
.list_item input:not([type=checkbox]) {
  padding-top: 3px;
  padding-bottom: 3px;
  height: 22px;
  line-height: 14px;
  margin: 0px;
}
.highlight_text {
  color: blue;
}
#project_name {
  display: inline-block;
  padding-left: 7px;
  margin-left: -2px;
}
#project_name > .breadcrumb {
  padding: 0px;
  margin-bottom: 0px;
  background-color: transparent;
  font-weight: bold;
}
.sort_button {
  display: inline-block;
  padding-left: 7px;
}
[dir="rtl"] .sort_button.pull-right {
  float: left !important;
  float: left;
}
#tree-selector {
  padding-right: 0px;
}
#button-select-all {
  min-width: 50px;
}
[dir="rtl"] #button-select-all.btn {
  float: right ;
}
#select-all {
  margin-left: 7px;
  margin-right: 2px;
  margin-top: 2px;
  height: 16px;
}
[dir="rtl"] #select-all.pull-left {
  float: right !important;
  float: right;
}
.menu_icon {
  margin-right: 2px;
}
.tab-content .row {
  margin-left: 0px;
  margin-right: 0px;
}
.folder_icon:before {
  display: inline-block;
  font: normal normal normal 14px/1 FontAwesome;
  font-size: inherit;
  text-rendering: auto;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  content: "\f114";
}
.folder_icon:before.fa-pull-left {
  margin-right: .3em;
}
.folder_icon:before.fa-pull-right {
  margin-left: .3em;
}
.folder_icon:before.pull-left {
  margin-right: .3em;
}
.folder_icon:before.pull-right {
  margin-left: .3em;
}
.notebook_icon:before {
  display: inline-block;
  font: normal normal normal 14px/1 FontAwesome;
  font-size: inherit;
  text-rendering: auto;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  content: "\f02d";
  position: relative;
  top: -1px;
}
.notebook_icon:before.fa-pull-left {
  margin-right: .3em;
}
.notebook_icon:before.fa-pull-right {
  margin-left: .3em;
}
.notebook_icon:before.pull-left {
  margin-right: .3em;
}
.notebook_icon:before.pull-right {
  margin-left: .3em;
}
.running_notebook_icon:before {
  display: inline-block;
  font: normal normal normal 14px/1 FontAwesome;
  font-size: inherit;
  text-rendering: auto;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  content: "\f02d";
  position: relative;
  top: -1px;
  color: #5cb85c;
}
.running_notebook_icon:before.fa-pull-left {
  margin-right: .3em;
}
.running_notebook_icon:before.fa-pull-right {
  margin-left: .3em;
}
.running_notebook_icon:before.pull-left {
  margin-right: .3em;
}
.running_notebook_icon:before.pull-right {
  margin-left: .3em;
}
.file_icon:before {
  display: inline-block;
  font: normal normal normal 14px/1 FontAwesome;
  font-size: inherit;
  text-rendering: auto;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  content: "\f016";
  position: relative;
  top: -2px;
}
.file_icon:before.fa-pull-left {
  margin-right: .3em;
}
.file_icon:before.fa-pull-right {
  margin-left: .3em;
}
.file_icon:before.pull-left {
  margin-right: .3em;
}
.file_icon:before.pull-right {
  margin-left: .3em;
}
#notebook_toolbar .pull-right {
  padding-top: 0px;
  margin-right: -1px;
}
ul#new-menu {
  left: auto;
  right: 0;
}
#new-menu .dropdown-header {
  font-size: 10px;
  border-bottom: 1px solid #e5e5e5;
  padding: 0 0 3px;
  margin: -3px 20px 0;
}
.kernel-menu-icon {
  padding-right: 12px;
  width: 24px;
  content: "\f096";
}
.kernel-menu-icon:before {
  content: "\f096";
}
.kernel-menu-icon-current:before {
  content: "\f00c";
}
#tab_content {
  padding-top: 20px;
}
#running .panel-group .panel {
  margin-top: 3px;
  margin-bottom: 1em;
}
#running .panel-group .panel .panel-heading {
  background-color: #EEE;
  padding-top: 4px;
  padding-bottom: 4px;
  padding-left: 7px;
  padding-right: 7px;
  line-height: 22px;
}
#running .panel-group .panel .panel-heading a:focus,
#running .panel-group .panel .panel-heading a:hover {
  text-decoration: none;
}
#running .panel-group .panel .panel-body {
  padding: 0px;
}
#running .panel-group .panel .panel-body .list_container {
  margin-top: 0px;
  margin-bottom: 0px;
  border: 0px;
  border-radius: 0px;
}
#running .panel-group .panel .panel-body .list_container .list_item {
  border-bottom: 1px solid #ddd;
}
#running .panel-group .panel .panel-body .list_container .list_item:last-child {
  border-bottom: 0px;
}
.delete-button {
  display: none;
}
.duplicate-button {
  display: none;
}
.rename-button {
  display: none;
}
.move-button {
  display: none;
}
.download-button {
  display: none;
}
.shutdown-button {
  display: none;
}
.dynamic-instructions {
  display: inline-block;
  padding-top: 4px;
}
/*!
*
* IPython text editor webapp
*
*/
.selected-keymap i.fa {
  padding: 0px 5px;
}
.selected-keymap i.fa:before {
  content: "\f00c";
}
#mode-menu {
  overflow: auto;
  max-height: 20em;
}
.edit_app #header {
  -webkit-box-shadow: 0px 0px 12px 1px rgba(87, 87, 87, 0.2);
  box-shadow: 0px 0px 12px 1px rgba(87, 87, 87, 0.2);
}
.edit_app #menubar .navbar {
  /* Use a negative 1 bottom margin, so the border overlaps the border of the
    header */
  margin-bottom: -1px;
}
.dirty-indicator {
  display: inline-block;
  font: normal normal normal 14px/1 FontAwesome;
  font-size: inherit;
  text-rendering: auto;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  width: 20px;
}
.dirty-indicator.fa-pull-left {
  margin-right: .3em;
}
.dirty-indicator.fa-pull-right {
  margin-left: .3em;
}
.dirty-indicator.pull-left {
  margin-right: .3em;
}
.dirty-indicator.pull-right {
  margin-left: .3em;
}
.dirty-indicator-dirty {
  display: inline-block;
  font: normal normal normal 14px/1 FontAwesome;
  font-size: inherit;
  text-rendering: auto;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  width: 20px;
}
.dirty-indicator-dirty.fa-pull-left {
  margin-right: .3em;
}
.dirty-indicator-dirty.fa-pull-right {
  margin-left: .3em;
}
.dirty-indicator-dirty.pull-left {
  margin-right: .3em;
}
.dirty-indicator-dirty.pull-right {
  margin-left: .3em;
}
.dirty-indicator-clean {
  display: inline-block;
  font: normal normal normal 14px/1 FontAwesome;
  font-size: inherit;
  text-rendering: auto;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  width: 20px;
}
.dirty-indicator-clean.fa-pull-left {
  margin-right: .3em;
}
.dirty-indicator-clean.fa-pull-right {
  margin-left: .3em;
}
.dirty-indicator-clean.pull-left {
  margin-right: .3em;
}
.dirty-indicator-clean.pull-right {
  margin-left: .3em;
}
.dirty-indicator-clean:before {
  display: inline-block;
  font: normal normal normal 14px/1 FontAwesome;
  font-size: inherit;
  text-rendering: auto;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  content: "\f00c";
}
.dirty-indicator-clean:before.fa-pull-left {
  margin-right: .3em;
}
.dirty-indicator-clean:before.fa-pull-right {
  margin-left: .3em;
}
.dirty-indicator-clean:before.pull-left {
  margin-right: .3em;
}
.dirty-indicator-clean:before.pull-right {
  margin-left: .3em;
}
#filename {
  font-size: 16pt;
  display: table;
  padding: 0px 5px;
}
#current-mode {
  padding-left: 5px;
  padding-right: 5px;
}
#texteditor-backdrop {
  padding-top: 20px;
  padding-bottom: 20px;
}
@media not print {
  #texteditor-backdrop {
    background-color: #EEE;
  }
}
@media print {
  #texteditor-backdrop #texteditor-container .CodeMirror-gutter,
  #texteditor-backdrop #texteditor-container .CodeMirror-gutters {
    background-color: #fff;
  }
}
@media not print {
  #texteditor-backdrop #texteditor-container .CodeMirror-gutter,
  #texteditor-backdrop #texteditor-container .CodeMirror-gutters {
    background-color: #fff;
  }
}
@media not print {
  #texteditor-backdrop #texteditor-container {
    padding: 0px;
    background-color: #fff;
    -webkit-box-shadow: 0px 0px 12px 1px rgba(87, 87, 87, 0.2);
    box-shadow: 0px 0px 12px 1px rgba(87, 87, 87, 0.2);
  }
}
.CodeMirror-dialog {
  background-color: #fff;
}
/*!
*
* IPython notebook
*
*/
/* CSS font colors for translated ANSI escape sequences */
/* The color values are a mix of
   http://www.xcolors.net/dl/baskerville-ivorylight and
   http://www.xcolors.net/dl/euphrasia */
.ansi-black-fg {
  color: #3E424D;
}
.ansi-black-bg {
  background-color: #3E424D;
}
.ansi-black-intense-fg {
  color: #282C36;
}
.ansi-black-intense-bg {
  background-color: #282C36;
}
.ansi-red-fg {
  color: #E75C58;
}
.ansi-red-bg {
  background-color: #E75C58;
}
.ansi-red-intense-fg {
  color: #B22B31;
}
.ansi-red-intense-bg {
  background-color: #B22B31;
}
.ansi-green-fg {
  color: #00A250;
}
.ansi-green-bg {
  background-color: #00A250;
}
.ansi-green-intense-fg {
  color: #007427;
}
.ansi-green-intense-bg {
  background-color: #007427;
}
.ansi-yellow-fg {
  color: #DDB62B;
}
.ansi-yellow-bg {
  background-color: #DDB62B;
}
.ansi-yellow-intense-fg {
  color: #B27D12;
}
.ansi-yellow-intense-bg {
  background-color: #B27D12;
}
.ansi-blue-fg {
  color: #208FFB;
}
.ansi-blue-bg {
  background-color: #208FFB;
}
.ansi-blue-intense-fg {
  color: #0065CA;
}
.ansi-blue-intense-bg {
  background-color: #0065CA;
}
.ansi-magenta-fg {
  color: #D160C4;
}
.ansi-magenta-bg {
  background-color: #D160C4;
}
.ansi-magenta-intense-fg {
  color: #A03196;
}
.ansi-magenta-intense-bg {
  background-color: #A03196;
}
.ansi-cyan-fg {
  color: #60C6C8;
}
.ansi-cyan-bg {
  background-color: #60C6C8;
}
.ansi-cyan-intense-fg {
  color: #258F8F;
}
.ansi-cyan-intense-bg {
  background-color: #258F8F;
}
.ansi-white-fg {
  color: #C5C1B4;
}
.ansi-white-bg {
  background-color: #C5C1B4;
}
.ansi-white-intense-fg {
  color: #A1A6B2;
}
.ansi-white-intense-bg {
  background-color: #A1A6B2;
}
.ansi-default-inverse-fg {
  color: #FFFFFF;
}
.ansi-default-inverse-bg {
  background-color: #000000;
}
.ansi-bold {
  font-weight: bold;
}
.ansi-underline {
  text-decoration: underline;
}
/* The following styles are deprecated an will be removed in a future version */
.ansibold {
  font-weight: bold;
}
.ansi-inverse {
  outline: 0.5px dotted;
}
/* use dark versions for foreground, to improve visibility */
.ansiblack {
  color: black;
}
.ansired {
  color: darkred;
}
.ansigreen {
  color: darkgreen;
}
.ansiyellow {
  color: #c4a000;
}
.ansiblue {
  color: darkblue;
}
.ansipurple {
  color: darkviolet;
}
.ansicyan {
  color: steelblue;
}
.ansigray {
  color: gray;
}
/* and light for background, for the same reason */
.ansibgblack {
  background-color: black;
}
.ansibgred {
  background-color: red;
}
.ansibggreen {
  background-color: green;
}
.ansibgyellow {
  background-color: yellow;
}
.ansibgblue {
  background-color: blue;
}
.ansibgpurple {
  background-color: magenta;
}
.ansibgcyan {
  background-color: cyan;
}
.ansibggray {
  background-color: gray;
}
div.cell {
  /* Old browsers */
  display: -webkit-box;
  -webkit-box-orient: vertical;
  -webkit-box-align: stretch;
  display: -moz-box;
  -moz-box-orient: vertical;
  -moz-box-align: stretch;
  display: box;
  box-orient: vertical;
  box-align: stretch;
  /* Modern browsers */
  display: flex;
  flex-direction: column;
  align-items: stretch;
  border-radius: 2px;
  box-sizing: border-box;
  -moz-box-sizing: border-box;
  -webkit-box-sizing: border-box;
  border-width: 1px;
  border-style: solid;
  border-color: transparent;
  width: 100%;
  padding: 5px;
  /* This acts as a spacer between cells, that is outside the border */
  margin: 0px;
  outline: none;
  position: relative;
  overflow: visible;
}
div.cell:before {
  position: absolute;
  display: block;
  top: -1px;
  left: -1px;
  width: 5px;
  height: calc(100% +  2px);
  content: '';
  background: transparent;
}
div.cell.jupyter-soft-selected {
  border-left-color: #E3F2FD;
  border-left-width: 1px;
  padding-left: 5px;
  border-right-color: #E3F2FD;
  border-right-width: 1px;
  background: #E3F2FD;
}
@media print {
  div.cell.jupyter-soft-selected {
    border-color: transparent;
  }
}
div.cell.selected,
div.cell.selected.jupyter-soft-selected {
  border-color: #ababab;
}
div.cell.selected:before,
div.cell.selected.jupyter-soft-selected:before {
  position: absolute;
  display: block;
  top: -1px;
  left: -1px;
  width: 5px;
  height: calc(100% +  2px);
  content: '';
  background: #42A5F5;
}
@media print {
  div.cell.selected,
  div.cell.selected.jupyter-soft-selected {
    border-color: transparent;
  }
}
.edit_mode div.cell.selected {
  border-color: #66BB6A;
}
.edit_mode div.cell.selected:before {
  position: absolute;
  display: block;
  top: -1px;
  left: -1px;
  width: 5px;
  height: calc(100% +  2px);
  content: '';
  background: #66BB6A;
}
@media print {
  .edit_mode div.cell.selected {
    border-color: transparent;
  }
}
.prompt {
  /* This needs to be wide enough for 3 digit prompt numbers: In[100]: */
  min-width: 14ex;
  /* This padding is tuned to match the padding on the CodeMirror editor. */
  padding: 0.4em;
  margin: 0px;
  font-family: monospace;
  text-align: right;
  /* This has to match that of the the CodeMirror class line-height below */
  line-height: 1.21429em;
  /* Don't highlight prompt number selection */
  -webkit-touch-callout: none;
  -webkit-user-select: none;
  -khtml-user-select: none;
  -moz-user-select: none;
  -ms-user-select: none;
  user-select: none;
  /* Use default cursor */
  cursor: default;
}
@media (max-width: 540px) {
  .prompt {
    text-align: left;
  }
}
div.inner_cell {
  min-width: 0;
  /* Old browsers */
  display: -webkit-box;
  -webkit-box-orient: vertical;
  -webkit-box-align: stretch;
  display: -moz-box;
  -moz-box-orient: vertical;
  -moz-box-align: stretch;
  display: box;
  box-orient: vertical;
  box-align: stretch;
  /* Modern browsers */
  display: flex;
  flex-direction: column;
  align-items: stretch;
  /* Old browsers */
  -webkit-box-flex: 1;
  -moz-box-flex: 1;
  box-flex: 1;
  /* Modern browsers */
  flex: 1;
}
/* input_area and input_prompt must match in top border and margin for alignment */
div.input_area {
  border: 1px solid #cfcfcf;
  border-radius: 2px;
  background: #f7f7f7;
  line-height: 1.21429em;
}
/* This is needed so that empty prompt areas can collapse to zero height when there
   is no content in the output_subarea and the prompt. The main purpose of this is
   to make sure that empty JavaScript output_subareas have no height. */
div.prompt:empty {
  padding-top: 0;
  padding-bottom: 0;
}
div.unrecognized_cell {
  padding: 5px 5px 5px 0px;
  /* Old browsers */
  display: -webkit-box;
  -webkit-box-orient: horizontal;
  -webkit-box-align: stretch;
  display: -moz-box;
  -moz-box-orient: horizontal;
  -moz-box-align: stretch;
  display: box;
  box-orient: horizontal;
  box-align: stretch;
  /* Modern browsers */
  display: flex;
  flex-direction: row;
  align-items: stretch;
}
div.unrecognized_cell .inner_cell {
  border-radius: 2px;
  padding: 5px;
  font-weight: bold;
  color: red;
  border: 1px solid #cfcfcf;
  background: #eaeaea;
}
div.unrecognized_cell .inner_cell a {
  color: inherit;
  text-decoration: none;
}
div.unrecognized_cell .inner_cell a:hover {
  color: inherit;
  text-decoration: none;
}
@media (max-width: 540px) {
  div.unrecognized_cell > div.prompt {
    display: none;
  }
}
div.code_cell {
  /* avoid page breaking on code cells when printing */
}
@media print {
  div.code_cell {
    page-break-inside: avoid;
  }
}
/* any special styling for code cells that are currently running goes here */
div.input {
  page-break-inside: avoid;
  /* Old browsers */
  display: -webkit-box;
  -webkit-box-orient: horizontal;
  -webkit-box-align: stretch;
  display: -moz-box;
  -moz-box-orient: horizontal;
  -moz-box-align: stretch;
  display: box;
  box-orient: horizontal;
  box-align: stretch;
  /* Modern browsers */
  display: flex;
  flex-direction: row;
  align-items: stretch;
}
@media (max-width: 540px) {
  div.input {
    /* Old browsers */
    display: -webkit-box;
    -webkit-box-orient: vertical;
    -webkit-box-align: stretch;
    display: -moz-box;
    -moz-box-orient: vertical;
    -moz-box-align: stretch;
    display: box;
    box-orient: vertical;
    box-align: stretch;
    /* Modern browsers */
    display: flex;
    flex-direction: column;
    align-items: stretch;
  }
}
/* input_area and input_prompt must match in top border and margin for alignment */
div.input_prompt {
  color: #303F9F;
  border-top: 1px solid transparent;
}
div.input_area > div.highlight {
  margin: 0.4em;
  border: none;
  padding: 0px;
  background-color: transparent;
}
div.input_area > div.highlight > pre {
  margin: 0px;
  border: none;
  padding: 0px;
  background-color: transparent;
}
/* The following gets added to the <head> if it is detected that the user has a
 * monospace font with inconsistent normal/bold/italic height.  See
 * notebookmain.js.  Such fonts will have keywords vertically offset with
 * respect to the rest of the text.  The user should select a better font.
 * See: https://github.com/ipython/ipython/issues/1503
 *
 * .CodeMirror span {
 *      vertical-align: bottom;
 * }
 */
.CodeMirror {
  line-height: 1.21429em;
  /* Changed from 1em to our global default */
  font-size: 14px;
  height: auto;
  /* Changed to auto to autogrow */
  background: none;
  /* Changed from white to allow our bg to show through */
}
.CodeMirror-scroll {
  /*  The CodeMirror docs are a bit fuzzy on if overflow-y should be hidden or visible.*/
  /*  We have found that if it is visible, vertical scrollbars appear with font size changes.*/
  overflow-y: hidden;
  overflow-x: auto;
}
.CodeMirror-lines {
  /* In CM2, this used to be 0.4em, but in CM3 it went to 4px. We need the em value because */
  /* we have set a different line-height and want this to scale with that. */
  /* Note that this should set vertical padding only, since CodeMirror assumes
       that horizontal padding will be set on CodeMirror pre */
  padding: 0.4em 0;
}
.CodeMirror-linenumber {
  padding: 0 8px 0 4px;
}
.CodeMirror-gutters {
  border-bottom-left-radius: 2px;
  border-top-left-radius: 2px;
}
.CodeMirror pre {
  /* In CM3 this went to 4px from 0 in CM2. This sets horizontal padding only,
    use .CodeMirror-lines for vertical */
  padding: 0 0.4em;
  border: 0;
  border-radius: 0;
}
.CodeMirror-cursor {
  border-left: 1.4px solid black;
}
@media screen and (min-width: 2138px) and (max-width: 4319px) {
  .CodeMirror-cursor {
    border-left: 2px solid black;
  }
}
@media screen and (min-width: 4320px) {
  .CodeMirror-cursor {
    border-left: 4px solid black;
  }
}
/*

Original style from softwaremaniacs.org (c) Ivan Sagalaev <Maniac@SoftwareManiacs.Org>
Adapted from GitHub theme

*/
.highlight-base {
  color: #000;
}
.highlight-variable {
  color: #000;
}
.highlight-variable-2 {
  color: #1a1a1a;
}
.highlight-variable-3 {
  color: #333333;
}
.highlight-string {
  color: #BA2121;
}
.highlight-comment {
  color: #408080;
  font-style: italic;
}
.highlight-number {
  color: #080;
}
.highlight-atom {
  color: #88F;
}
.highlight-keyword {
  color: #008000;
  font-weight: bold;
}
.highlight-builtin {
  color: #008000;
}
.highlight-error {
  color: #f00;
}
.highlight-operator {
  color: #AA22FF;
  font-weight: bold;
}
.highlight-meta {
  color: #AA22FF;
}
/* previously not defined, copying from default codemirror */
.highlight-def {
  color: #00f;
}
.highlight-string-2 {
  color: #f50;
}
.highlight-qualifier {
  color: #555;
}
.highlight-bracket {
  color: #997;
}
.highlight-tag {
  color: #170;
}
.highlight-attribute {
  color: #00c;
}
.highlight-header {
  color: blue;
}
.highlight-quote {
  color: #090;
}
.highlight-link {
  color: #00c;
}
/* apply the same style to codemirror */
.cm-s-ipython span.cm-keyword {
  color: #008000;
  font-weight: bold;
}
.cm-s-ipython span.cm-atom {
  color: #88F;
}
.cm-s-ipython span.cm-number {
  color: #080;
}
.cm-s-ipython span.cm-def {
  color: #00f;
}
.cm-s-ipython span.cm-variable {
  color: #000;
}
.cm-s-ipython span.cm-operator {
  color: #AA22FF;
  font-weight: bold;
}
.cm-s-ipython span.cm-variable-2 {
  color: #1a1a1a;
}
.cm-s-ipython span.cm-variable-3 {
  color: #333333;
}
.cm-s-ipython span.cm-comment {
  color: #408080;
  font-style: italic;
}
.cm-s-ipython span.cm-string {
  color: #BA2121;
}
.cm-s-ipython span.cm-string-2 {
  color: #f50;
}
.cm-s-ipython span.cm-meta {
  color: #AA22FF;
}
.cm-s-ipython span.cm-qualifier {
  color: #555;
}
.cm-s-ipython span.cm-builtin {
  color: #008000;
}
.cm-s-ipython span.cm-bracket {
  color: #997;
}
.cm-s-ipython span.cm-tag {
  color: #170;
}
.cm-s-ipython span.cm-attribute {
  color: #00c;
}
.cm-s-ipython span.cm-header {
  color: blue;
}
.cm-s-ipython span.cm-quote {
  color: #090;
}
.cm-s-ipython span.cm-link {
  color: #00c;
}
.cm-s-ipython span.cm-error {
  color: #f00;
}
.cm-s-ipython span.cm-tab {
  background: url(data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAADAAAAAMCAYAAAAkuj5RAAAAAXNSR0IArs4c6QAAAGFJREFUSMft1LsRQFAQheHPowAKoACx3IgEKtaEHujDjORSgWTH/ZOdnZOcM/sgk/kFFWY0qV8foQwS4MKBCS3qR6ixBJvElOobYAtivseIE120FaowJPN75GMu8j/LfMwNjh4HUpwg4LUAAAAASUVORK5CYII=);
  background-position: right;
  background-repeat: no-repeat;
}
div.output_wrapper {
  /* this position must be relative to enable descendents to be absolute within it */
  position: relative;
  /* Old browsers */
  display: -webkit-box;
  -webkit-box-orient: vertical;
  -webkit-box-align: stretch;
  display: -moz-box;
  -moz-box-orient: vertical;
  -moz-box-align: stretch;
  display: box;
  box-orient: vertical;
  box-align: stretch;
  /* Modern browsers */
  display: flex;
  flex-direction: column;
  align-items: stretch;
  z-index: 1;
}
/* class for the output area when it should be height-limited */
div.output_scroll {
  /* ideally, this would be max-height, but FF barfs all over that */
  height: 24em;
  /* FF needs this *and the wrapper* to specify full width, or it will shrinkwrap */
  width: 100%;
  overflow: auto;
  border-radius: 2px;
  -webkit-box-shadow: inset 0 2px 8px rgba(0, 0, 0, 0.8);
  box-shadow: inset 0 2px 8px rgba(0, 0, 0, 0.8);
  display: block;
}
/* output div while it is collapsed */
div.output_collapsed {
  margin: 0px;
  padding: 0px;
  /* Old browsers */
  display: -webkit-box;
  -webkit-box-orient: vertical;
  -webkit-box-align: stretch;
  display: -moz-box;
  -moz-box-orient: vertical;
  -moz-box-align: stretch;
  display: box;
  box-orient: vertical;
  box-align: stretch;
  /* Modern browsers */
  display: flex;
  flex-direction: column;
  align-items: stretch;
}
div.out_prompt_overlay {
  height: 100%;
  padding: 0px 0.4em;
  position: absolute;
  border-radius: 2px;
}
div.out_prompt_overlay:hover {
  /* use inner shadow to get border that is computed the same on WebKit/FF */
  -webkit-box-shadow: inset 0 0 1px #000;
  box-shadow: inset 0 0 1px #000;
  background: rgba(240, 240, 240, 0.5);
}
div.output_prompt {
  color: #D84315;
}
/* This class is the outer container of all output sections. */
div.output_area {
  padding: 0px;
  page-break-inside: avoid;
  /* Old browsers */
  display: -webkit-box;
  -webkit-box-orient: horizontal;
  -webkit-box-align: stretch;
  display: -moz-box;
  -moz-box-orient: horizontal;
  -moz-box-align: stretch;
  display: box;
  box-orient: horizontal;
  box-align: stretch;
  /* Modern browsers */
  display: flex;
  flex-direction: row;
  align-items: stretch;
}
div.output_area .MathJax_Display {
  text-align: left !important;
}
div.output_area .rendered_html table {
  margin-left: 0;
  margin-right: 0;
}
div.output_area .rendered_html img {
  margin-left: 0;
  margin-right: 0;
}
div.output_area img,
div.output_area svg {
  max-width: 100%;
  height: auto;
}
div.output_area img.unconfined,
div.output_area svg.unconfined {
  max-width: none;
}
div.output_area .mglyph > img {
  max-width: none;
}
/* This is needed to protect the pre formating from global settings such
   as that of bootstrap */
.output {
  /* Old browsers */
  display: -webkit-box;
  -webkit-box-orient: vertical;
  -webkit-box-align: stretch;
  display: -moz-box;
  -moz-box-orient: vertical;
  -moz-box-align: stretch;
  display: box;
  box-orient: vertical;
  box-align: stretch;
  /* Modern browsers */
  display: flex;
  flex-direction: column;
  align-items: stretch;
}
@media (max-width: 540px) {
  div.output_area {
    /* Old browsers */
    display: -webkit-box;
    -webkit-box-orient: vertical;
    -webkit-box-align: stretch;
    display: -moz-box;
    -moz-box-orient: vertical;
    -moz-box-align: stretch;
    display: box;
    box-orient: vertical;
    box-align: stretch;
    /* Modern browsers */
    display: flex;
    flex-direction: column;
    align-items: stretch;
  }
}
div.output_area pre {
  margin: 0;
  padding: 1px 0 1px 0;
  border: 0;
  vertical-align: baseline;
  color: black;
  background-color: transparent;
  border-radius: 0;
}
/* This class is for the output subarea inside the output_area and after
   the prompt div. */
div.output_subarea {
  overflow-x: auto;
  padding: 0.4em;
  /* Old browsers */
  -webkit-box-flex: 1;
  -moz-box-flex: 1;
  box-flex: 1;
  /* Modern browsers */
  flex: 1;
  max-width: calc(100% - 14ex);
}
div.output_scroll div.output_subarea {
  overflow-x: visible;
}
/* The rest of the output_* classes are for special styling of the different
   output types */
/* all text output has this class: */
div.output_text {
  text-align: left;
  color: #000;
  /* This has to match that of the the CodeMirror class line-height below */
  line-height: 1.21429em;
}
/* stdout/stderr are 'text' as well as 'stream', but execute_result/error are *not* streams */
div.output_stderr {
  background: #fdd;
  /* very light red background for stderr */
}
div.output_latex {
  text-align: left;
}
/* Empty output_javascript divs should have no height */
div.output_javascript:empty {
  padding: 0;
}
.js-error {
  color: darkred;
}
/* raw_input styles */
div.raw_input_container {
  line-height: 1.21429em;
  padding-top: 5px;
}
pre.raw_input_prompt {
  /* nothing needed here. */
}
input.raw_input {
  font-family: monospace;
  font-size: inherit;
  color: inherit;
  width: auto;
  /* make sure input baseline aligns with prompt */
  vertical-align: baseline;
  /* padding + margin = 0.5em between prompt and cursor */
  padding: 0em 0.25em;
  margin: 0em 0.25em;
}
input.raw_input:focus {
  box-shadow: none;
}
p.p-space {
  margin-bottom: 10px;
}
div.output_unrecognized {
  padding: 5px;
  font-weight: bold;
  color: red;
}
div.output_unrecognized a {
  color: inherit;
  text-decoration: none;
}
div.output_unrecognized a:hover {
  color: inherit;
  text-decoration: none;
}
.rendered_html {
  color: #000;
  /* any extras will just be numbers: */
}
.rendered_html em {
  font-style: italic;
}
.rendered_html strong {
  font-weight: bold;
}
.rendered_html u {
  text-decoration: underline;
}
.rendered_html :link {
  text-decoration: underline;
}
.rendered_html :visited {
  text-decoration: underline;
}
.rendered_html h1 {
  font-size: 185.7%;
  margin: 1.08em 0 0 0;
  font-weight: bold;
  line-height: 1.0;
}
.rendered_html h2 {
  font-size: 157.1%;
  margin: 1.27em 0 0 0;
  font-weight: bold;
  line-height: 1.0;
}
.rendered_html h3 {
  font-size: 128.6%;
  margin: 1.55em 0 0 0;
  font-weight: bold;
  line-height: 1.0;
}
.rendered_html h4 {
  font-size: 100%;
  margin: 2em 0 0 0;
  font-weight: bold;
  line-height: 1.0;
}
.rendered_html h5 {
  font-size: 100%;
  margin: 2em 0 0 0;
  font-weight: bold;
  line-height: 1.0;
  font-style: italic;
}
.rendered_html h6 {
  font-size: 100%;
  margin: 2em 0 0 0;
  font-weight: bold;
  line-height: 1.0;
  font-style: italic;
}
.rendered_html h1:first-child {
  margin-top: 0.538em;
}
.rendered_html h2:first-child {
  margin-top: 0.636em;
}
.rendered_html h3:first-child {
  margin-top: 0.777em;
}
.rendered_html h4:first-child {
  margin-top: 1em;
}
.rendered_html h5:first-child {
  margin-top: 1em;
}
.rendered_html h6:first-child {
  margin-top: 1em;
}
.rendered_html ul:not(.list-inline),
.rendered_html ol:not(.list-inline) {
  padding-left: 2em;
}
.rendered_html ul {
  list-style: disc;
}
.rendered_html ul ul {
  list-style: square;
  margin-top: 0;
}
.rendered_html ul ul ul {
  list-style: circle;
}
.rendered_html ol {
  list-style: decimal;
}
.rendered_html ol ol {
  list-style: upper-alpha;
  margin-top: 0;
}
.rendered_html ol ol ol {
  list-style: lower-alpha;
}
.rendered_html ol ol ol ol {
  list-style: lower-roman;
}
.rendered_html ol ol ol ol ol {
  list-style: decimal;
}
.rendered_html * + ul {
  margin-top: 1em;
}
.rendered_html * + ol {
  margin-top: 1em;
}
.rendered_html hr {
  color: black;
  background-color: black;
}
.rendered_html pre {
  margin: 1em 2em;
  padding: 0px;
  background-color: #fff;
}
.rendered_html code {
  background-color: #eff0f1;
}
.rendered_html p code {
  padding: 1px 5px;
}
.rendered_html pre code {
  background-color: #fff;
}
.rendered_html pre,
.rendered_html code {
  border: 0;
  color: #000;
  font-size: 100%;
}
.rendered_html blockquote {
  margin: 1em 2em;
}
.rendered_html table {
  margin-left: auto;
  margin-right: auto;
  border: none;
  border-collapse: collapse;
  border-spacing: 0;
  color: black;
  font-size: 12px;
  table-layout: fixed;
}
.rendered_html thead {
  border-bottom: 1px solid black;
  vertical-align: bottom;
}
.rendered_html tr,
.rendered_html th,
.rendered_html td {
  text-align: right;
  vertical-align: middle;
  padding: 0.5em 0.5em;
  line-height: normal;
  white-space: normal;
  max-width: none;
  border: none;
}
.rendered_html th {
  font-weight: bold;
}
.rendered_html tbody tr:nth-child(odd) {
  background: #f5f5f5;
}
.rendered_html tbody tr:hover {
  background: rgba(66, 165, 245, 0.2);
}
.rendered_html * + table {
  margin-top: 1em;
}
.rendered_html p {
  text-align: left;
}
.rendered_html * + p {
  margin-top: 1em;
}
.rendered_html img {
  display: block;
  margin-left: auto;
  margin-right: auto;
}
.rendered_html * + img {
  margin-top: 1em;
}
.rendered_html img,
.rendered_html svg {
  max-width: 100%;
  height: auto;
}
.rendered_html img.unconfined,
.rendered_html svg.unconfined {
  max-width: none;
}
.rendered_html .alert {
  margin-bottom: initial;
}
.rendered_html * + .alert {
  margin-top: 1em;
}
[dir="rtl"] .rendered_html p {
  text-align: right;
}
div.text_cell {
  /* Old browsers */
  display: -webkit-box;
  -webkit-box-orient: horizontal;
  -webkit-box-align: stretch;
  display: -moz-box;
  -moz-box-orient: horizontal;
  -moz-box-align: stretch;
  display: box;
  box-orient: horizontal;
  box-align: stretch;
  /* Modern browsers */
  display: flex;
  flex-direction: row;
  align-items: stretch;
}
@media (max-width: 540px) {
  div.text_cell > div.prompt {
    display: none;
  }
}
div.text_cell_render {
  /*font-family: "Helvetica Neue", Arial, Helvetica, Geneva, sans-serif;*/
  outline: none;
  resize: none;
  width: inherit;
  border-style: none;
  padding: 0.5em 0.5em 0.5em 0.4em;
  color: #000;
  box-sizing: border-box;
  -moz-box-sizing: border-box;
  -webkit-box-sizing: border-box;
}
a.anchor-link:link {
  text-decoration: none;
  padding: 0px 20px;
  visibility: hidden;
}
h1:hover .anchor-link,
h2:hover .anchor-link,
h3:hover .anchor-link,
h4:hover .anchor-link,
h5:hover .anchor-link,
h6:hover .anchor-link {
  visibility: visible;
}
.text_cell.rendered .input_area {
  display: none;
}
.text_cell.rendered .rendered_html {
  overflow-x: auto;
  overflow-y: hidden;
}
.text_cell.rendered .rendered_html tr,
.text_cell.rendered .rendered_html th,
.text_cell.rendered .rendered_html td {
  max-width: none;
}
.text_cell.unrendered .text_cell_render {
  display: none;
}
.text_cell .dropzone .input_area {
  border: 2px dashed #bababa;
  margin: -1px;
}
.cm-header-1,
.cm-header-2,
.cm-header-3,
.cm-header-4,
.cm-header-5,
.cm-header-6 {
  font-weight: bold;
  font-family: "Helvetica Neue", Helvetica, Arial, sans-serif;
}
.cm-header-1 {
  font-size: 185.7%;
}
.cm-header-2 {
  font-size: 157.1%;
}
.cm-header-3 {
  font-size: 128.6%;
}
.cm-header-4 {
  font-size: 110%;
}
.cm-header-5 {
  font-size: 100%;
  font-style: italic;
}
.cm-header-6 {
  font-size: 100%;
  font-style: italic;
}
/*!
*
* IPython notebook webapp
*
*/
@media (max-width: 767px) {
  .notebook_app {
    padding-left: 0px;
    padding-right: 0px;
  }
}
#ipython-main-app {
  box-sizing: border-box;
  -moz-box-sizing: border-box;
  -webkit-box-sizing: border-box;
  height: 100%;
}
div#notebook_panel {
  margin: 0px;
  padding: 0px;
  box-sizing: border-box;
  -moz-box-sizing: border-box;
  -webkit-box-sizing: border-box;
  height: 100%;
}
div#notebook {
  font-size: 14px;
  line-height: 20px;
  overflow-y: hidden;
  overflow-x: auto;
  width: 100%;
  /* This spaces the page away from the edge of the notebook area */
  padding-top: 20px;
  margin: 0px;
  outline: none;
  box-sizing: border-box;
  -moz-box-sizing: border-box;
  -webkit-box-sizing: border-box;
  min-height: 100%;
}
@media not print {
  #notebook-container {
    padding: 15px;
    background-color: #fff;
    min-height: 0;
    -webkit-box-shadow: 0px 0px 12px 1px rgba(87, 87, 87, 0.2);
    box-shadow: 0px 0px 12px 1px rgba(87, 87, 87, 0.2);
  }
}
@media print {
  #notebook-container {
    width: 100%;
  }
}
div.ui-widget-content {
  border: 1px solid #ababab;
  outline: none;
}
pre.dialog {
  background-color: #f7f7f7;
  border: 1px solid #ddd;
  border-radius: 2px;
  padding: 0.4em;
  padding-left: 2em;
}
p.dialog {
  padding: 0.2em;
}
/* Word-wrap output correctly.  This is the CSS3 spelling, though Firefox seems
   to not honor it correctly.  Webkit browsers (Chrome, rekonq, Safari) do.
 */
pre,
code,
kbd,
samp {
  white-space: pre-wrap;
}
#fonttest {
  font-family: monospace;
}
p {
  margin-bottom: 0;
}
.end_space {
  min-height: 100px;
  transition: height .2s ease;
}
.notebook_app > #header {
  -webkit-box-shadow: 0px 0px 12px 1px rgba(87, 87, 87, 0.2);
  box-shadow: 0px 0px 12px 1px rgba(87, 87, 87, 0.2);
}
@media not print {
  .notebook_app {
    background-color: #EEE;
  }
}
kbd {
  border-style: solid;
  border-width: 1px;
  box-shadow: none;
  margin: 2px;
  padding-left: 2px;
  padding-right: 2px;
  padding-top: 1px;
  padding-bottom: 1px;
}
.jupyter-keybindings {
  padding: 1px;
  line-height: 24px;
  border-bottom: 1px solid gray;
}
.jupyter-keybindings input {
  margin: 0;
  padding: 0;
  border: none;
}
.jupyter-keybindings i {
  padding: 6px;
}
.well code {
  background-color: #ffffff;
  border-color: #ababab;
  border-width: 1px;
  border-style: solid;
  padding: 2px;
  padding-top: 1px;
  padding-bottom: 1px;
}
/* CSS for the cell toolbar */
.celltoolbar {
  border: thin solid #CFCFCF;
  border-bottom: none;
  background: #EEE;
  border-radius: 2px 2px 0px 0px;
  width: 100%;
  height: 29px;
  padding-right: 4px;
  /* Old browsers */
  display: -webkit-box;
  -webkit-box-orient: horizontal;
  -webkit-box-align: stretch;
  display: -moz-box;
  -moz-box-orient: horizontal;
  -moz-box-align: stretch;
  display: box;
  box-orient: horizontal;
  box-align: stretch;
  /* Modern browsers */
  display: flex;
  flex-direction: row;
  align-items: stretch;
  /* Old browsers */
  -webkit-box-pack: end;
  -moz-box-pack: end;
  box-pack: end;
  /* Modern browsers */
  justify-content: flex-end;
  display: -webkit-flex;
}
@media print {
  .celltoolbar {
    display: none;
  }
}
.ctb_hideshow {
  display: none;
  vertical-align: bottom;
}
/* ctb_show is added to the ctb_hideshow div to show the cell toolbar.
   Cell toolbars are only shown when the ctb_global_show class is also set.
*/
.ctb_global_show .ctb_show.ctb_hideshow {
  display: block;
}
.ctb_global_show .ctb_show + .input_area,
.ctb_global_show .ctb_show + div.text_cell_input,
.ctb_global_show .ctb_show ~ div.text_cell_render {
  border-top-right-radius: 0px;
  border-top-left-radius: 0px;
}
.ctb_global_show .ctb_show ~ div.text_cell_render {
  border: 1px solid #cfcfcf;
}
.celltoolbar {
  font-size: 87%;
  padding-top: 3px;
}
.celltoolbar select {
  display: block;
  width: 100%;
  height: 32px;
  padding: 6px 12px;
  font-size: 13px;
  line-height: 1.42857143;
  color: #555555;
  background-color: #fff;
  background-image: none;
  border: 1px solid #ccc;
  border-radius: 2px;
  -webkit-box-shadow: inset 0 1px 1px rgba(0, 0, 0, 0.075);
  box-shadow: inset 0 1px 1px rgba(0, 0, 0, 0.075);
  -webkit-transition: border-color ease-in-out .15s, box-shadow ease-in-out .15s;
  -o-transition: border-color ease-in-out .15s, box-shadow ease-in-out .15s;
  transition: border-color ease-in-out .15s, box-shadow ease-in-out .15s;
  height: 30px;
  padding: 5px 10px;
  font-size: 12px;
  line-height: 1.5;
  border-radius: 1px;
  width: inherit;
  font-size: inherit;
  height: 22px;
  padding: 0px;
  display: inline-block;
}
.celltoolbar select:focus {
  border-color: #66afe9;
  outline: 0;
  -webkit-box-shadow: inset 0 1px 1px rgba(0,0,0,.075), 0 0 8px rgba(102, 175, 233, 0.6);
  box-shadow: inset 0 1px 1px rgba(0,0,0,.075), 0 0 8px rgba(102, 175, 233, 0.6);
}
.celltoolbar select::-moz-placeholder {
  color: #999;
  opacity: 1;
}
.celltoolbar select:-ms-input-placeholder {
  color: #999;
}
.celltoolbar select::-webkit-input-placeholder {
  color: #999;
}
.celltoolbar select::-ms-expand {
  border: 0;
  background-color: transparent;
}
.celltoolbar select[disabled],
.celltoolbar select[readonly],
fieldset[disabled] .celltoolbar select {
  background-color: #eeeeee;
  opacity: 1;
}
.celltoolbar select[disabled],
fieldset[disabled] .celltoolbar select {
  cursor: not-allowed;
}
textarea.celltoolbar select {
  height: auto;
}
select.celltoolbar select {
  height: 30px;
  line-height: 30px;
}
textarea.celltoolbar select,
select[multiple].celltoolbar select {
  height: auto;
}
.celltoolbar label {
  margin-left: 5px;
  margin-right: 5px;
}
.tags_button_container {
  width: 100%;
  display: flex;
}
.tag-container {
  display: flex;
  flex-direction: row;
  flex-grow: 1;
  overflow: hidden;
  position: relative;
}
.tag-container > * {
  margin: 0 4px;
}
.remove-tag-btn {
  margin-left: 4px;
}
.tags-input {
  display: flex;
}
.cell-tag:last-child:after {
  content: "";
  position: absolute;
  right: 0;
  width: 40px;
  height: 100%;
  /* Fade to background color of cell toolbar */
  background: linear-gradient(to right, rgba(0, 0, 0, 0), #EEE);
}
.tags-input > * {
  margin-left: 4px;
}
.cell-tag,
.tags-input input,
.tags-input button {
  display: block;
  width: 100%;
  height: 32px;
  padding: 6px 12px;
  font-size: 13px;
  line-height: 1.42857143;
  color: #555555;
  background-color: #fff;
  background-image: none;
  border: 1px solid #ccc;
  border-radius: 2px;
  -webkit-box-shadow: inset 0 1px 1px rgba(0, 0, 0, 0.075);
  box-shadow: inset 0 1px 1px rgba(0, 0, 0, 0.075);
  -webkit-transition: border-color ease-in-out .15s, box-shadow ease-in-out .15s;
  -o-transition: border-color ease-in-out .15s, box-shadow ease-in-out .15s;
  transition: border-color ease-in-out .15s, box-shadow ease-in-out .15s;
  height: 30px;
  padding: 5px 10px;
  font-size: 12px;
  line-height: 1.5;
  border-radius: 1px;
  box-shadow: none;
  width: inherit;
  font-size: inherit;
  height: 22px;
  line-height: 22px;
  padding: 0px 4px;
  display: inline-block;
}
.cell-tag:focus,
.tags-input input:focus,
.tags-input button:focus {
  border-color: #66afe9;
  outline: 0;
  -webkit-box-shadow: inset 0 1px 1px rgba(0,0,0,.075), 0 0 8px rgba(102, 175, 233, 0.6);
  box-shadow: inset 0 1px 1px rgba(0,0,0,.075), 0 0 8px rgba(102, 175, 233, 0.6);
}
.cell-tag::-moz-placeholder,
.tags-input input::-moz-placeholder,
.tags-input button::-moz-placeholder {
  color: #999;
  opacity: 1;
}
.cell-tag:-ms-input-placeholder,
.tags-input input:-ms-input-placeholder,
.tags-input button:-ms-input-placeholder {
  color: #999;
}
.cell-tag::-webkit-input-placeholder,
.tags-input input::-webkit-input-placeholder,
.tags-input button::-webkit-input-placeholder {
  color: #999;
}
.cell-tag::-ms-expand,
.tags-input input::-ms-expand,
.tags-input button::-ms-expand {
  border: 0;
  background-color: transparent;
}
.cell-tag[disabled],
.tags-input input[disabled],
.tags-input button[disabled],
.cell-tag[readonly],
.tags-input input[readonly],
.tags-input button[readonly],
fieldset[disabled] .cell-tag,
fieldset[disabled] .tags-input input,
fieldset[disabled] .tags-input button {
  background-color: #eeeeee;
  opacity: 1;
}
.cell-tag[disabled],
.tags-input input[disabled],
.tags-input button[disabled],
fieldset[disabled] .cell-tag,
fieldset[disabled] .tags-input input,
fieldset[disabled] .tags-input button {
  cursor: not-allowed;
}
textarea.cell-tag,
textarea.tags-input input,
textarea.tags-input button {
  height: auto;
}
select.cell-tag,
select.tags-input input,
select.tags-input button {
  height: 30px;
  line-height: 30px;
}
textarea.cell-tag,
textarea.tags-input input,
textarea.tags-input button,
select[multiple].cell-tag,
select[multiple].tags-input input,
select[multiple].tags-input button {
  height: auto;
}
.cell-tag,
.tags-input button {
  padding: 0px 4px;
}
.cell-tag {
  background-color: #fff;
  white-space: nowrap;
}
.tags-input input[type=text]:focus {
  outline: none;
  box-shadow: none;
  border-color: #ccc;
}
.completions {
  position: absolute;
  z-index: 110;
  overflow: hidden;
  border: 1px solid #ababab;
  border-radius: 2px;
  -webkit-box-shadow: 0px 6px 10px -1px #adadad;
  box-shadow: 0px 6px 10px -1px #adadad;
  line-height: 1;
}
.completions select {
  background: white;
  outline: none;
  border: none;
  padding: 0px;
  margin: 0px;
  overflow: auto;
  font-family: monospace;
  font-size: 110%;
  color: #000;
  width: auto;
}
.completions select option.context {
  color: #286090;
}
#kernel_logo_widget .current_kernel_logo {
  display: none;
  margin-top: -1px;
  margin-bottom: -1px;
  width: 32px;
  height: 32px;
}
[dir="rtl"] #kernel_logo_widget {
  float: left !important;
  float: left;
}
.modal .modal-body .move-path {
  display: flex;
  flex-direction: row;
  justify-content: space;
  align-items: center;
}
.modal .modal-body .move-path .server-root {
  padding-right: 20px;
}
.modal .modal-body .move-path .path-input {
  flex: 1;
}
#menubar {
  box-sizing: border-box;
  -moz-box-sizing: border-box;
  -webkit-box-sizing: border-box;
  margin-top: 1px;
}
#menubar .navbar {
  border-top: 1px;
  border-radius: 0px 0px 2px 2px;
  margin-bottom: 0px;
}
#menubar .navbar-toggle {
  float: left;
  padding-top: 7px;
  padding-bottom: 7px;
  border: none;
}
#menubar .navbar-collapse {
  clear: left;
}
[dir="rtl"] #menubar .navbar-toggle {
  float: right;
}
[dir="rtl"] #menubar .navbar-collapse {
  clear: right;
}
[dir="rtl"] #menubar .navbar-nav {
  float: right;
}
[dir="rtl"] #menubar .nav {
  padding-right: 0px;
}
[dir="rtl"] #menubar .navbar-nav > li {
  float: right;
}
[dir="rtl"] #menubar .navbar-right {
  float: left !important;
}
[dir="rtl"] ul.dropdown-menu {
  text-align: right;
  left: auto;
}
[dir="rtl"] ul#new-menu.dropdown-menu {
  right: auto;
  left: 0;
}
.nav-wrapper {
  border-bottom: 1px solid #e7e7e7;
}
i.menu-icon {
  padding-top: 4px;
}
[dir="rtl"] i.menu-icon.pull-right {
  float: left !important;
  float: left;
}
ul#help_menu li a {
  overflow: hidden;
  padding-right: 2.2em;
}
ul#help_menu li a i {
  margin-right: -1.2em;
}
[dir="rtl"] ul#help_menu li a {
  padding-left: 2.2em;
}
[dir="rtl"] ul#help_menu li a i {
  margin-right: 0;
  margin-left: -1.2em;
}
[dir="rtl"] ul#help_menu li a i.pull-right {
  float: left !important;
  float: left;
}
.dropdown-submenu {
  position: relative;
}
.dropdown-submenu > .dropdown-menu {
  top: 0;
  left: 100%;
  margin-top: -6px;
  margin-left: -1px;
}
[dir="rtl"] .dropdown-submenu > .dropdown-menu {
  right: 100%;
  margin-right: -1px;
}
.dropdown-submenu:hover > .dropdown-menu {
  display: block;
}
.dropdown-submenu > a:after {
  display: inline-block;
  font: normal normal normal 14px/1 FontAwesome;
  font-size: inherit;
  text-rendering: auto;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  display: block;
  content: "\f0da";
  float: right;
  color: #333333;
  margin-top: 2px;
  margin-right: -10px;
}
.dropdown-submenu > a:after.fa-pull-left {
  margin-right: .3em;
}
.dropdown-submenu > a:after.fa-pull-right {
  margin-left: .3em;
}
.dropdown-submenu > a:after.pull-left {
  margin-right: .3em;
}
.dropdown-submenu > a:after.pull-right {
  margin-left: .3em;
}
[dir="rtl"] .dropdown-submenu > a:after {
  float: left;
  content: "\f0d9";
  margin-right: 0;
  margin-left: -10px;
}
.dropdown-submenu:hover > a:after {
  color: #262626;
}
.dropdown-submenu.pull-left {
  float: none;
}
.dropdown-submenu.pull-left > .dropdown-menu {
  left: -100%;
  margin-left: 10px;
}
#notification_area {
  float: right !important;
  float: right;
  z-index: 10;
}
[dir="rtl"] #notification_area {
  float: left !important;
  float: left;
}
.indicator_area {
  float: right !important;
  float: right;
  color: #777;
  margin-left: 5px;
  margin-right: 5px;
  width: 11px;
  z-index: 10;
  text-align: center;
  width: auto;
}
[dir="rtl"] .indicator_area {
  float: left !important;
  float: left;
}
#kernel_indicator {
  float: right !important;
  float: right;
  color: #777;
  margin-left: 5px;
  margin-right: 5px;
  width: 11px;
  z-index: 10;
  text-align: center;
  width: auto;
  border-left: 1px solid;
}
#kernel_indicator .kernel_indicator_name {
  padding-left: 5px;
  padding-right: 5px;
}
[dir="rtl"] #kernel_indicator {
  float: left !important;
  float: left;
  border-left: 0;
  border-right: 1px solid;
}
#modal_indicator {
  float: right !important;
  float: right;
  color: #777;
  margin-left: 5px;
  margin-right: 5px;
  width: 11px;
  z-index: 10;
  text-align: center;
  width: auto;
}
[dir="rtl"] #modal_indicator {
  float: left !important;
  float: left;
}
#readonly-indicator {
  float: right !important;
  float: right;
  color: #777;
  margin-left: 5px;
  margin-right: 5px;
  width: 11px;
  z-index: 10;
  text-align: center;
  width: auto;
  margin-top: 2px;
  margin-bottom: 0px;
  margin-left: 0px;
  margin-right: 0px;
  display: none;
}
.modal_indicator:before {
  width: 1.28571429em;
  text-align: center;
}
.edit_mode .modal_indicator:before {
  display: inline-block;
  font: normal normal normal 14px/1 FontAwesome;
  font-size: inherit;
  text-rendering: auto;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  content: "\f040";
}
.edit_mode .modal_indicator:before.fa-pull-left {
  margin-right: .3em;
}
.edit_mode .modal_indicator:before.fa-pull-right {
  margin-left: .3em;
}
.edit_mode .modal_indicator:before.pull-left {
  margin-right: .3em;
}
.edit_mode .modal_indicator:before.pull-right {
  margin-left: .3em;
}
.command_mode .modal_indicator:before {
  display: inline-block;
  font: normal normal normal 14px/1 FontAwesome;
  font-size: inherit;
  text-rendering: auto;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  content: ' ';
}
.command_mode .modal_indicator:before.fa-pull-left {
  margin-right: .3em;
}
.command_mode .modal_indicator:before.fa-pull-right {
  margin-left: .3em;
}
.command_mode .modal_indicator:before.pull-left {
  margin-right: .3em;
}
.command_mode .modal_indicator:before.pull-right {
  margin-left: .3em;
}
.kernel_idle_icon:before {
  display: inline-block;
  font: normal normal normal 14px/1 FontAwesome;
  font-size: inherit;
  text-rendering: auto;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  content: "\f10c";
}
.kernel_idle_icon:before.fa-pull-left {
  margin-right: .3em;
}
.kernel_idle_icon:before.fa-pull-right {
  margin-left: .3em;
}
.kernel_idle_icon:before.pull-left {
  margin-right: .3em;
}
.kernel_idle_icon:before.pull-right {
  margin-left: .3em;
}
.kernel_busy_icon:before {
  display: inline-block;
  font: normal normal normal 14px/1 FontAwesome;
  font-size: inherit;
  text-rendering: auto;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  content: "\f111";
}
.kernel_busy_icon:before.fa-pull-left {
  margin-right: .3em;
}
.kernel_busy_icon:before.fa-pull-right {
  margin-left: .3em;
}
.kernel_busy_icon:before.pull-left {
  margin-right: .3em;
}
.kernel_busy_icon:before.pull-right {
  margin-left: .3em;
}
.kernel_dead_icon:before {
  display: inline-block;
  font: normal normal normal 14px/1 FontAwesome;
  font-size: inherit;
  text-rendering: auto;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  content: "\f1e2";
}
.kernel_dead_icon:before.fa-pull-left {
  margin-right: .3em;
}
.kernel_dead_icon:before.fa-pull-right {
  margin-left: .3em;
}
.kernel_dead_icon:before.pull-left {
  margin-right: .3em;
}
.kernel_dead_icon:before.pull-right {
  margin-left: .3em;
}
.kernel_disconnected_icon:before {
  display: inline-block;
  font: normal normal normal 14px/1 FontAwesome;
  font-size: inherit;
  text-rendering: auto;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  content: "\f127";
}
.kernel_disconnected_icon:before.fa-pull-left {
  margin-right: .3em;
}
.kernel_disconnected_icon:before.fa-pull-right {
  margin-left: .3em;
}
.kernel_disconnected_icon:before.pull-left {
  margin-right: .3em;
}
.kernel_disconnected_icon:before.pull-right {
  margin-left: .3em;
}
.notification_widget {
  color: #777;
  z-index: 10;
  background: rgba(240, 240, 240, 0.5);
  margin-right: 4px;
  color: #333;
  background-color: #fff;
  border-color: #ccc;
}
.notification_widget:focus,
.notification_widget.focus {
  color: #333;
  background-color: #e6e6e6;
  border-color: #8c8c8c;
}
.notification_widget:hover {
  color: #333;
  background-color: #e6e6e6;
  border-color: #adadad;
}
.notification_widget:active,
.notification_widget.active,
.open > .dropdown-toggle.notification_widget {
  color: #333;
  background-color: #e6e6e6;
  border-color: #adadad;
}
.notification_widget:active:hover,
.notification_widget.active:hover,
.open > .dropdown-toggle.notification_widget:hover,
.notification_widget:active:focus,
.notification_widget.active:focus,
.open > .dropdown-toggle.notification_widget:focus,
.notification_widget:active.focus,
.notification_widget.active.focus,
.open > .dropdown-toggle.notification_widget.focus {
  color: #333;
  background-color: #d4d4d4;
  border-color: #8c8c8c;
}
.notification_widget:active,
.notification_widget.active,
.open > .dropdown-toggle.notification_widget {
  background-image: none;
}
.notification_widget.disabled:hover,
.notification_widget[disabled]:hover,
fieldset[disabled] .notification_widget:hover,
.notification_widget.disabled:focus,
.notification_widget[disabled]:focus,
fieldset[disabled] .notification_widget:focus,
.notification_widget.disabled.focus,
.notification_widget[disabled].focus,
fieldset[disabled] .notification_widget.focus {
  background-color: #fff;
  border-color: #ccc;
}
.notification_widget .badge {
  color: #fff;
  background-color: #333;
}
.notification_widget.warning {
  color: #fff;
  background-color: #f0ad4e;
  border-color: #eea236;
}
.notification_widget.warning:focus,
.notification_widget.warning.focus {
  color: #fff;
  background-color: #ec971f;
  border-color: #985f0d;
}
.notification_widget.warning:hover {
  color: #fff;
  background-color: #ec971f;
  border-color: #d58512;
}
.notification_widget.warning:active,
.notification_widget.warning.active,
.open > .dropdown-toggle.notification_widget.warning {
  color: #fff;
  background-color: #ec971f;
  border-color: #d58512;
}
.notification_widget.warning:active:hover,
.notification_widget.warning.active:hover,
.open > .dropdown-toggle.notification_widget.warning:hover,
.notification_widget.warning:active:focus,
.notification_widget.warning.active:focus,
.open > .dropdown-toggle.notification_widget.warning:focus,
.notification_widget.warning:active.focus,
.notification_widget.warning.active.focus,
.open > .dropdown-toggle.notification_widget.warning.focus {
  color: #fff;
  background-color: #d58512;
  border-color: #985f0d;
}
.notification_widget.warning:active,
.notification_widget.warning.active,
.open > .dropdown-toggle.notification_widget.warning {
  background-image: none;
}
.notification_widget.warning.disabled:hover,
.notification_widget.warning[disabled]:hover,
fieldset[disabled] .notification_widget.warning:hover,
.notification_widget.warning.disabled:focus,
.notification_widget.warning[disabled]:focus,
fieldset[disabled] .notification_widget.warning:focus,
.notification_widget.warning.disabled.focus,
.notification_widget.warning[disabled].focus,
fieldset[disabled] .notification_widget.warning.focus {
  background-color: #f0ad4e;
  border-color: #eea236;
}
.notification_widget.warning .badge {
  color: #f0ad4e;
  background-color: #fff;
}
.notification_widget.success {
  color: #fff;
  background-color: #5cb85c;
  border-color: #4cae4c;
}
.notification_widget.success:focus,
.notification_widget.success.focus {
  color: #fff;
  background-color: #449d44;
  border-color: #255625;
}
.notification_widget.success:hover {
  color: #fff;
  background-color: #449d44;
  border-color: #398439;
}
.notification_widget.success:active,
.notification_widget.success.active,
.open > .dropdown-toggle.notification_widget.success {
  color: #fff;
  background-color: #449d44;
  border-color: #398439;
}
.notification_widget.success:active:hover,
.notification_widget.success.active:hover,
.open > .dropdown-toggle.notification_widget.success:hover,
.notification_widget.success:active:focus,
.notification_widget.success.active:focus,
.open > .dropdown-toggle.notification_widget.success:focus,
.notification_widget.success:active.focus,
.notification_widget.success.active.focus,
.open > .dropdown-toggle.notification_widget.success.focus {
  color: #fff;
  background-color: #398439;
  border-color: #255625;
}
.notification_widget.success:active,
.notification_widget.success.active,
.open > .dropdown-toggle.notification_widget.success {
  background-image: none;
}
.notification_widget.success.disabled:hover,
.notification_widget.success[disabled]:hover,
fieldset[disabled] .notification_widget.success:hover,
.notification_widget.success.disabled:focus,
.notification_widget.success[disabled]:focus,
fieldset[disabled] .notification_widget.success:focus,
.notification_widget.success.disabled.focus,
.notification_widget.success[disabled].focus,
fieldset[disabled] .notification_widget.success.focus {
  background-color: #5cb85c;
  border-color: #4cae4c;
}
.notification_widget.success .badge {
  color: #5cb85c;
  background-color: #fff;
}
.notification_widget.info {
  color: #fff;
  background-color: #5bc0de;
  border-color: #46b8da;
}
.notification_widget.info:focus,
.notification_widget.info.focus {
  color: #fff;
  background-color: #31b0d5;
  border-color: #1b6d85;
}
.notification_widget.info:hover {
  color: #fff;
  background-color: #31b0d5;
  border-color: #269abc;
}
.notification_widget.info:active,
.notification_widget.info.active,
.open > .dropdown-toggle.notification_widget.info {
  color: #fff;
  background-color: #31b0d5;
  border-color: #269abc;
}
.notification_widget.info:active:hover,
.notification_widget.info.active:hover,
.open > .dropdown-toggle.notification_widget.info:hover,
.notification_widget.info:active:focus,
.notification_widget.info.active:focus,
.open > .dropdown-toggle.notification_widget.info:focus,
.notification_widget.info:active.focus,
.notification_widget.info.active.focus,
.open > .dropdown-toggle.notification_widget.info.focus {
  color: #fff;
  background-color: #269abc;
  border-color: #1b6d85;
}
.notification_widget.info:active,
.notification_widget.info.active,
.open > .dropdown-toggle.notification_widget.info {
  background-image: none;
}
.notification_widget.info.disabled:hover,
.notification_widget.info[disabled]:hover,
fieldset[disabled] .notification_widget.info:hover,
.notification_widget.info.disabled:focus,
.notification_widget.info[disabled]:focus,
fieldset[disabled] .notification_widget.info:focus,
.notification_widget.info.disabled.focus,
.notification_widget.info[disabled].focus,
fieldset[disabled] .notification_widget.info.focus {
  background-color: #5bc0de;
  border-color: #46b8da;
}
.notification_widget.info .badge {
  color: #5bc0de;
  background-color: #fff;
}
.notification_widget.danger {
  color: #fff;
  background-color: #d9534f;
  border-color: #d43f3a;
}
.notification_widget.danger:focus,
.notification_widget.danger.focus {
  color: #fff;
  background-color: #c9302c;
  border-color: #761c19;
}
.notification_widget.danger:hover {
  color: #fff;
  background-color: #c9302c;
  border-color: #ac2925;
}
.notification_widget.danger:active,
.notification_widget.danger.active,
.open > .dropdown-toggle.notification_widget.danger {
  color: #fff;
  background-color: #c9302c;
  border-color: #ac2925;
}
.notification_widget.danger:active:hover,
.notification_widget.danger.active:hover,
.open > .dropdown-toggle.notification_widget.danger:hover,
.notification_widget.danger:active:focus,
.notification_widget.danger.active:focus,
.open > .dropdown-toggle.notification_widget.danger:focus,
.notification_widget.danger:active.focus,
.notification_widget.danger.active.focus,
.open > .dropdown-toggle.notification_widget.danger.focus {
  color: #fff;
  background-color: #ac2925;
  border-color: #761c19;
}
.notification_widget.danger:active,
.notification_widget.danger.active,
.open > .dropdown-toggle.notification_widget.danger {
  background-image: none;
}
.notification_widget.danger.disabled:hover,
.notification_widget.danger[disabled]:hover,
fieldset[disabled] .notification_widget.danger:hover,
.notification_widget.danger.disabled:focus,
.notification_widget.danger[disabled]:focus,
fieldset[disabled] .notification_widget.danger:focus,
.notification_widget.danger.disabled.focus,
.notification_widget.danger[disabled].focus,
fieldset[disabled] .notification_widget.danger.focus {
  background-color: #d9534f;
  border-color: #d43f3a;
}
.notification_widget.danger .badge {
  color: #d9534f;
  background-color: #fff;
}
div#pager {
  background-color: #fff;
  font-size: 14px;
  line-height: 20px;
  overflow: hidden;
  display: none;
  position: fixed;
  bottom: 0px;
  width: 100%;
  max-height: 50%;
  padding-top: 8px;
  -webkit-box-shadow: 0px 0px 12px 1px rgba(87, 87, 87, 0.2);
  box-shadow: 0px 0px 12px 1px rgba(87, 87, 87, 0.2);
  /* Display over codemirror */
  z-index: 100;
  /* Hack which prevents jquery ui resizable from changing top. */
  top: auto !important;
}
div#pager pre {
  line-height: 1.21429em;
  color: #000;
  background-color: #f7f7f7;
  padding: 0.4em;
}
div#pager #pager-button-area {
  position: absolute;
  top: 8px;
  right: 20px;
}
div#pager #pager-contents {
  position: relative;
  overflow: auto;
  width: 100%;
  height: 100%;
}
div#pager #pager-contents #pager-container {
  position: relative;
  padding: 15px 0px;
  box-sizing: border-box;
  -moz-box-sizing: border-box;
  -webkit-box-sizing: border-box;
}
div#pager .ui-resizable-handle {
  top: 0px;
  height: 8px;
  background: #f7f7f7;
  border-top: 1px solid #cfcfcf;
  border-bottom: 1px solid #cfcfcf;
  /* This injects handle bars (a short, wide = symbol) for 
        the resize handle. */
}
div#pager .ui-resizable-handle::after {
  content: '';
  top: 2px;
  left: 50%;
  height: 3px;
  width: 30px;
  margin-left: -15px;
  position: absolute;
  border-top: 1px solid #cfcfcf;
}
.quickhelp {
  /* Old browsers */
  display: -webkit-box;
  -webkit-box-orient: horizontal;
  -webkit-box-align: stretch;
  display: -moz-box;
  -moz-box-orient: horizontal;
  -moz-box-align: stretch;
  display: box;
  box-orient: horizontal;
  box-align: stretch;
  /* Modern browsers */
  display: flex;
  flex-direction: row;
  align-items: stretch;
  line-height: 1.8em;
}
.shortcut_key {
  display: inline-block;
  width: 21ex;
  text-align: right;
  font-family: monospace;
}
.shortcut_descr {
  display: inline-block;
  /* Old browsers */
  -webkit-box-flex: 1;
  -moz-box-flex: 1;
  box-flex: 1;
  /* Modern browsers */
  flex: 1;
}
span.save_widget {
  height: 30px;
  margin-top: 4px;
  display: flex;
  justify-content: flex-start;
  align-items: baseline;
  width: 50%;
  flex: 1;
}
span.save_widget span.filename {
  height: 100%;
  line-height: 1em;
  margin-left: 16px;
  border: none;
  font-size: 146.5%;
  text-overflow: ellipsis;
  overflow: hidden;
  white-space: nowrap;
  border-radius: 2px;
}
span.save_widget span.filename:hover {
  background-color: #e6e6e6;
}
[dir="rtl"] span.save_widget.pull-left {
  float: right !important;
  float: right;
}
[dir="rtl"] span.save_widget span.filename {
  margin-left: 0;
  margin-right: 16px;
}
span.checkpoint_status,
span.autosave_status {
  font-size: small;
  white-space: nowrap;
  padding: 0 5px;
}
@media (max-width: 767px) {
  span.save_widget {
    font-size: small;
    padding: 0 0 0 5px;
  }
  span.checkpoint_status,
  span.autosave_status {
    display: none;
  }
}
@media (min-width: 768px) and (max-width: 991px) {
  span.checkpoint_status {
    display: none;
  }
  span.autosave_status {
    font-size: x-small;
  }
}
.toolbar {
  padding: 0px;
  margin-left: -5px;
  margin-top: 2px;
  margin-bottom: 5px;
  box-sizing: border-box;
  -moz-box-sizing: border-box;
  -webkit-box-sizing: border-box;
}
.toolbar select,
.toolbar label {
  width: auto;
  vertical-align: middle;
  margin-right: 2px;
  margin-bottom: 0px;
  display: inline;
  font-size: 92%;
  margin-left: 0.3em;
  margin-right: 0.3em;
  padding: 0px;
  padding-top: 3px;
}
.toolbar .btn {
  padding: 2px 8px;
}
.toolbar .btn-group {
  margin-top: 0px;
  margin-left: 5px;
}
.toolbar-btn-label {
  margin-left: 6px;
}
#maintoolbar {
  margin-bottom: -3px;
  margin-top: -8px;
  border: 0px;
  min-height: 27px;
  margin-left: 0px;
  padding-top: 11px;
  padding-bottom: 3px;
}
#maintoolbar .navbar-text {
  float: none;
  vertical-align: middle;
  text-align: right;
  margin-left: 5px;
  margin-right: 0px;
  margin-top: 0px;
}
.select-xs {
  height: 24px;
}
[dir="rtl"] .btn-group > .btn,
.btn-group-vertical > .btn {
  float: right;
}
.pulse,
.dropdown-menu > li > a.pulse,
li.pulse > a.dropdown-toggle,
li.pulse.open > a.dropdown-toggle {
  background-color: #F37626;
  color: white;
}
/**
 * Primary styles
 *
 * Author: Jupyter Development Team
 */
/** WARNING IF YOU ARE EDITTING THIS FILE, if this is a .css file, It has a lot
 * of chance of beeing generated from the ../less/[samename].less file, you can
 * try to get back the less file by reverting somme commit in history
 **/
/*
 * We'll try to get something pretty, so we
 * have some strange css to have the scroll bar on
 * the left with fix button on the top right of the tooltip
 */
@-moz-keyframes fadeOut {
  from {
    opacity: 1;
  }
  to {
    opacity: 0;
  }
}
@-webkit-keyframes fadeOut {
  from {
    opacity: 1;
  }
  to {
    opacity: 0;
  }
}
@-moz-keyframes fadeIn {
  from {
    opacity: 0;
  }
  to {
    opacity: 1;
  }
}
@-webkit-keyframes fadeIn {
  from {
    opacity: 0;
  }
  to {
    opacity: 1;
  }
}
/*properties of tooltip after "expand"*/
.bigtooltip {
  overflow: auto;
  height: 200px;
  -webkit-transition-property: height;
  -webkit-transition-duration: 500ms;
  -moz-transition-property: height;
  -moz-transition-duration: 500ms;
  transition-property: height;
  transition-duration: 500ms;
}
/*properties of tooltip before "expand"*/
.smalltooltip {
  -webkit-transition-property: height;
  -webkit-transition-duration: 500ms;
  -moz-transition-property: height;
  -moz-transition-duration: 500ms;
  transition-property: height;
  transition-duration: 500ms;
  text-overflow: ellipsis;
  overflow: hidden;
  height: 80px;
}
.tooltipbuttons {
  position: absolute;
  padding-right: 15px;
  top: 0px;
  right: 0px;
}
.tooltiptext {
  /*avoid the button to overlap on some docstring*/
  padding-right: 30px;
}
.ipython_tooltip {
  max-width: 700px;
  /*fade-in animation when inserted*/
  -webkit-animation: fadeOut 400ms;
  -moz-animation: fadeOut 400ms;
  animation: fadeOut 400ms;
  -webkit-animation: fadeIn 400ms;
  -moz-animation: fadeIn 400ms;
  animation: fadeIn 400ms;
  vertical-align: middle;
  background-color: #f7f7f7;
  overflow: visible;
  border: #ababab 1px solid;
  outline: none;
  padding: 3px;
  margin: 0px;
  padding-left: 7px;
  font-family: monospace;
  min-height: 50px;
  -moz-box-shadow: 0px 6px 10px -1px #adadad;
  -webkit-box-shadow: 0px 6px 10px -1px #adadad;
  box-shadow: 0px 6px 10px -1px #adadad;
  border-radius: 2px;
  position: absolute;
  z-index: 1000;
}
.ipython_tooltip a {
  float: right;
}
.ipython_tooltip .tooltiptext pre {
  border: 0;
  border-radius: 0;
  font-size: 100%;
  background-color: #f7f7f7;
}
.pretooltiparrow {
  left: 0px;
  margin: 0px;
  top: -16px;
  width: 40px;
  height: 16px;
  overflow: hidden;
  position: absolute;
}
.pretooltiparrow:before {
  background-color: #f7f7f7;
  border: 1px #ababab solid;
  z-index: 11;
  content: "";
  position: absolute;
  left: 15px;
  top: 10px;
  width: 25px;
  height: 25px;
  -webkit-transform: rotate(45deg);
  -moz-transform: rotate(45deg);
  -ms-transform: rotate(45deg);
  -o-transform: rotate(45deg);
}
ul.typeahead-list i {
  margin-left: -10px;
  width: 18px;
}
[dir="rtl"] ul.typeahead-list i {
  margin-left: 0;
  margin-right: -10px;
}
ul.typeahead-list {
  max-height: 80vh;
  overflow: auto;
}
ul.typeahead-list > li > a {
  /** Firefox bug **/
  /* see https://github.com/jupyter/notebook/issues/559 */
  white-space: normal;
}
ul.typeahead-list  > li > a.pull-right {
  float: left !important;
  float: left;
}
[dir="rtl"] .typeahead-list {
  text-align: right;
}
.cmd-palette .modal-body {
  padding: 7px;
}
.cmd-palette form {
  background: white;
}
.cmd-palette input {
  outline: none;
}
.no-shortcut {
  min-width: 20px;
  color: transparent;
}
[dir="rtl"] .no-shortcut.pull-right {
  float: left !important;
  float: left;
}
[dir="rtl"] .command-shortcut.pull-right {
  float: left !important;
  float: left;
}
.command-shortcut:before {
  content: "(command mode)";
  padding-right: 3px;
  color: #777777;
}
.edit-shortcut:before {
  content: "(edit)";
  padding-right: 3px;
  color: #777777;
}
[dir="rtl"] .edit-shortcut.pull-right {
  float: left !important;
  float: left;
}
#find-and-replace #replace-preview .match,
#find-and-replace #replace-preview .insert {
  background-color: #BBDEFB;
  border-color: #90CAF9;
  border-style: solid;
  border-width: 1px;
  border-radius: 0px;
}
[dir="ltr"] #find-and-replace .input-group-btn + .form-control {
  border-left: none;
}
[dir="rtl"] #find-and-replace .input-group-btn + .form-control {
  border-right: none;
}
#find-and-replace #replace-preview .replace .match {
  background-color: #FFCDD2;
  border-color: #EF9A9A;
  border-radius: 0px;
}
#find-and-replace #replace-preview .replace .insert {
  background-color: #C8E6C9;
  border-color: #A5D6A7;
  border-radius: 0px;
}
#find-and-replace #replace-preview {
  max-height: 60vh;
  overflow: auto;
}
#find-and-replace #replace-preview pre {
  padding: 5px 10px;
}
.terminal-app {
  background: #EEE;
}
.terminal-app #header {
  background: #fff;
  -webkit-box-shadow: 0px 0px 12px 1px rgba(87, 87, 87, 0.2);
  box-shadow: 0px 0px 12px 1px rgba(87, 87, 87, 0.2);
}
.terminal-app .terminal {
  width: 100%;
  float: left;
  font-family: monospace;
  color: white;
  background: black;
  padding: 0.4em;
  border-radius: 2px;
  -webkit-box-shadow: 0px 0px 12px 1px rgba(87, 87, 87, 0.4);
  box-shadow: 0px 0px 12px 1px rgba(87, 87, 87, 0.4);
}
.terminal-app .terminal,
.terminal-app .terminal dummy-screen {
  line-height: 1em;
  font-size: 14px;
}
.terminal-app .terminal .xterm-rows {
  padding: 10px;
}
.terminal-app .terminal-cursor {
  color: black;
  background: white;
}
.terminal-app #terminado-container {
  margin-top: 20px;
}
/*# sourceMappingURL=style.min.css.map */
    </style>
<style type="text/css">
    .highlight .hll { background-color: #ffffcc }
.highlight  { background: #f8f8f8; }
.highlight .c { color: #408080; font-style: italic } /* Comment */
.highlight .err { border: 1px solid #FF0000 } /* Error */
.highlight .k { color: #008000; font-weight: bold } /* Keyword */
.highlight .o { color: #666666 } /* Operator */
.highlight .ch { color: #408080; font-style: italic } /* Comment.Hashbang */
.highlight .cm { color: #408080; font-style: italic } /* Comment.Multiline */
.highlight .cp { color: #BC7A00 } /* Comment.Preproc */
.highlight .cpf { color: #408080; font-style: italic } /* Comment.PreprocFile */
.highlight .c1 { color: #408080; font-style: italic } /* Comment.Single */
.highlight .cs { color: #408080; font-style: italic } /* Comment.Special */
.highlight .gd { color: #A00000 } /* Generic.Deleted */
.highlight .ge { font-style: italic } /* Generic.Emph */
.highlight .gr { color: #FF0000 } /* Generic.Error */
.highlight .gh { color: #000080; font-weight: bold } /* Generic.Heading */
.highlight .gi { color: #00A000 } /* Generic.Inserted */
.highlight .go { color: #888888 } /* Generic.Output */
.highlight .gp { color: #000080; font-weight: bold } /* Generic.Prompt */
.highlight .gs { font-weight: bold } /* Generic.Strong */
.highlight .gu { color: #800080; font-weight: bold } /* Generic.Subheading */
.highlight .gt { color: #0044DD } /* Generic.Traceback */
.highlight .kc { color: #008000; font-weight: bold } /* Keyword.Constant */
.highlight .kd { color: #008000; font-weight: bold } /* Keyword.Declaration */
.highlight .kn { color: #008000; font-weight: bold } /* Keyword.Namespace */
.highlight .kp { color: #008000 } /* Keyword.Pseudo */
.highlight .kr { color: #008000; font-weight: bold } /* Keyword.Reserved */
.highlight .kt { color: #B00040 } /* Keyword.Type */
.highlight .m { color: #666666 } /* Literal.Number */
.highlight .s { color: #BA2121 } /* Literal.String */
.highlight .na { color: #7D9029 } /* Name.Attribute */
.highlight .nb { color: #008000 } /* Name.Builtin */
.highlight .nc { color: #0000FF; font-weight: bold } /* Name.Class */
.highlight .no { color: #880000 } /* Name.Constant */
.highlight .nd { color: #AA22FF } /* Name.Decorator */
.highlight .ni { color: #999999; font-weight: bold } /* Name.Entity */
.highlight .ne { color: #D2413A; font-weight: bold } /* Name.Exception */
.highlight .nf { color: #0000FF } /* Name.Function */
.highlight .nl { color: #A0A000 } /* Name.Label */
.highlight .nn { color: #0000FF; font-weight: bold } /* Name.Namespace */
.highlight .nt { color: #008000; font-weight: bold } /* Name.Tag */
.highlight .nv { color: #19177C } /* Name.Variable */
.highlight .ow { color: #AA22FF; font-weight: bold } /* Operator.Word */
.highlight .w { color: #bbbbbb } /* Text.Whitespace */
.highlight .mb { color: #666666 } /* Literal.Number.Bin */
.highlight .mf { color: #666666 } /* Literal.Number.Float */
.highlight .mh { color: #666666 } /* Literal.Number.Hex */
.highlight .mi { color: #666666 } /* Literal.Number.Integer */
.highlight .mo { color: #666666 } /* Literal.Number.Oct */
.highlight .sa { color: #BA2121 } /* Literal.String.Affix */
.highlight .sb { color: #BA2121 } /* Literal.String.Backtick */
.highlight .sc { color: #BA2121 } /* Literal.String.Char */
.highlight .dl { color: #BA2121 } /* Literal.String.Delimiter */
.highlight .sd { color: #BA2121; font-style: italic } /* Literal.String.Doc */
.highlight .s2 { color: #BA2121 } /* Literal.String.Double */
.highlight .se { color: #BB6622; font-weight: bold } /* Literal.String.Escape */
.highlight .sh { color: #BA2121 } /* Literal.String.Heredoc */
.highlight .si { color: #BB6688; font-weight: bold } /* Literal.String.Interpol */
.highlight .sx { color: #008000 } /* Literal.String.Other */
.highlight .sr { color: #BB6688 } /* Literal.String.Regex */
.highlight .s1 { color: #BA2121 } /* Literal.String.Single */
.highlight .ss { color: #19177C } /* Literal.String.Symbol */
.highlight .bp { color: #008000 } /* Name.Builtin.Pseudo */
.highlight .fm { color: #0000FF } /* Name.Function.Magic */
.highlight .vc { color: #19177C } /* Name.Variable.Class */
.highlight .vg { color: #19177C } /* Name.Variable.Global */
.highlight .vi { color: #19177C } /* Name.Variable.Instance */
.highlight .vm { color: #19177C } /* Name.Variable.Magic */
.highlight .il { color: #666666 } /* Literal.Number.Integer.Long */
    </style>


<style type="text/css">
/* Overrides of notebook CSS for static HTML export */
body {
  overflow: visible;
  padding: 8px;
}

div#notebook {
  overflow: visible;
  border-top: none;
}@media print {
  div.cell {
    display: block;
    page-break-inside: avoid;
  } 
  div.output_wrapper { 
    display: block;
    page-break-inside: avoid; 
  }
  div.output { 
    display: block;
    page-break-inside: avoid; 
  }
}
</style>

<!-- Custom stylesheet, it must be in the same directory as the html file -->
<link rel="stylesheet" href="custom.css">

<!-- Loading mathjax macro -->
<!-- Load mathjax -->
    <script src="https://cdnjs.cloudflare.com/ajax/libs/mathjax/2.7.5/latest.js?config=TeX-AMS_HTML"></script>
    <!-- MathJax configuration -->
    <script type="text/x-mathjax-config">
    MathJax.Hub.Config({
        tex2jax: {
            inlineMath: [ ['$','$'], ["\\(","\\)"] ],
            displayMath: [ ['$$','$$'], ["\\[","\\]"] ],
            processEscapes: true,
            processEnvironments: true
        },
        // Center justify equations in code and markdown cells. Elsewhere
        // we use CSS to left justify single line equations in code cells.
        displayAlign: 'center',
        "HTML-CSS": {
            styles: {'.MathJax_Display': {"margin": 0}},
            linebreaks: { automatic: true }
        }
    });
    </script>
    <!-- End of mathjax configuration --></head>
<body>
  <div tabindex="-1" id="notebook" class="border-box-sizing">
    <div class="container" id="notebook-container">

<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[1]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="c1"># %matplotlib nbagg -&gt; Uncomment for viewing in notebook</span>
<span class="kn">import</span> <span class="nn">numpy</span> <span class="k">as</span> <span class="nn">np</span>
<span class="kn">from</span> <span class="nn">scipy.spatial.distance</span> <span class="kn">import</span> <span class="n">pdist</span><span class="p">,</span> <span class="n">squareform</span>
<span class="kn">import</span> <span class="nn">random</span>
<span class="kn">from</span> <span class="nn">random</span> <span class="kn">import</span> <span class="n">gauss</span><span class="p">,</span> <span class="n">seed</span>
<span class="kn">import</span> <span class="nn">matplotlib.pyplot</span> <span class="k">as</span> <span class="nn">plt</span>
<span class="kn">import</span> <span class="nn">scipy.integrate</span> <span class="k">as</span> <span class="nn">integrate</span>
<span class="kn">import</span> <span class="nn">matplotlib.animation</span> <span class="k">as</span> <span class="nn">animation</span>
<span class="kn">import</span> <span class="nn">scipy.stats</span> <span class="k">as</span> <span class="nn">ss</span>
<span class="kn">import</span> <span class="nn">seaborn</span> <span class="k">as</span> <span class="nn">sns</span>
<span class="kn">import</span> <span class="nn">math</span>
<span class="kn">import</span> <span class="nn">pandas</span> <span class="k">as</span> <span class="nn">pd</span>
<span class="kn">import</span> <span class="nn">copy</span>
</pre></div>

    </div>
</div>
</div>

</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[2]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="c1"># Constants</span>
<span class="n">graphlen</span> <span class="o">=</span> <span class="mi">10</span>
<span class="n">boxlen</span> <span class="o">=</span> <span class="mi">7</span>
<span class="n">fps</span> <span class="o">=</span> <span class="mi">10</span>
<span class="n">m</span> <span class="o">=</span> <span class="p">[</span><span class="mi">300</span><span class="p">,</span><span class="mi">300</span><span class="p">,</span><span class="mi">300</span><span class="p">]</span>
<span class="n">f</span> <span class="o">=</span> <span class="mi">300</span>
<span class="n">mu</span> <span class="o">=</span> <span class="mi">1200</span>
<span class="n">sigma</span> <span class="o">=</span> <span class="mi">200</span>
<span class="n">frames</span> <span class="o">=</span> <span class="mi">800</span>
<span class="n">iterations</span> <span class="o">=</span> <span class="mi">10</span>
</pre></div>

    </div>
</div>
</div>

</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[3]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="k">def</span> <span class="nf">findAverage</span><span class="p">(</span><span class="n">runs</span><span class="p">):</span>
    <span class="n">avg</span> <span class="o">=</span> <span class="p">[]</span>
    <span class="k">for</span> <span class="n">i</span> <span class="ow">in</span> <span class="nb">range</span><span class="p">(</span><span class="mi">0</span><span class="p">,</span> <span class="nb">len</span><span class="p">(</span><span class="n">runs</span><span class="p">[</span><span class="mi">0</span><span class="p">])):</span>
        <span class="n">avg</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="mi">0</span><span class="p">)</span>
        <span class="k">for</span> <span class="n">j</span> <span class="ow">in</span> <span class="nb">range</span><span class="p">(</span><span class="mi">0</span><span class="p">,</span> <span class="nb">len</span><span class="p">(</span><span class="n">runs</span><span class="p">)):</span>
            <span class="n">avg</span><span class="p">[</span><span class="n">i</span><span class="p">]</span> <span class="o">=</span> <span class="n">avg</span><span class="p">[</span><span class="n">i</span><span class="p">]</span> <span class="o">+</span> <span class="n">runs</span><span class="p">[</span><span class="n">j</span><span class="p">][</span><span class="n">i</span><span class="p">]</span>
        <span class="n">avg</span><span class="p">[</span><span class="n">i</span><span class="p">]</span> <span class="o">=</span> <span class="n">avg</span><span class="p">[</span><span class="n">i</span><span class="p">]</span> <span class="o">/</span> <span class="nb">len</span><span class="p">(</span><span class="n">runs</span><span class="p">)</span> 
    <span class="k">return</span> <span class="n">avg</span>
</pre></div>

    </div>
</div>
</div>

</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[4]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">x</span> <span class="o">=</span> <span class="n">np</span><span class="o">.</span><span class="n">linspace</span><span class="p">(</span><span class="mi">400</span><span class="p">,</span> <span class="mi">2000</span><span class="p">,</span> <span class="mi">5000</span><span class="p">)</span>

<span class="n">pdf</span> <span class="o">=</span> <span class="n">ss</span><span class="o">.</span><span class="n">norm</span><span class="o">.</span><span class="n">pdf</span><span class="p">(</span><span class="n">x</span><span class="p">,</span> <span class="n">mu</span><span class="p">,</span> <span class="n">sigma</span><span class="p">)</span> 
<span class="n">cdf</span> <span class="o">=</span> <span class="n">ss</span><span class="o">.</span><span class="n">norm</span><span class="o">.</span><span class="n">cdf</span><span class="p">(</span><span class="n">x</span><span class="p">,</span> <span class="n">mu</span><span class="p">,</span> <span class="n">sigma</span><span class="p">)</span>

<span class="n">fig</span><span class="p">,</span> <span class="n">axes</span> <span class="o">=</span> <span class="n">plt</span><span class="o">.</span><span class="n">subplots</span><span class="p">(</span><span class="n">nrows</span><span class="o">=</span><span class="mi">1</span><span class="p">,</span> <span class="n">ncols</span><span class="o">=</span><span class="mi">2</span><span class="p">,</span> <span class="n">figsize</span><span class="o">=</span><span class="p">(</span><span class="mi">12</span><span class="p">,</span> <span class="mi">5</span><span class="p">))</span>
<span class="n">axes</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span><span class="o">.</span><span class="n">plot</span><span class="p">(</span><span class="n">x</span><span class="p">,</span> <span class="n">pdf</span><span class="p">)</span>
<span class="n">axes</span><span class="p">[</span><span class="mi">1</span><span class="p">]</span><span class="o">.</span><span class="n">plot</span><span class="p">(</span><span class="n">x</span><span class="p">,</span> <span class="n">cdf</span><span class="p">)</span>
<span class="n">axes</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span><span class="o">.</span><span class="n">title</span><span class="o">.</span><span class="n">set_text</span><span class="p">(</span><span class="s1">&#39;PDF&#39;</span><span class="p">)</span>
<span class="n">axes</span><span class="p">[</span><span class="mi">1</span><span class="p">]</span><span class="o">.</span><span class="n">title</span><span class="o">.</span><span class="n">set_text</span><span class="p">(</span><span class="s1">&#39;CDF&#39;</span><span class="p">)</span>
</pre></div>

    </div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area">

    <div class="prompt"></div>




<div class="output_png output_subarea ">
<img src="data:image/png;base64,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
"
>
</div>

</div>

</div>
</div>

</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[5]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="c1"># For making a permanent deep copy of user ratings across multiple simulations</span>
<span class="n">user_ratings</span> <span class="o">=</span> <span class="p">[]</span>
<span class="k">for</span> <span class="n">i</span> <span class="ow">in</span> <span class="nb">range</span><span class="p">(</span><span class="mi">0</span><span class="p">,</span> <span class="nb">sum</span><span class="p">(</span><span class="n">m</span><span class="p">)</span><span class="o">+</span><span class="n">f</span><span class="p">):</span>
    <span class="n">user_ratings</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">gauss</span><span class="p">(</span><span class="n">mu</span><span class="p">,</span> <span class="n">sigma</span><span class="p">))</span>

<span class="c1"># copy.deepcopy(user_ratings) can be used to create a temporary copy</span>
</pre></div>

    </div>
</div>
</div>

</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[6]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="k">class</span> <span class="nc">Particle</span><span class="p">:</span>
    <span class="k">def</span> <span class="fm">__init__</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">ID</span><span class="p">,</span> <span class="n">gender</span><span class="p">,</span> <span class="n">rating</span><span class="p">,</span> <span class="n">group</span> <span class="o">=</span> <span class="s1">&#39;normal&#39;</span><span class="p">):</span>
        <span class="bp">self</span><span class="o">.</span><span class="n">ID</span> <span class="o">=</span> <span class="n">ID</span>
        <span class="bp">self</span><span class="o">.</span><span class="n">gender</span> <span class="o">=</span> <span class="n">gender</span>
        <span class="bp">self</span><span class="o">.</span><span class="n">elo</span> <span class="o">=</span> <span class="n">mu</span>
        <span class="bp">self</span><span class="o">.</span><span class="n">rating</span> <span class="o">=</span> <span class="n">rating</span>
        <span class="bp">self</span><span class="o">.</span><span class="n">left</span> <span class="o">=</span> <span class="p">{}</span>
        <span class="bp">self</span><span class="o">.</span><span class="n">right</span> <span class="o">=</span> <span class="p">{}</span>
        <span class="bp">self</span><span class="o">.</span><span class="n">rightswipes</span> <span class="o">=</span> <span class="mi">0</span>
        <span class="bp">self</span><span class="o">.</span><span class="n">leftswipes</span> <span class="o">=</span> <span class="mi">0</span>
        <span class="bp">self</span><span class="o">.</span><span class="n">group</span> <span class="o">=</span> <span class="n">group</span>
    
    <span class="k">def</span> <span class="nf">connect</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">particle</span><span class="p">):</span>
        <span class="k">if</span> <span class="n">particle</span><span class="o">.</span><span class="n">gender</span> <span class="o">==</span> <span class="bp">self</span><span class="o">.</span><span class="n">gender</span> <span class="ow">or</span> <span class="bp">self</span><span class="o">.</span><span class="n">filterEvaluation</span><span class="p">(</span><span class="n">particle</span><span class="o">.</span><span class="n">elo</span><span class="p">):</span>
            <span class="k">return</span> <span class="s2">&quot;None&quot;</span>
        <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">swipeLeftEvaluation</span><span class="p">(</span><span class="n">particle</span><span class="o">.</span><span class="n">rating</span><span class="p">):</span>
            <span class="bp">self</span><span class="o">.</span><span class="n">leftswipes</span> <span class="o">+=</span> <span class="mi">1</span>
            <span class="k">return</span> <span class="s2">&quot;Left&quot;</span>
        <span class="bp">self</span><span class="o">.</span><span class="n">rightswipes</span> <span class="o">+=</span> <span class="mi">1</span>
        <span class="k">return</span> <span class="s2">&quot;Right&quot;</span>
    
    <span class="k">def</span> <span class="nf">update</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">particle</span><span class="p">,</span> <span class="n">status</span><span class="p">):</span>
        <span class="k">if</span> <span class="n">status</span> <span class="o">==</span> <span class="s2">&quot;Left&quot;</span><span class="p">:</span>
            <span class="bp">self</span><span class="o">.</span><span class="n">left</span><span class="p">[</span><span class="n">particle</span><span class="o">.</span><span class="n">ID</span><span class="p">]</span> <span class="o">=</span> <span class="n">particle</span><span class="o">.</span><span class="n">elo</span>
        <span class="k">if</span> <span class="n">status</span> <span class="o">==</span> <span class="s2">&quot;Right&quot;</span><span class="p">:</span>
            <span class="bp">self</span><span class="o">.</span><span class="n">right</span><span class="p">[</span><span class="n">particle</span><span class="o">.</span><span class="n">ID</span><span class="p">]</span> <span class="o">=</span> <span class="n">particle</span><span class="o">.</span><span class="n">elo</span>
        <span class="k">if</span> <span class="n">status</span> <span class="o">==</span> <span class="s2">&quot;None&quot;</span><span class="p">:</span>
            <span class="k">return</span>
            
    <span class="k">def</span> <span class="nf">filterEvaluation</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">elo</span><span class="p">):</span>
        <span class="k">return</span> <span class="bp">self</span><span class="o">.</span><span class="n">elo</span> <span class="o">&gt;</span> <span class="p">(</span><span class="n">elo</span> <span class="o">+</span> <span class="mi">2</span><span class="o">*</span><span class="n">sigma</span><span class="p">)</span>
    
    <span class="k">def</span> <span class="nf">computeElo</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
        <span class="n">count</span> <span class="o">=</span> <span class="mi">0</span>
        <span class="n">elo</span> <span class="o">=</span> <span class="mi">0</span>
        <span class="k">for</span> <span class="n">e</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">right</span><span class="o">.</span><span class="n">values</span><span class="p">():</span>
            <span class="n">elo</span> <span class="o">+=</span> <span class="p">(</span><span class="mi">2</span><span class="o">*</span><span class="n">sigma</span> <span class="o">+</span> <span class="n">e</span><span class="p">)</span>
            <span class="n">count</span> <span class="o">+=</span> <span class="mi">1</span>
        <span class="k">for</span> <span class="n">e</span> <span class="ow">in</span> <span class="bp">self</span><span class="o">.</span><span class="n">left</span><span class="o">.</span><span class="n">values</span><span class="p">():</span>
            <span class="n">elo</span> <span class="o">+=</span> <span class="p">(</span><span class="n">e</span> <span class="o">-</span> <span class="mi">2</span><span class="o">*</span><span class="n">sigma</span><span class="p">)</span>
            <span class="n">count</span> <span class="o">+=</span> <span class="mi">1</span>
        <span class="k">if</span> <span class="n">count</span> <span class="o">==</span> <span class="mi">0</span><span class="p">:</span>
            <span class="bp">self</span><span class="o">.</span><span class="n">elo</span> <span class="o">=</span> <span class="n">mu</span>
        <span class="k">else</span><span class="p">:</span>
            <span class="bp">self</span><span class="o">.</span><span class="n">elo</span> <span class="o">=</span> <span class="n">elo</span> <span class="o">/</span> <span class="n">count</span>
        <span class="bp">self</span><span class="o">.</span><span class="n">elo</span> <span class="o">-=</span> <span class="bp">self</span><span class="o">.</span><span class="n">rightswipes</span> <span class="o">*</span> <span class="mi">5</span>
        <span class="bp">self</span><span class="o">.</span><span class="n">elo</span> <span class="o">+=</span> <span class="nb">len</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">right</span><span class="p">)</span> <span class="o">*</span> <span class="mi">10</span>
    
    <span class="k">def</span> <span class="nf">swipeLeftEvaluation</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">rating</span><span class="p">):</span>
        <span class="k">if</span> <span class="bp">self</span><span class="o">.</span><span class="n">group</span> <span class="o">==</span> <span class="s1">&#39;allright&#39;</span><span class="p">:</span>
            <span class="k">return</span> <span class="kc">False</span>
        <span class="k">elif</span> <span class="bp">self</span><span class="o">.</span><span class="n">group</span> <span class="o">==</span> <span class="s1">&#39;half&#39;</span><span class="p">:</span>
            <span class="k">return</span> <span class="n">random</span><span class="o">.</span><span class="n">uniform</span><span class="p">(</span><span class="mi">0</span><span class="p">,</span> <span class="mi">1</span><span class="p">)</span> <span class="o">&gt;</span> <span class="mf">0.5</span>
        <span class="k">return</span> <span class="n">random</span><span class="o">.</span><span class="n">uniform</span><span class="p">(</span><span class="mi">0</span><span class="p">,</span> <span class="mi">1</span><span class="p">)</span> <span class="o">&gt;</span> <span class="n">ss</span><span class="o">.</span><span class="n">norm</span><span class="o">.</span><span class="n">cdf</span><span class="p">(</span><span class="n">rating</span><span class="p">,</span> <span class="bp">self</span><span class="o">.</span><span class="n">rating</span><span class="p">,</span> <span class="n">sigma</span><span class="p">)</span>
</pre></div>

    </div>
</div>
</div>

</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[7]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="k">class</span> <span class="nc">ParticleBox</span><span class="p">:</span>
    <span class="k">def</span> <span class="fm">__init__</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span>
                 <span class="n">init_state</span><span class="p">,</span>
                 <span class="n">bounds</span> <span class="o">=</span> <span class="p">[</span><span class="o">-</span><span class="n">boxlen</span><span class="p">,</span> <span class="n">boxlen</span><span class="p">,</span> <span class="o">-</span><span class="n">boxlen</span><span class="p">,</span> <span class="n">boxlen</span><span class="p">],</span>
                 <span class="n">size</span> <span class="o">=</span> <span class="mf">0.04</span><span class="p">,</span>
                 <span class="n">ratingarr</span> <span class="o">=</span> <span class="p">[],</span>
                 <span class="n">logprogress</span> <span class="o">=</span> <span class="kc">False</span><span class="p">):</span>
        <span class="n">M</span> <span class="o">=</span> <span class="mf">0.05</span>
        <span class="bp">self</span><span class="o">.</span><span class="n">m_average_likes</span> <span class="o">=</span> <span class="p">[[],[],[]]</span>
        <span class="bp">self</span><span class="o">.</span><span class="n">f_average_likes</span> <span class="o">=</span> <span class="p">[]</span>
        <span class="bp">self</span><span class="o">.</span><span class="n">m_average_elo</span> <span class="o">=</span> <span class="p">[[],[],[]]</span>
        <span class="bp">self</span><span class="o">.</span><span class="n">f_average_elo</span> <span class="o">=</span> <span class="p">[]</span>
        <span class="bp">self</span><span class="o">.</span><span class="n">logprogress</span> <span class="o">=</span> <span class="n">logprogress</span>
        <span class="bp">self</span><span class="o">.</span><span class="n">init_state</span> <span class="o">=</span> <span class="n">np</span><span class="o">.</span><span class="n">asarray</span><span class="p">(</span><span class="n">init_state</span><span class="p">,</span> <span class="n">dtype</span><span class="o">=</span><span class="nb">float</span><span class="p">)</span>
        <span class="bp">self</span><span class="o">.</span><span class="n">M</span> <span class="o">=</span> <span class="n">M</span> <span class="o">*</span> <span class="n">np</span><span class="o">.</span><span class="n">ones</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">init_state</span><span class="o">.</span><span class="n">shape</span><span class="p">[</span><span class="mi">0</span><span class="p">])</span>
        <span class="bp">self</span><span class="o">.</span><span class="n">size</span> <span class="o">=</span> <span class="n">size</span>
        <span class="bp">self</span><span class="o">.</span><span class="n">state</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">init_state</span><span class="o">.</span><span class="n">copy</span><span class="p">()</span>
        <span class="bp">self</span><span class="o">.</span><span class="n">time_elapsed</span> <span class="o">=</span> <span class="mi">0</span>
        <span class="bp">self</span><span class="o">.</span><span class="n">bounds</span> <span class="o">=</span> <span class="n">bounds</span>
        <span class="bp">self</span><span class="o">.</span><span class="n">particles</span> <span class="o">=</span> <span class="p">[]</span>
        <span class="k">for</span> <span class="n">i</span> <span class="ow">in</span> <span class="nb">range</span><span class="p">(</span><span class="mi">0</span><span class="p">,</span> <span class="nb">len</span><span class="p">(</span><span class="n">ratingarr</span><span class="p">)):</span>
            <span class="k">if</span> <span class="n">i</span> <span class="o">&lt;</span> <span class="n">m</span><span class="p">[</span><span class="mi">0</span><span class="p">]:</span>
                <span class="bp">self</span><span class="o">.</span><span class="n">particles</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">Particle</span><span class="p">(</span><span class="n">i</span><span class="p">,</span> <span class="s1">&#39;m&#39;</span><span class="p">,</span> <span class="n">ratingarr</span><span class="p">[</span><span class="n">i</span><span class="p">],</span> <span class="s1">&#39;normal&#39;</span><span class="p">))</span>
            <span class="k">elif</span> <span class="n">i</span> <span class="o">&lt;</span> <span class="n">m</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span> <span class="o">+</span> <span class="n">m</span><span class="p">[</span><span class="mi">1</span><span class="p">]:</span>
                <span class="bp">self</span><span class="o">.</span><span class="n">particles</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">Particle</span><span class="p">(</span><span class="n">i</span><span class="p">,</span> <span class="s1">&#39;m&#39;</span><span class="p">,</span> <span class="n">ratingarr</span><span class="p">[</span><span class="n">i</span><span class="p">],</span> <span class="s1">&#39;half&#39;</span><span class="p">))</span>
            <span class="k">elif</span> <span class="n">i</span> <span class="o">&lt;</span> <span class="nb">sum</span><span class="p">(</span><span class="n">m</span><span class="p">):</span>
                <span class="bp">self</span><span class="o">.</span><span class="n">particles</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">Particle</span><span class="p">(</span><span class="n">i</span><span class="p">,</span> <span class="s1">&#39;m&#39;</span><span class="p">,</span> <span class="n">ratingarr</span><span class="p">[</span><span class="n">i</span><span class="p">],</span> <span class="s1">&#39;allright&#39;</span><span class="p">))</span>
            <span class="k">else</span><span class="p">:</span>
                <span class="bp">self</span><span class="o">.</span><span class="n">particles</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">Particle</span><span class="p">(</span><span class="n">i</span><span class="p">,</span> <span class="s1">&#39;f&#39;</span><span class="p">,</span> <span class="n">ratingarr</span><span class="p">[</span><span class="n">i</span><span class="p">]))</span>
    
    <span class="k">def</span> <span class="nf">log</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
        <span class="k">if</span> <span class="ow">not</span> <span class="bp">self</span><span class="o">.</span><span class="n">logprogress</span><span class="p">:</span>
            <span class="k">return</span>
        <span class="n">m_likes</span> <span class="o">=</span> <span class="p">[</span><span class="mi">0</span><span class="p">,</span><span class="mi">0</span><span class="p">,</span><span class="mi">0</span><span class="p">]</span>
        <span class="n">f_likes</span> <span class="o">=</span> <span class="mi">0</span>
        <span class="n">m_elo</span> <span class="o">=</span> <span class="p">[</span><span class="mi">0</span><span class="p">,</span><span class="mi">0</span><span class="p">,</span><span class="mi">0</span><span class="p">]</span>
        <span class="n">f_elo</span> <span class="o">=</span> <span class="mi">0</span>
        <span class="k">for</span> <span class="n">i</span> <span class="ow">in</span> <span class="nb">range</span><span class="p">(</span><span class="mi">0</span><span class="p">,</span> <span class="nb">sum</span><span class="p">(</span><span class="n">m</span><span class="p">)</span><span class="o">+</span><span class="n">f</span><span class="p">):</span>
            <span class="k">if</span> <span class="n">i</span> <span class="o">&lt;</span> <span class="n">m</span><span class="p">[</span><span class="mi">0</span><span class="p">]:</span>
                <span class="n">m_likes</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span> <span class="o">+=</span> <span class="nb">len</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">particles</span><span class="p">[</span><span class="n">i</span><span class="p">]</span><span class="o">.</span><span class="n">right</span><span class="p">)</span>
                <span class="n">m_elo</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span> <span class="o">+=</span> <span class="bp">self</span><span class="o">.</span><span class="n">particles</span><span class="p">[</span><span class="n">i</span><span class="p">]</span><span class="o">.</span><span class="n">elo</span>
            <span class="k">elif</span> <span class="n">i</span> <span class="o">&lt;</span> <span class="n">m</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span> <span class="o">+</span> <span class="n">m</span><span class="p">[</span><span class="mi">1</span><span class="p">]:</span>
                <span class="n">m_likes</span><span class="p">[</span><span class="mi">1</span><span class="p">]</span> <span class="o">+=</span> <span class="nb">len</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">particles</span><span class="p">[</span><span class="n">i</span><span class="p">]</span><span class="o">.</span><span class="n">right</span><span class="p">)</span>
                <span class="n">m_elo</span><span class="p">[</span><span class="mi">1</span><span class="p">]</span> <span class="o">+=</span> <span class="bp">self</span><span class="o">.</span><span class="n">particles</span><span class="p">[</span><span class="n">i</span><span class="p">]</span><span class="o">.</span><span class="n">elo</span>
            <span class="k">elif</span> <span class="n">i</span> <span class="o">&lt;</span> <span class="nb">sum</span><span class="p">(</span><span class="n">m</span><span class="p">):</span>
                <span class="n">m_likes</span><span class="p">[</span><span class="mi">2</span><span class="p">]</span> <span class="o">+=</span> <span class="nb">len</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">particles</span><span class="p">[</span><span class="n">i</span><span class="p">]</span><span class="o">.</span><span class="n">right</span><span class="p">)</span>
                <span class="n">m_elo</span><span class="p">[</span><span class="mi">2</span><span class="p">]</span> <span class="o">+=</span> <span class="bp">self</span><span class="o">.</span><span class="n">particles</span><span class="p">[</span><span class="n">i</span><span class="p">]</span><span class="o">.</span><span class="n">elo</span>
            <span class="k">else</span><span class="p">:</span>
                <span class="n">f_likes</span> <span class="o">+=</span> <span class="nb">len</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">particles</span><span class="p">[</span><span class="n">i</span><span class="p">]</span><span class="o">.</span><span class="n">right</span><span class="p">)</span>
                <span class="n">f_elo</span> <span class="o">+=</span> <span class="bp">self</span><span class="o">.</span><span class="n">particles</span><span class="p">[</span><span class="n">i</span><span class="p">]</span><span class="o">.</span><span class="n">elo</span>

        <span class="bp">self</span><span class="o">.</span><span class="n">m_average_likes</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">m_likes</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span> <span class="o">/</span> <span class="n">m</span><span class="p">[</span><span class="mi">0</span><span class="p">])</span>
        <span class="bp">self</span><span class="o">.</span><span class="n">m_average_likes</span><span class="p">[</span><span class="mi">1</span><span class="p">]</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">m_likes</span><span class="p">[</span><span class="mi">1</span><span class="p">]</span> <span class="o">/</span> <span class="n">m</span><span class="p">[</span><span class="mi">1</span><span class="p">])</span>
        <span class="bp">self</span><span class="o">.</span><span class="n">m_average_likes</span><span class="p">[</span><span class="mi">2</span><span class="p">]</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">m_likes</span><span class="p">[</span><span class="mi">2</span><span class="p">]</span> <span class="o">/</span> <span class="n">m</span><span class="p">[</span><span class="mi">2</span><span class="p">])</span>
        <span class="bp">self</span><span class="o">.</span><span class="n">f_average_likes</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">f_likes</span> <span class="o">/</span> <span class="n">f</span><span class="p">)</span>
        
        <span class="bp">self</span><span class="o">.</span><span class="n">m_average_elo</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">m_elo</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span> <span class="o">/</span> <span class="n">m</span><span class="p">[</span><span class="mi">0</span><span class="p">])</span>
        <span class="bp">self</span><span class="o">.</span><span class="n">m_average_elo</span><span class="p">[</span><span class="mi">1</span><span class="p">]</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">m_elo</span><span class="p">[</span><span class="mi">1</span><span class="p">]</span> <span class="o">/</span> <span class="n">m</span><span class="p">[</span><span class="mi">1</span><span class="p">])</span>
        <span class="bp">self</span><span class="o">.</span><span class="n">m_average_elo</span><span class="p">[</span><span class="mi">2</span><span class="p">]</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">m_elo</span><span class="p">[</span><span class="mi">2</span><span class="p">]</span> <span class="o">/</span> <span class="n">m</span><span class="p">[</span><span class="mi">2</span><span class="p">])</span>
        <span class="bp">self</span><span class="o">.</span><span class="n">f_average_elo</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">f_elo</span> <span class="o">/</span> <span class="n">f</span><span class="p">)</span>
        
    <span class="k">def</span> <span class="nf">step</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">dt</span><span class="p">):</span>
        <span class="bp">self</span><span class="o">.</span><span class="n">log</span><span class="p">()</span>
        <span class="bp">self</span><span class="o">.</span><span class="n">time_elapsed</span> <span class="o">+=</span> <span class="n">dt</span>
        <span class="bp">self</span><span class="o">.</span><span class="n">state</span><span class="p">[:,</span> <span class="p">:</span><span class="mi">2</span><span class="p">]</span> <span class="o">+=</span> <span class="n">dt</span> <span class="o">*</span> <span class="bp">self</span><span class="o">.</span><span class="n">state</span><span class="p">[:,</span> <span class="mi">2</span><span class="p">:]</span>
        
        <span class="n">D</span> <span class="o">=</span> <span class="n">squareform</span><span class="p">(</span><span class="n">pdist</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">state</span><span class="p">[:,</span> <span class="p">:</span><span class="mi">2</span><span class="p">]))</span>
        <span class="n">ind1</span><span class="p">,</span> <span class="n">ind2</span> <span class="o">=</span> <span class="n">np</span><span class="o">.</span><span class="n">where</span><span class="p">(</span><span class="n">D</span> <span class="o">&lt;</span> <span class="mi">2</span> <span class="o">*</span> <span class="bp">self</span><span class="o">.</span><span class="n">size</span><span class="p">)</span>
        <span class="n">unique</span> <span class="o">=</span> <span class="p">(</span><span class="n">ind1</span> <span class="o">&lt;</span> <span class="n">ind2</span><span class="p">)</span>
        <span class="n">ind1</span> <span class="o">=</span> <span class="n">ind1</span><span class="p">[</span><span class="n">unique</span><span class="p">]</span>
        <span class="n">ind2</span> <span class="o">=</span> <span class="n">ind2</span><span class="p">[</span><span class="n">unique</span><span class="p">]</span>

        <span class="k">for</span> <span class="n">i1</span><span class="p">,</span> <span class="n">i2</span> <span class="ow">in</span> <span class="nb">zip</span><span class="p">(</span><span class="n">ind1</span><span class="p">,</span> <span class="n">ind2</span><span class="p">):</span>
            <span class="bp">self</span><span class="o">.</span><span class="n">connect</span><span class="p">(</span><span class="n">i1</span><span class="p">,</span> <span class="n">i2</span><span class="p">)</span>
            
            <span class="c1"># Perfectly elastic Collision</span>
            <span class="n">m1</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">M</span><span class="p">[</span><span class="n">i1</span><span class="p">]</span>
            <span class="n">m2</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">M</span><span class="p">[</span><span class="n">i2</span><span class="p">]</span>
            
            <span class="n">r1</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">state</span><span class="p">[</span><span class="n">i1</span><span class="p">,</span> <span class="p">:</span><span class="mi">2</span><span class="p">]</span>
            <span class="n">r2</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">state</span><span class="p">[</span><span class="n">i2</span><span class="p">,</span> <span class="p">:</span><span class="mi">2</span><span class="p">]</span>

            <span class="n">v1</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">state</span><span class="p">[</span><span class="n">i1</span><span class="p">,</span> <span class="mi">2</span><span class="p">:]</span>
            <span class="n">v2</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">state</span><span class="p">[</span><span class="n">i2</span><span class="p">,</span> <span class="mi">2</span><span class="p">:]</span>

            <span class="n">r_rel</span> <span class="o">=</span> <span class="n">r1</span> <span class="o">-</span> <span class="n">r2</span>
            <span class="n">v_rel</span> <span class="o">=</span> <span class="n">v1</span> <span class="o">-</span> <span class="n">v2</span>

            <span class="n">v_cm</span> <span class="o">=</span> <span class="p">(</span><span class="n">m1</span> <span class="o">*</span> <span class="n">v1</span> <span class="o">+</span> <span class="n">m2</span> <span class="o">*</span> <span class="n">v2</span><span class="p">)</span> <span class="o">/</span> <span class="p">(</span><span class="n">m1</span> <span class="o">+</span> <span class="n">m2</span><span class="p">)</span>

            <span class="c1"># collisions of spheres reflect v_rel over r_rel</span>
            <span class="n">rr_rel</span> <span class="o">=</span> <span class="n">np</span><span class="o">.</span><span class="n">dot</span><span class="p">(</span><span class="n">r_rel</span><span class="p">,</span> <span class="n">r_rel</span><span class="p">)</span>
            <span class="n">vr_rel</span> <span class="o">=</span> <span class="n">np</span><span class="o">.</span><span class="n">dot</span><span class="p">(</span><span class="n">v_rel</span><span class="p">,</span> <span class="n">r_rel</span><span class="p">)</span>
            <span class="n">v_rel</span> <span class="o">=</span> <span class="mi">2</span> <span class="o">*</span> <span class="n">r_rel</span> <span class="o">*</span> <span class="n">vr_rel</span> <span class="o">/</span> <span class="n">rr_rel</span> <span class="o">-</span> <span class="n">v_rel</span>

            <span class="c1"># assign new velocities</span>
            <span class="bp">self</span><span class="o">.</span><span class="n">state</span><span class="p">[</span><span class="n">i1</span><span class="p">,</span> <span class="mi">2</span><span class="p">:]</span> <span class="o">=</span> <span class="n">v_cm</span> <span class="o">+</span> <span class="n">v_rel</span> <span class="o">*</span> <span class="n">m2</span> <span class="o">/</span> <span class="p">(</span><span class="n">m1</span> <span class="o">+</span> <span class="n">m2</span><span class="p">)</span>
            <span class="bp">self</span><span class="o">.</span><span class="n">state</span><span class="p">[</span><span class="n">i2</span><span class="p">,</span> <span class="mi">2</span><span class="p">:]</span> <span class="o">=</span> <span class="n">v_cm</span> <span class="o">-</span> <span class="n">v_rel</span> <span class="o">*</span> <span class="n">m1</span> <span class="o">/</span> <span class="p">(</span><span class="n">m1</span> <span class="o">+</span> <span class="n">m2</span><span class="p">)</span> 
            
        <span class="c1"># check for crossing boundary</span>
        <span class="n">crossed_x1</span> <span class="o">=</span> <span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">state</span><span class="p">[:,</span> <span class="mi">0</span><span class="p">]</span> <span class="o">&lt;</span> <span class="bp">self</span><span class="o">.</span><span class="n">bounds</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span> <span class="o">+</span> <span class="bp">self</span><span class="o">.</span><span class="n">size</span><span class="p">)</span>
        <span class="n">crossed_x2</span> <span class="o">=</span> <span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">state</span><span class="p">[:,</span> <span class="mi">0</span><span class="p">]</span> <span class="o">&gt;</span> <span class="bp">self</span><span class="o">.</span><span class="n">bounds</span><span class="p">[</span><span class="mi">1</span><span class="p">]</span> <span class="o">-</span> <span class="bp">self</span><span class="o">.</span><span class="n">size</span><span class="p">)</span>
        <span class="n">crossed_y1</span> <span class="o">=</span> <span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">state</span><span class="p">[:,</span> <span class="mi">1</span><span class="p">]</span> <span class="o">&lt;</span> <span class="bp">self</span><span class="o">.</span><span class="n">bounds</span><span class="p">[</span><span class="mi">2</span><span class="p">]</span> <span class="o">+</span> <span class="bp">self</span><span class="o">.</span><span class="n">size</span><span class="p">)</span>
        <span class="n">crossed_y2</span> <span class="o">=</span> <span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">state</span><span class="p">[:,</span> <span class="mi">1</span><span class="p">]</span> <span class="o">&gt;</span> <span class="bp">self</span><span class="o">.</span><span class="n">bounds</span><span class="p">[</span><span class="mi">3</span><span class="p">]</span> <span class="o">-</span> <span class="bp">self</span><span class="o">.</span><span class="n">size</span><span class="p">)</span>

        <span class="bp">self</span><span class="o">.</span><span class="n">state</span><span class="p">[</span><span class="n">crossed_x1</span><span class="p">,</span> <span class="mi">0</span><span class="p">]</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">bounds</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span> <span class="o">+</span> <span class="bp">self</span><span class="o">.</span><span class="n">size</span>
        <span class="bp">self</span><span class="o">.</span><span class="n">state</span><span class="p">[</span><span class="n">crossed_x2</span><span class="p">,</span> <span class="mi">0</span><span class="p">]</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">bounds</span><span class="p">[</span><span class="mi">1</span><span class="p">]</span> <span class="o">-</span> <span class="bp">self</span><span class="o">.</span><span class="n">size</span>

        <span class="bp">self</span><span class="o">.</span><span class="n">state</span><span class="p">[</span><span class="n">crossed_y1</span><span class="p">,</span> <span class="mi">1</span><span class="p">]</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">bounds</span><span class="p">[</span><span class="mi">2</span><span class="p">]</span> <span class="o">+</span> <span class="bp">self</span><span class="o">.</span><span class="n">size</span>
        <span class="bp">self</span><span class="o">.</span><span class="n">state</span><span class="p">[</span><span class="n">crossed_y2</span><span class="p">,</span> <span class="mi">1</span><span class="p">]</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">bounds</span><span class="p">[</span><span class="mi">3</span><span class="p">]</span> <span class="o">-</span> <span class="bp">self</span><span class="o">.</span><span class="n">size</span>

        <span class="bp">self</span><span class="o">.</span><span class="n">state</span><span class="p">[</span><span class="n">crossed_x1</span> <span class="o">|</span> <span class="n">crossed_x2</span><span class="p">,</span> <span class="mi">2</span><span class="p">]</span> <span class="o">*=</span> <span class="o">-</span><span class="mi">1</span>
        <span class="bp">self</span><span class="o">.</span><span class="n">state</span><span class="p">[</span><span class="n">crossed_y1</span> <span class="o">|</span> <span class="n">crossed_y2</span><span class="p">,</span> <span class="mi">3</span><span class="p">]</span> <span class="o">*=</span> <span class="o">-</span><span class="mi">1</span>
    
    <span class="k">def</span> <span class="nf">connect</span><span class="p">(</span><span class="bp">self</span><span class="p">,</span> <span class="n">ind1</span><span class="p">,</span> <span class="n">ind2</span><span class="p">):</span>
        <span class="n">particle_a</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">particles</span><span class="p">[</span><span class="n">ind1</span><span class="p">]</span>
        <span class="n">particle_b</span> <span class="o">=</span> <span class="bp">self</span><span class="o">.</span><span class="n">particles</span><span class="p">[</span><span class="n">ind2</span><span class="p">]</span>
        <span class="k">if</span> <span class="n">particle_a</span><span class="o">.</span><span class="n">gender</span> <span class="o">==</span> <span class="n">particle_b</span><span class="o">.</span><span class="n">gender</span><span class="p">:</span>
            <span class="k">return</span>
        <span class="k">if</span> <span class="n">particle_a</span><span class="o">.</span><span class="n">ID</span> <span class="ow">not</span> <span class="ow">in</span> <span class="n">particle_b</span><span class="o">.</span><span class="n">left</span> <span class="ow">and</span> <span class="n">particle_a</span><span class="o">.</span><span class="n">ID</span> <span class="ow">not</span> <span class="ow">in</span> <span class="n">particle_b</span><span class="o">.</span><span class="n">right</span><span class="p">:</span>
            <span class="n">a_swipe_b</span> <span class="o">=</span> <span class="n">particle_a</span><span class="o">.</span><span class="n">connect</span><span class="p">(</span><span class="n">particle_b</span><span class="p">)</span>
            <span class="n">particle_b</span><span class="o">.</span><span class="n">update</span><span class="p">(</span><span class="n">particle_a</span><span class="p">,</span> <span class="n">a_swipe_b</span><span class="p">)</span>
        <span class="k">if</span> <span class="n">particle_b</span><span class="o">.</span><span class="n">ID</span> <span class="ow">not</span> <span class="ow">in</span> <span class="n">particle_a</span><span class="o">.</span><span class="n">left</span> <span class="ow">and</span> <span class="n">particle_b</span><span class="o">.</span><span class="n">ID</span> <span class="ow">not</span> <span class="ow">in</span> <span class="n">particle_a</span><span class="o">.</span><span class="n">right</span><span class="p">:</span>
            <span class="n">b_swipe_a</span><span class="o">=</span> <span class="n">particle_b</span><span class="o">.</span><span class="n">connect</span><span class="p">(</span><span class="n">particle_a</span><span class="p">)</span>
            <span class="n">particle_a</span><span class="o">.</span><span class="n">update</span><span class="p">(</span><span class="n">particle_b</span><span class="p">,</span> <span class="n">b_swipe_a</span><span class="p">)</span>
        <span class="n">particle_a</span><span class="o">.</span><span class="n">computeElo</span><span class="p">()</span>
        <span class="n">particle_b</span><span class="o">.</span><span class="n">computeElo</span><span class="p">()</span>
        
    <span class="k">def</span> <span class="nf">plotDistributions</span><span class="p">(</span><span class="bp">self</span><span class="p">):</span>
        <span class="n">elos</span> <span class="o">=</span> <span class="p">[]</span>
        <span class="n">ratings</span> <span class="o">=</span> <span class="p">[]</span>
        <span class="k">for</span> <span class="n">i</span> <span class="ow">in</span> <span class="nb">range</span><span class="p">(</span><span class="mi">0</span><span class="p">,</span> <span class="nb">len</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">particles</span><span class="p">)):</span>
            <span class="n">ratings</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">particles</span><span class="p">[</span><span class="n">i</span><span class="p">]</span><span class="o">.</span><span class="n">rating</span><span class="p">)</span>
            <span class="n">elos</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="bp">self</span><span class="o">.</span><span class="n">particles</span><span class="p">[</span><span class="n">i</span><span class="p">]</span><span class="o">.</span><span class="n">elo</span><span class="p">)</span>
        <span class="n">fig</span><span class="p">,</span> <span class="n">axes</span> <span class="o">=</span> <span class="n">plt</span><span class="o">.</span><span class="n">subplots</span><span class="p">(</span><span class="n">nrows</span><span class="o">=</span><span class="mi">1</span><span class="p">,</span> <span class="n">ncols</span><span class="o">=</span><span class="mi">2</span><span class="p">,</span> <span class="n">figsize</span><span class="o">=</span><span class="p">(</span><span class="mi">12</span><span class="p">,</span> <span class="mi">5</span><span class="p">))</span>
        <span class="n">sns</span><span class="o">.</span><span class="n">distplot</span><span class="p">(</span><span class="n">elos</span><span class="p">,</span> <span class="n">hist</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span> <span class="n">kde</span><span class="o">=</span><span class="kc">False</span><span class="p">,</span> 
             <span class="n">bins</span><span class="o">=</span><span class="nb">int</span><span class="p">(</span><span class="mi">180</span><span class="o">/</span><span class="mi">5</span><span class="p">),</span> <span class="n">color</span> <span class="o">=</span> <span class="s1">&#39;blue&#39;</span><span class="p">,</span> <span class="n">ax</span><span class="o">=</span><span class="n">axes</span><span class="p">[</span><span class="mi">0</span><span class="p">],</span>
             <span class="n">hist_kws</span><span class="o">=</span><span class="p">{</span><span class="s1">&#39;edgecolor&#39;</span><span class="p">:</span><span class="s1">&#39;black&#39;</span><span class="p">})</span><span class="o">.</span><span class="n">set_title</span><span class="p">(</span><span class="s2">&quot;Empirical Elo Distribution&quot;</span><span class="p">)</span>
        <span class="n">sns</span><span class="o">.</span><span class="n">distplot</span><span class="p">(</span><span class="n">ratings</span><span class="p">,</span> <span class="n">hist</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span> <span class="n">kde</span><span class="o">=</span><span class="kc">False</span><span class="p">,</span> 
             <span class="n">bins</span><span class="o">=</span><span class="nb">int</span><span class="p">(</span><span class="mi">180</span><span class="o">/</span><span class="mi">5</span><span class="p">),</span> <span class="n">color</span> <span class="o">=</span> <span class="s1">&#39;blue&#39;</span><span class="p">,</span> <span class="n">ax</span><span class="o">=</span><span class="n">axes</span><span class="p">[</span><span class="mi">1</span><span class="p">],</span>
             <span class="n">hist_kws</span><span class="o">=</span><span class="p">{</span><span class="s1">&#39;edgecolor&#39;</span><span class="p">:</span><span class="s1">&#39;black&#39;</span><span class="p">})</span><span class="o">.</span><span class="n">set_title</span><span class="p">(</span><span class="s2">&quot;Empirical Rating Distribution&quot;</span><span class="p">)</span>
</pre></div>

    </div>
</div>
</div>

</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[8]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">m_elo</span> <span class="o">=</span> <span class="p">[[],[],[]]</span>
<span class="n">f_elo</span> <span class="o">=</span> <span class="p">[]</span>
<span class="n">m_likes</span> <span class="o">=</span> <span class="p">[[],[],[]]</span>
<span class="n">f_likes</span> <span class="o">=</span> <span class="p">[]</span>
<span class="k">for</span> <span class="n">i</span> <span class="ow">in</span> <span class="nb">range</span><span class="p">(</span><span class="mi">0</span><span class="p">,</span> <span class="n">iterations</span><span class="p">):</span>
    <span class="c1"># Rerun this block of code for repeated simulations</span>
    <span class="c1">############################################################################################################</span>
    <span class="n">np</span><span class="o">.</span><span class="n">random</span><span class="o">.</span><span class="n">seed</span><span class="p">(</span><span class="mi">0</span><span class="p">)</span>
    <span class="n">init_state</span> <span class="o">=</span> <span class="o">-</span><span class="mf">0.5</span> <span class="o">+</span> <span class="n">np</span><span class="o">.</span><span class="n">random</span><span class="o">.</span><span class="n">random</span><span class="p">((</span><span class="nb">sum</span><span class="p">(</span><span class="n">m</span><span class="p">)</span><span class="o">+</span><span class="n">f</span><span class="p">,</span> <span class="mi">4</span><span class="p">))</span>
    <span class="n">init_state</span><span class="p">[:,</span> <span class="p">:</span><span class="mi">2</span><span class="p">]</span> <span class="o">*=</span> <span class="p">(</span><span class="n">boxlen</span><span class="o">*</span><span class="mf">1.5</span><span class="p">)</span>

    <span class="n">box</span> <span class="o">=</span> <span class="n">ParticleBox</span><span class="p">(</span><span class="n">init_state</span><span class="p">,</span> <span class="n">size</span><span class="o">=</span><span class="mf">0.1</span><span class="p">,</span> <span class="n">ratingarr</span> <span class="o">=</span> <span class="n">copy</span><span class="o">.</span><span class="n">deepcopy</span><span class="p">(</span><span class="n">user_ratings</span><span class="p">),</span> <span class="n">logprogress</span> <span class="o">=</span> <span class="kc">True</span><span class="p">)</span>
    <span class="n">dt</span> <span class="o">=</span> <span class="mf">1.</span> <span class="o">/</span> <span class="n">fps</span> 

    <span class="c1"># set up figure and animation</span>
    <span class="n">fig</span> <span class="o">=</span> <span class="n">plt</span><span class="o">.</span><span class="n">figure</span><span class="p">()</span>
    <span class="n">fig</span><span class="o">.</span><span class="n">subplots_adjust</span><span class="p">(</span><span class="n">left</span><span class="o">=</span><span class="mi">0</span><span class="p">,</span> <span class="n">right</span><span class="o">=</span><span class="mi">1</span><span class="p">,</span> <span class="n">bottom</span><span class="o">=</span><span class="mi">0</span><span class="p">,</span> <span class="n">top</span><span class="o">=</span><span class="mi">1</span><span class="p">)</span>
    <span class="n">ax</span> <span class="o">=</span> <span class="n">fig</span><span class="o">.</span><span class="n">add_subplot</span><span class="p">(</span><span class="mi">111</span><span class="p">,</span> <span class="n">aspect</span><span class="o">=</span><span class="s1">&#39;equal&#39;</span><span class="p">,</span> <span class="n">autoscale_on</span><span class="o">=</span><span class="kc">False</span><span class="p">,</span>
                         <span class="n">xlim</span><span class="o">=</span><span class="p">(</span><span class="o">-</span><span class="n">graphlen</span><span class="p">,</span> <span class="n">graphlen</span><span class="p">),</span> <span class="n">ylim</span><span class="o">=</span><span class="p">(</span><span class="o">-</span><span class="n">graphlen</span><span class="p">,</span> <span class="n">graphlen</span><span class="p">))</span>

    <span class="c1"># particles holds the locations of the particles</span>
    <span class="n">particles_f</span><span class="p">,</span> <span class="o">=</span> <span class="n">ax</span><span class="o">.</span><span class="n">plot</span><span class="p">([],</span> <span class="p">[],</span> <span class="s1">&#39;ro&#39;</span><span class="p">,</span> <span class="n">ms</span><span class="o">=</span><span class="mi">4</span><span class="p">)</span>
    <span class="n">particles_m1</span><span class="p">,</span> <span class="o">=</span> <span class="n">ax</span><span class="o">.</span><span class="n">plot</span><span class="p">([],</span> <span class="p">[],</span> <span class="s1">&#39;o&#39;</span><span class="p">,</span> <span class="n">color</span> <span class="o">=</span> <span class="s1">&#39;blue&#39;</span><span class="p">,</span> <span class="n">ms</span><span class="o">=</span><span class="mi">4</span><span class="p">)</span>
    <span class="n">particles_m2</span><span class="p">,</span> <span class="o">=</span> <span class="n">ax</span><span class="o">.</span><span class="n">plot</span><span class="p">([],</span> <span class="p">[],</span> <span class="s1">&#39;o&#39;</span><span class="p">,</span> <span class="n">color</span> <span class="o">=</span> <span class="s1">&#39;royalblue&#39;</span><span class="p">,</span> <span class="n">ms</span><span class="o">=</span><span class="mi">4</span><span class="p">)</span>
    <span class="n">particles_m3</span><span class="p">,</span> <span class="o">=</span> <span class="n">ax</span><span class="o">.</span><span class="n">plot</span><span class="p">([],</span> <span class="p">[],</span> <span class="s1">&#39;o&#39;</span><span class="p">,</span> <span class="n">color</span> <span class="o">=</span> <span class="s1">&#39;lightskyblue&#39;</span><span class="p">,</span> <span class="n">ms</span><span class="o">=</span><span class="mi">4</span><span class="p">)</span>

    <span class="c1"># box edge</span>
    <span class="n">rect</span> <span class="o">=</span> <span class="n">plt</span><span class="o">.</span><span class="n">Rectangle</span><span class="p">(</span><span class="n">box</span><span class="o">.</span><span class="n">bounds</span><span class="p">[::</span><span class="mi">2</span><span class="p">],</span>
                         <span class="n">box</span><span class="o">.</span><span class="n">bounds</span><span class="p">[</span><span class="mi">1</span><span class="p">]</span> <span class="o">-</span> <span class="n">box</span><span class="o">.</span><span class="n">bounds</span><span class="p">[</span><span class="mi">0</span><span class="p">],</span>
                         <span class="n">box</span><span class="o">.</span><span class="n">bounds</span><span class="p">[</span><span class="mi">3</span><span class="p">]</span> <span class="o">-</span> <span class="n">box</span><span class="o">.</span><span class="n">bounds</span><span class="p">[</span><span class="mi">2</span><span class="p">],</span>
                         <span class="n">ec</span><span class="o">=</span><span class="s1">&#39;none&#39;</span><span class="p">,</span> <span class="n">lw</span><span class="o">=</span><span class="mi">2</span><span class="p">,</span> <span class="n">fc</span><span class="o">=</span><span class="s1">&#39;none&#39;</span><span class="p">)</span>
    <span class="n">ax</span><span class="o">.</span><span class="n">add_patch</span><span class="p">(</span><span class="n">rect</span><span class="p">)</span>

    <span class="k">def</span> <span class="nf">init</span><span class="p">():</span>
        <span class="sd">&quot;&quot;&quot;initialize animation&quot;&quot;&quot;</span>
        <span class="k">global</span> <span class="n">box</span><span class="p">,</span> <span class="n">rect</span>
        <span class="n">particles_f</span><span class="o">.</span><span class="n">set_data</span><span class="p">([],</span> <span class="p">[])</span>
        <span class="n">particles_m1</span><span class="o">.</span><span class="n">set_data</span><span class="p">([],</span> <span class="p">[])</span>
        <span class="n">particles_m2</span><span class="o">.</span><span class="n">set_data</span><span class="p">([],</span> <span class="p">[])</span>
        <span class="n">particles_m3</span><span class="o">.</span><span class="n">set_data</span><span class="p">([],</span> <span class="p">[])</span>
        <span class="n">rect</span><span class="o">.</span><span class="n">set_edgecolor</span><span class="p">(</span><span class="s1">&#39;none&#39;</span><span class="p">)</span>
        <span class="k">return</span> <span class="n">particles_f</span><span class="p">,</span> <span class="n">particles_m1</span><span class="p">,</span> <span class="n">particles_m2</span><span class="p">,</span> <span class="n">particles_m3</span><span class="p">,</span> <span class="n">rect</span>

    <span class="k">def</span> <span class="nf">animate</span><span class="p">(</span><span class="n">i</span><span class="p">):</span>
        <span class="sd">&quot;&quot;&quot;perform animation step&quot;&quot;&quot;</span>
        <span class="k">global</span> <span class="n">box</span><span class="p">,</span> <span class="n">rect</span><span class="p">,</span> <span class="n">dt</span><span class="p">,</span> <span class="n">ax</span><span class="p">,</span> <span class="n">fig</span>
        <span class="n">box</span><span class="o">.</span><span class="n">step</span><span class="p">(</span><span class="n">dt</span><span class="p">)</span>

        <span class="n">ms</span> <span class="o">=</span> <span class="nb">int</span><span class="p">(</span><span class="n">fig</span><span class="o">.</span><span class="n">dpi</span> <span class="o">*</span> <span class="mi">2</span> <span class="o">*</span> <span class="n">box</span><span class="o">.</span><span class="n">size</span> <span class="o">*</span> <span class="n">fig</span><span class="o">.</span><span class="n">get_figwidth</span><span class="p">()</span>
                 <span class="o">/</span> <span class="n">np</span><span class="o">.</span><span class="n">diff</span><span class="p">(</span><span class="n">ax</span><span class="o">.</span><span class="n">get_xbound</span><span class="p">())[</span><span class="mi">0</span><span class="p">])</span>

        <span class="c1"># update pieces of the animation</span>
        <span class="n">rect</span><span class="o">.</span><span class="n">set_edgecolor</span><span class="p">(</span><span class="s1">&#39;k&#39;</span><span class="p">)</span>
        <span class="n">particles_f</span><span class="o">.</span><span class="n">set_data</span><span class="p">(</span><span class="n">box</span><span class="o">.</span><span class="n">state</span><span class="p">[</span><span class="nb">sum</span><span class="p">(</span><span class="n">m</span><span class="p">):,</span> <span class="mi">0</span><span class="p">],</span> <span class="n">box</span><span class="o">.</span><span class="n">state</span><span class="p">[</span><span class="nb">sum</span><span class="p">(</span><span class="n">m</span><span class="p">):,</span> <span class="mi">1</span><span class="p">])</span>
        <span class="n">particles_f</span><span class="o">.</span><span class="n">set_markersize</span><span class="p">(</span><span class="n">ms</span><span class="p">)</span>
        <span class="n">particles_m1</span><span class="o">.</span><span class="n">set_data</span><span class="p">(</span><span class="n">box</span><span class="o">.</span><span class="n">state</span><span class="p">[</span><span class="mi">0</span><span class="p">:</span><span class="n">m</span><span class="p">[</span><span class="mi">0</span><span class="p">],</span> <span class="mi">0</span><span class="p">],</span> <span class="n">box</span><span class="o">.</span><span class="n">state</span><span class="p">[</span><span class="mi">0</span><span class="p">:</span><span class="n">m</span><span class="p">[</span><span class="mi">0</span><span class="p">],</span> <span class="mi">1</span><span class="p">])</span>
        <span class="n">particles_m1</span><span class="o">.</span><span class="n">set_markersize</span><span class="p">(</span><span class="n">ms</span><span class="p">)</span>
        <span class="n">particles_m2</span><span class="o">.</span><span class="n">set_data</span><span class="p">(</span><span class="n">box</span><span class="o">.</span><span class="n">state</span><span class="p">[</span><span class="n">m</span><span class="p">[</span><span class="mi">0</span><span class="p">]:</span><span class="n">m</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span> <span class="o">+</span> <span class="n">m</span><span class="p">[</span><span class="mi">1</span><span class="p">],</span> <span class="mi">0</span><span class="p">],</span> <span class="n">box</span><span class="o">.</span><span class="n">state</span><span class="p">[</span><span class="n">m</span><span class="p">[</span><span class="mi">0</span><span class="p">]:</span> <span class="n">m</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span> <span class="o">+</span> <span class="n">m</span><span class="p">[</span><span class="mi">1</span><span class="p">],</span> <span class="mi">1</span><span class="p">])</span>
        <span class="n">particles_m2</span><span class="o">.</span><span class="n">set_markersize</span><span class="p">(</span><span class="n">ms</span><span class="p">)</span>
        <span class="n">particles_m3</span><span class="o">.</span><span class="n">set_data</span><span class="p">(</span><span class="n">box</span><span class="o">.</span><span class="n">state</span><span class="p">[</span><span class="n">m</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span> <span class="o">+</span> <span class="n">m</span><span class="p">[</span><span class="mi">1</span><span class="p">]:</span><span class="nb">sum</span><span class="p">(</span><span class="n">m</span><span class="p">),</span> <span class="mi">0</span><span class="p">],</span> <span class="n">box</span><span class="o">.</span><span class="n">state</span><span class="p">[</span><span class="n">m</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span> <span class="o">+</span> <span class="n">m</span><span class="p">[</span><span class="mi">1</span><span class="p">]:</span><span class="nb">sum</span><span class="p">(</span><span class="n">m</span><span class="p">),</span> <span class="mi">1</span><span class="p">])</span>
        <span class="n">particles_m3</span><span class="o">.</span><span class="n">set_markersize</span><span class="p">(</span><span class="n">ms</span><span class="p">)</span>
        <span class="k">return</span> <span class="n">particles_f</span><span class="p">,</span> <span class="n">particles_m1</span><span class="p">,</span> <span class="n">particles_m2</span><span class="p">,</span> <span class="n">particles_m3</span><span class="p">,</span> <span class="n">rect</span>

    <span class="n">ani</span> <span class="o">=</span> <span class="n">animation</span><span class="o">.</span><span class="n">FuncAnimation</span><span class="p">(</span><span class="n">fig</span><span class="p">,</span> <span class="n">animate</span><span class="p">,</span> <span class="n">frames</span><span class="o">=</span><span class="n">frames</span><span class="p">,</span>
                                  <span class="n">interval</span><span class="o">=</span><span class="mi">10</span><span class="p">,</span> <span class="n">blit</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span> <span class="n">init_func</span><span class="o">=</span><span class="n">init</span><span class="p">)</span>
    <span class="n">writergif</span> <span class="o">=</span> <span class="n">animation</span><span class="o">.</span><span class="n">PillowWriter</span><span class="p">(</span><span class="n">fps</span><span class="o">=</span><span class="n">fps</span><span class="p">)</span>
    <span class="n">ani</span><span class="o">.</span><span class="n">save</span><span class="p">(</span><span class="s1">&#39;sim.gif&#39;</span><span class="p">,</span><span class="n">writer</span><span class="o">=</span><span class="n">writergif</span><span class="p">)</span>

    <span class="c1"># plt.show()</span>
    <span class="n">m_elo</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">box</span><span class="o">.</span><span class="n">m_average_elo</span><span class="p">[</span><span class="mi">0</span><span class="p">])</span>
    <span class="n">m_elo</span><span class="p">[</span><span class="mi">1</span><span class="p">]</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">box</span><span class="o">.</span><span class="n">m_average_elo</span><span class="p">[</span><span class="mi">1</span><span class="p">])</span>
    <span class="n">m_elo</span><span class="p">[</span><span class="mi">2</span><span class="p">]</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">box</span><span class="o">.</span><span class="n">m_average_elo</span><span class="p">[</span><span class="mi">2</span><span class="p">])</span>
    <span class="n">f_elo</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">box</span><span class="o">.</span><span class="n">f_average_elo</span><span class="p">)</span>
    <span class="n">m_likes</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">box</span><span class="o">.</span><span class="n">m_average_likes</span><span class="p">[</span><span class="mi">0</span><span class="p">])</span>
    <span class="n">m_likes</span><span class="p">[</span><span class="mi">1</span><span class="p">]</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">box</span><span class="o">.</span><span class="n">m_average_likes</span><span class="p">[</span><span class="mi">1</span><span class="p">])</span>
    <span class="n">m_likes</span><span class="p">[</span><span class="mi">2</span><span class="p">]</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">box</span><span class="o">.</span><span class="n">m_average_likes</span><span class="p">[</span><span class="mi">2</span><span class="p">])</span>
    <span class="n">f_likes</span><span class="o">.</span><span class="n">append</span><span class="p">(</span><span class="n">box</span><span class="o">.</span><span class="n">f_average_likes</span><span class="p">)</span>
</pre></div>

    </div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area">

    <div class="prompt"></div>




<div class="output_png output_subarea ">
<img src="data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAAV4AAAFDCAYAAAByY2ZfAAAAOXRFWHRTb2Z0d2FyZQBNYXRwbG90bGliIHZlcnNpb24zLjMuMywgaHR0cHM6Ly9tYXRwbG90bGliLm9yZy/Il7ecAAAACXBIWXMAAAsTAAALEwEAmpwYAACY+klEQVR4nO29e3wcdb3///zszqZN08smNKVNmrTdXlIakHKxKqgHpbRYjaASKd44xVO0wjkgHo56+lNAvz2KHBDOAVGqIOKlEDyg0R5awAscUO7XtE0v2yZp0pKk6faStM3O7uf3x+zMzszO7M5usultXo9HH02ys7Of+ezM6/P+vN+v9/stpJT48OHDh4+RQ+BoD8CHDx8+Tjb4xOvDhw8fIwyfeH348OFjhOETrw8fPnyMMHzi9eHDh48Rhk+8Pnz48DHCGBbiFULcL4ToFkK8bfpbhRDiSSHEltT/5S7vvTJ1zBYhxJXDMR4fPnz4OJYxXBbvz4GLbX/7BvC0lHI28HTqdwuEEBXATcB7gAXATW4E7cOHDx8nCoaFeKWUzwB9tj9fAjyY+vlB4FKHty4GnpRS9kkp9wJPkkngPnz48HFCoZg+3lOllLtSP+8GTnU4phroMP2+M/U3Hz58+DhhoYzEh0gppRBiSLnJQoirgasBysrKzpk7d+6wjM2HDx8+8sErr7zSK6WsHMo5ikm87wghpkgpdwkhpgDdDsd0AheYfp8K/MXpZFLK+4D7AM4991z58ssvD+9offjw4cMDhBBtQz1HMV0Nvwd0lcKVwO8cjlkHLBJClKeCaotSf/Phw4ePExbDJSf7DfA3oE4IsVMI8UXg+8BFQogtwMLU7wghzhVC/BRAStkHfBd4KfXvO6m/+fDhw8cJC3E8loX0XQ0+fPg4WhBCvCKlPHco5/Az13z48OFjhOETrw8fPnyMMHzi9eHDh48Rhk+8Pnz48DHC8InXhw8fPkYYPvH68OHDxwjDJ14fPnz4GGH4xOvDhw8fIwyfeH348OFjhOETrw8fPnyMMHzi9eHDh48Rhk+8Pnz48DHC8InXhw8fPkYYPvH68OHDxwjDJ14fPnz4GGH4xOvDhw8fIwyfeH348OFjhOETrw8fPnyMMHzi9eHDh48Rhk+8Pnz48DHC8InXhw8fPkYYPvH68OHDxwjDJ14fPnz4GGH4xOvDhw8fIwyfeH348OFjhOETrw8fPnyMMHzi9eHDh48RRlGJVwhRJ4R43fRvvxDietsxFwgh9pmO+XYxx+TDhw8fRxtKMU8upWwF5gMIIYJAJ/CYw6HPSik/Vsyx+PDhw8exgpF0NVwIbJNSto3gZ/rw4cPHMYeRJN6lwG9cXnufEOINIcT/CiHqR3BMPnz48DHiGBHiFUKUAB8HmhxefhWYJqU8E/hv4HGXc1wthHhZCPFyT09P0cbqw4cPH8XGSFm8HwFelVK+Y39BSrlfSnkw9fNaICSEmOhw3H1SynOllOdWVlYWf8Q+fPjwUSSMFPFegYubQQgxWQghUj8vSI1pzwiNy4cPHz5GHEVVNQAIIcqAi4Avmf72ZQAp5Y+By4AVQggVOAQslVLKYo/Lhw8fPo4Wik68Usp+4BTb335s+vlu4O5ij8OHDx8+jhX4mWs+fPjwMcIousV7MiPluvbhw4cHnEweRt/iPcZRXj2D65teZ9WLA1zf9Drl1TOO9pB8DDNGj6thweVPcsGXtrHg8icZPa4m45gZwNtAPPW/17ug0PcNJ/x7OBPieFxlzj33XPnyyy8f7WHkhG7xSimJHZE0RVX6DkPFaGiMKIRH5baIV2+M03cYJCDQ3rv8tFBxB14MRKPQ0ACtrVBXB83NEInkeumYQVevysp7u+l4R6XmVIVVKyZRNXF4NozLvttF+24VKUEIqJ2s8MC3qqwH1dfDpk2QTEIgAHPnQktL7vF2HaFm7zZWrb2Kqv7OnO8rBnLdw+bn5HiAEOIVKeW5QzmHb/GOENZsVdmTuvn2HNZ+jx2RrN4Y59bX4qzeGCd2JPPG029Y0P7vOzySox5GNDRoxJFIaP83NHh5adjQ1auy7LtdLLy2nWXf7aKrV83r/Svv7aZ9t0oyCe27NVIbLnS8o5EugJTa7xlobdVIF7T/W1u9jVcEaQ/PZOWS+4lNmcbqW36d9X7LhmhU439F0f6PRr2974S5h4cRPvGOEGKDmb/rFrB+MzZFMx+4itGalQBpa8Hx/B5IPB8Mhagcx5KFOPLklIIwVOK0k2PbLtUyN8Z8XdPGsiufpat8hmd2qjlVQQ8HCKH9noG6Os3SBe3/ujrv4w0E6QhHaLrzMfqm1xmL//fXq3mRaKELpNd7+GSCT7xHEV4sgcaIYty4uovCCV5IPB8Mhagcx5KFOOrqYMwElQWXd3HBl9o577P5W6SQffHxZFVmgZkcdZjnxpgvKWgvncrKxasz2Mk+vvYDSVZvjDP3Y5V88PJKyiYEqZ2suTEy0NysuQmCQWIfuJDVv34p6yJrIfNkgppYlL7pc5DBoHHM+Cn5kajTAullgfZ6D59M8Il3hDB4UDV8WFJKBg+qjpaA/eEEzR/29bNCLD8t5OoXHu7tXKFE1dWr0jsgM8fS3Ew0spB63kZJHqF+8DXDympuhnMu6aY0rCICEBqrkVm+W9tsi48XqzIbiaxaMYnayYqxduiQEnZ0qezozLQw7ea7fXxrtiWM30ePU/j40nIeWHMRVZNHZ15wJKL5ZlWVpnv/SF8ylHWRNY+3tnoUq+6+gIoyxbjfkgno2ZH62eMuw2nt9LJAh0cJT/fwyQSfeEcIL63toz+mkkxK+mMqL63tc7QEzA/nnsNw1wuHrUTgwkbDvZ3ztP11wMp7u+nfp10ngExKbSyRCA0l69gUqCeBwqZoiWFlRSJQMk41Hmqd6B23tlnYONviYyEiF6syG4lUTdQCXk/dXcu0Kem5kUk4tE9BJjGIV7cw7Za9fXyJpG28ceFpL28/z57DZFi95vE+8K0qqiYqlvtt/y546AbtO83ludAXpCkXtHP+57ooC6vMnastmEPdSZys8G3+EcLEMYK//bbXErnWLQEzzA8VQKgsaCGCB9Y0pKPb+sPZ0mIh7eHYzq1aMSkjiu8FHe+o7P+/fZy95BSklCQlLJ6qbW+z+XJrTlUskf2aUxX+kjp+9DiVdy3pZkxYZdktnazq7KfKTE6pKH3FaDKi5zp0Iso1di8kYp6bA30KIiAhoI1bSgiRYNW65RjslIJ5fMmE9i8Q1P4lE1C5Y7MnZ3fFaI1szWiKqsa95KagMd9v0QnQPA5iwbSSxA36giSlthtpvKHbmEun781HbvgW7wjBzeKyuxYmlKQt12RSMrBPe/gNIjCxVzQ5jdkbHkMIKB8t+MHHQzROyNzOFRJ4c7KYDGSxOmtOVTjt/RMQQpMJBQSs25kAsseHnOZHP/5dS9JuiPbSqdx48YO8p7qVrz58mP/4+Wv86A3tmgrxJZrdC0HT05CNRMxzc/CtKkrHJ4zrEgISSglVe7drC4JJF2ceX88O+NlXgvTsgKSq/d549405A2jRKPx0hYJdeWW27r34+0ePV1mwtIsLvtzOgqVdjB7vbqlmW5C87CR8ZMLX8RYRXvSJdo1juER75noHJP37VF5bt5dDBzTimjZF4YE1FxkWbz1vs4F5pKka5s3LlGkOuxY4i6a0q1flwbYkIpAekwC+flbIs17XbLHt3QlvPtPN4f6E8bpMSuYvrKJyuslaLCvsmuwaWiWouQC8anWjUfjHW7oIlGquElcdrg2OU9ice4L09/3Lw3Hj+s3fabb5z3bd2cZ89e27mXTWeMZMUBjYp9L92n7u+9rkrNeXD3wdr48Rh91fFxvUHqCnH9jN84/2GqQLmnVhjm63UoeZdMF5dzrsOsosPoOqiQoTxwhHf7MpPmQ3Bi0wW2zlU+E9DRUmf7NkIBaicppGOqD9X+g12a25RBJnK98FkQisuX0SM6rzs/pMX2PaI+FhgvSpf/B6RbOWE1br3tXHnuO6zVasfUNz+odOoWyCQiAgKJugcFbdwfzFvD4s8In3KMMxKBaNUnOgDZHUSFcIybQpikYEpoezbl4mMTgFSYZdR5lDU5pty+9FqWBfKEJjFOIHFQICaieHOLRlEj1tGulAmnwKQaFBRDOyumVc4HUR0qHPWyJ1zXs7Bf91eYhfXam5lvo6BfX1sKNT2yUNpMi3f5/q6HLJdt16UDM0RmXsGV0clNKwoEVAsP/U6uJmu5wE8Il3pODCOI4k1dDAqt99ntrYNgJJldqD7Y5WVHMzzJqV/n3WLOcgSWNEYbyiWT8H9sZ5ae2evHSyGTKrh5zMtTSyyYfsSoVLGzMlXHt3Wkm1Zwc898sqdv1FI7bHmxSevztt8YVDhQcTC/FRDjULrhDo82aGeer11wdiCv37Ejz/aC9P37+bzudijvItp+vWr2vSB9o5t7GLMz/2DqVh1SBxAJFIUNG2WTtJsbJdTgL4Pt4iwuK7yifXXlHSpg1oBKcO7eHOx6c3nO+1w35pCy7vYuwp1nP/4adT+NztKpXToKdN21bv7RTDMQ2eEI1Cw+JBWrcGqKOV5lk3EFl3r2GWFjofQ6lJkeuW0F83K0AShxRe/f0kplUpnj7LfF3JJKkAKZSOC3LW4nLGTFDYv32Qn10/ikmdm2kWlzD6rGmsvPShIdWw8H28PoqHfPJiHbbyXpUJbtbYUPSWw6nVtF/amPLMc08aq22jVy4IcWdjiL2dwkuWrIFCawroaGiATVuDmt6YuZy29XcoM2uNcznOh4cPHUpNilwZw/rrhw8ovPzwqTz/k0k894tT6Y8p1s/KMk7zdRma6iQcOpDgb4+8wxO3dXJbYym9nSE2MZeG0BOsXHJ/0WpYnMjwiXekkE+uvUPkxWtKsFsSQCG+TJ3sL1w2mfMum0jpuOCQtZr2S6uamDmu5maon59OIV5weRf189WsWlMz8iU4Oxe1tkISLXKXJMggozQSTp3LcS49fOhQalI4BuNsr2sWrSRJgEFGpa/B/FlZxmm/rqmTFKbrQcPKAK+unWKZl9bELDr2Ck+L8tFwzxzL8Il3pJDryTHDIfLipExwMl7crNN8fJldvSpX376be96K03tIC6yUTVA4a3H5kLWa9ku77brMcUUicM6l3Yw9RdPujj1F5ZxLuz1vy3MRnH33cMVV0sJFwSAE0Pf1uggvfS5jLoWk9mAbq+44HzZsyMmqeda5yTpvo8dbiWz0eJWSEgiQJB1KlZmflWVy7PfIrf88KR00/O40ptWMzhh/rgVdJ9zPfbuLtl2+ZazD9/EWEYX6rpxqv/6xR2Zoce+8LJThNl6wdOj+2GXf7aL6/DBlYcXSRcNJD+oFhdQiXnhtu8EPoF3fU3fXejqn7k6fMEVy5Z0qldM1na9+jF3XvHsb/PgqYfhGB2IKhzaE2fBWCUFU4oSQBLU5jgzSUnKWRli6o9U8UH2wDj784aw77ORnfuiWKosfGCRBEtTNM/l484g12O/DL390Eld9XrGMf/R4hzrF+9sNy3rZp9fTPiGC1LV/pinSv0/fx+vjmICTu8BJ/eBkvAxHJlHHOypjJlhJFwqXbBVSOS2XJZXtnPrmQiddXeerH2PfPVROhzM/1s2Ycs3CHlOucuYnYqhSYeO20Zw2L5jeqGDaqg8OQjJJlBla8R/i1PM2L9QvZdkn12Zsq3Wrtbdfcv2jcZr2pf31+fqlnXY2mkWdsnJJMK9kG+q2dqtcLY+dl/k+bNul8u2fd/HkX1WLBO7wfoUX11Txlx/X8uKaKg7vN7ldkkk6JszIIF0/tdgn3mMSGQ9V1xHCZSGWXzafr0/oMCRaTlvXbJpSr362mlMVi4RISklAFC7ZKiSBI9cC4lQoRicxneAmz0wnWUigZ0Cy7LtdjFesuuZwCEonqBai7+yxkqVBNtufzrBwG2hmE3M1P3CgnhvP/gFte4RBWP/23+9YjndaNPL1SzstTBqnauqPufOCNG+clWlSexAQ64uAueIaQFwlw0XgOG6TRVATixp6dP1kfmqxT7xFxwzIO8SeUUt17zbHJzIftzFoD01Pv+S9n5zI7CUTWb3BWR2xasUkul/bz8A+FZmUhEOCq0/z1qrICU4JHG4Wnu5/fahDct5llTx6e41jUoL5nDrslq/5GL3uRftuldfW77HsHj4zN7PWro6Mcc64ML3aCQElJbRSZwlkBUst+326eqy/Oy1E+QbezAvT5AqFVx6fxJw52mubN3tLynCDWRNs3/3bg2eO4zZZBKvWXmXo0acNtPPL71R5TjI5keETb5HRDJ5NGd0ibd+togTRMrViWr8sIOOJzDf7qeMdlfmLND1mICAIlQUdt/1VExXu+9pk/t+Hx/DNc0pYccbQaqg6uUncLLwMa3DToayJJ+ZabhLo6ZcoCsyeDff+k8LubWnSfW3dXqSE6PbBjASPqkrrdlj/PWOcmFa7006DjRupm6dYdh654LQQ5Rt403c2j95eQ82CSpb+RPLPa+K8c0Dmn0yWWl26ymew7MpnjQSK1mcqkIl0uUuZhAO9imWhdBy3bhEEAlQdeYcHHr2Yp55t4IGbqk96wtXhE2+RUQeeTRlz+T01ATWTFR546zqtSSG4P5Emsyx2wSJWvzHgqPetOVUxSFc7nRiR/ldOmWxuFl6GNehSo1Y/5yk7o4hURCmZkPTsECQSsHUrvPa84M7GEL+7rZfnHtHqXrj5F3/wz6cybYpGoNNOkfzgD18ARaF1g2od5/aSjNXOvvM4tdx6/upK6+9OC1G+uxf9O29qfpPxUzSXSuV0+Pwdav7JZKnVZeXi1bSXTkUEoDSsUvfBPl56pIrEgGb5DsQU3lw7ybJQZq05kUjAkSPeLYOTCL6qoYgQQvA2UB8IeIoiZ0TyZYKnVs/W7up4HEIh7Wa2h8RNkerVTa9rfbWCwYxKZF29Kqs3xAmVBQ3yPWX00ela7BZcX70xbtSaTSZg/44jXN34LiJs1/4YDNK1+7ARSY/E2zlrcTn7ayLsblOMLDcz9GyucRM9ZleZBlfP22xiruFKKCmBjRuzc4iuBugdkJz7kQpGj1Py6iztCfX1RDceYc0LGwgo6XMmE/CrK0P5NRJOpb0t/NI2koH0vMgkdD9bS3MzzJljy5xDRZ135rC0hPZVDT6GHQ3g2ZRx9e2qqka6qurssjCZj33T0n217IGsqokK171nNJWp6mGnjB5awfShiOLdLLzGiML+3dr2VgRAVUZxRfUT2ospi98cbd8mqnnxkV18fcEY1jduZl9nMuOzBvsVDr6VvYiN5VrOuIuusmptnDSgEDeOi8dzB750N8DHvzCJ0eOUYeuDZ0FrKw3yd+zpwAiCJpOS/bszb7GcWY8pf4E5ECYETK9WDEPV4lIgQR2tsGkT0cUrhpQleLKi6MQrhNghhHhLCPG6ECLDTBUa/ksIsVUI8aYQ4uxij2kksR3cHbG2yM2qjx5OR/Ltvt2UdMn43byfND0VFW2bja23vRJZNArnny1YcUaIX3wuxIWjhua79Rqsc0IkotWfVevqebJrBt+95VkWXtPGV3+wiyOHNWtLCKiYCufdOcPC0BkddMtnQjBI86wbmDsrQTCoFQyaNSu/wKMh4Uu1QweIBNpImBq1SOk946yobc3r6miljlfXWVtK7X5rDw0NViLMKedLrYKr1i2n9tBOLTHEpjwwFkpU5rJJk9UlkzRsvaPgNOiTGSPl6f6QlLLX5bWPALNT/94D3Jv6/8SHSe/Ipk1Ufb6BVX99Q9tGJ7SHf9XaqzQfr6Kkxfp2X29zs6HMb7z7Rpruepy+ZDCjJKPt48xdcwpCxzsq7/3kxIxgnWfXhe5bbFxHe+lUpBS071aZvUSm/dAp36W5IkzNqdbkgZopo0BViQCFXo4bmVNXR91gkk1R56l3RTRKxc5B+qZMT7l9JBWjh+5mMJIaLljLee/aCSLA336bfrSkzPyOv/DLHAtAyidbBTzgci2RhgZaWluhJEhs0lSafvgYTdPnsGiHwq7rJXs7Nflc6wYV6ofHBXEi41hwNVwC/EJq+DsQFkJMOdqDKip0S9chzfTGu7rZ0amSFEF2hGdz45JfaqbGunXuLguTvCH8l/UsP3OMY0nGodQKcLqEwQNDDNa1ttJVVk1b+WxDZC8lmobYVBYyHEp/Zn09NN0xyVSfd3g0oRm62KpRxi6leV1JfoEvgIYGGq/5GBU7WhEJlYqd0WFpa25uIx+q0B5f/TsVAg7tC3Juo1bj4tzGLtq69G7WprKOO7fl5xMwSztUlaY7H0vFERQqp2vZgWB1Qfimb3aMhMUrgfVCCAn8REp5n+31aqDD9PvO1N92jcDYjg6ciqumTKmuXi17CrSi013l09Nmqck87epVWfndrrzK8dXVWQNabpabU8qy/dwNDbCjcxLv/1ycsRXpYF1e2W11daw8466MP3e/tp93LzmFvsPpVF+iURpOS7JpcAZJFJ775RTmzhU8NQSL3Zx2vODSSkLr9xDdPpjR3FNf1/JCayvhRILljfO133PVtPSYT2xPrgkGNfWL/l1t64fAaNVQJpz98W4aI1NoWt9K35RpVOzYTOMNn4Jxo7xflG3F7ps224gjBIKCyumaC6KOVsMFwYYN2jXp1zCc+dInAIquahBCVEspO4UQk4AngX+WUj5jev0PwPellP+X+v1p4OtSypdt57kauBqgtrb2nLa2tqKOezjgGq21F1cFrVlaczPv+ffRlIa1/l3JJByKKbywJrPWQiE1Yb3e+17OrV9CebVzPQRPnxmNsvA2QVJYNbS//I5DAKy+HmXDGxZ/61Dq80ajcF9L3JBigbPCw8si5Ih86i/ncXyu72bhNe0kTbdbQMBT99QOrcazbWyrH2+hb+pMo9bFeAVe/M+/01FazeT9HQhg1/gaag51sur292nzleX6fFVDESCl7Ez93w08BiywHdIJ1Jh+n5r6m/0890kpz5VSnltZWVms4Y4M7KpzvUNlJMLGpyZxKKZodVBjChufct5GF1Ij12vChf3cbbvUDNWCfgn2FjT2YF3WVNhIhJqqUZYtvtHiyI7WVupoNaqGjRl3hPM+W3iZwYYGLKQLzsGvmx/spfr8MB9eNpnq88Pc/KBbqMKGfIW5Hv1AuVKpaybbXCaTU3Npv+dmzHBMTHFUqtiupfG0UktHkyd+0017WS3JgELXhOl0TphOMqDQXjo1nWI8nH6uEwBFJV4hRJkQYpz+M7AIeNt22O+BL6TUDe8F9kkpT1w3A2R9KAdiCi8+XMVfflLLiw9XMRBztq6Go1eYGWbJ0Qc+XcmY8VYr1F7KzyuvZHveYkckCy6tZOFVWr3fmZESd39tXR3N4hLmsokgKud8dBehsYWXGWxtxWgdBO592/TuuoGAYMwEhUlnjff2AfmmFQ6lZqQJrsRs/8LAcUU0qzu2d6os/Vo3UazXEp41jRcf7+Gp+7WGrAdiCSSmm1G3YAPBtEEwTNd3oqDYPt5TgcdSWwkF+LWU8gkhxJcBpJQ/BtYCS4CtwACwrMhjOvrI4jTM5Yc1tr6ptGI1MTwBpqZNh+iLB5DBIKPGCN79kXL++rA1Wm62qr36PbNdz282q8QGTfV+F53ivo1vbk5F1s+EujoWVqw1ttSFdMWoq4OHblD4/B3pFkO/u1vhwvutHFk2QTEaPepddqmvh+ZmusbXFuaGcLk+GhqIHTxC091/oG9qhPFvxXlxbS9tbZqOuLpSQSLZ1ZtAyvSCY3Y16BriDNi/MEVxXBHtXShEqeqofjEfp0FzPGjuAqHxLyaDwKS8MXxOJzGKSrxSyihwpsPff2z6WQLXFHMcxxNy3Z/mtGKZIt1vfbaKi/7BwY/q4GCNVc9wrGPbFxdGwIRgkNFlWmdji2yrAKva6Xr0oFYsbu1eGxvM4uOzEUeNzdeZ79i0cWkpxToCgUyJXbhEGIuDTCYJt201LMSVS580xuBEgl6QDvDVUPHo6ySSsG9Qo7HYoKT63RNoa9MWwM7uVCKH4ROFjt35O7m7elVWfvbPdJRWE5FdnLW4gv21M6jYGCcyo4TNWwYtMQYnr0DNqel7AyCUjDNIiEP7FUBQOl5FPWQyCAqKUJ64OBbkZD5MyLVDdfLtuvpRHV5wE9NX7DAlXiQSVOzYPCy1fZ2uRx+DEMIIqOityO1+R7esq6GOTR9X0ORRcXI9XjFHYeIYgUioTNy+iSv+pcE4cDh60dm/j9hgWnMrUu4NA0IThZkN1cGD+S+GK+/qpL10KsmAwqRPn01s2kxkUKHvMJy16BStNkOKdN9cO4kZMzLPYZ7/aVMUHnj4Il769anIpEa6AzGFlx7TjrFntNm/0/Jqhw84weGXCjrOYLY0dEvvL25+VAcHq1s2VePdN9J07W30TZtDRdtmGu++kfBl6x0tuEI6SphhHoNOvgP7VLofeztD/d/06OsZC8Xy00LuW+o8kcu1oxfjoX5+xoFO30W+sH8foG3RJVrwamCficyl5PCBIKPGJBk9Xuv8WzZBYfXGeMZ3kO076uhNGrrpMeG0K0UC+1XY/bcqtm41DfLUzHFnzP+aMZx9xi4C4aAhZXvXkm5efLgqI1nH7GLqHZD8438188NPnZ733B3P8C3e4wxOll5GHn2iha5zLmTZZ/7Ewi9tY9nlT9I1YRrU1TmWJAQI3/9jlt/0Gb7+vnEsv+kzhO//sdPHE43C99er9PSnC5DnW4PAPAaZSnXtfC7Gzb+8POdCYS54PhzwLD5wOHA4dgT276O8JP23cImg86V92otSUr1vB6FkHAJw9sXllIUVAkHhmAbcFFXZczhdAP6uFw4byo9gQgUpKR0XRCatMq6K0bB9u3WM9t/d5qckbOsgHdY+LyOoOmh1MU2cNtvDB5xY8In3GIKX9i9OHSac8uhXzv4m7WNqNFlPeCYrL3kImpsdSxICnqPwXmVY2a7HPIaJYwT/en4pq1ZMYuXHf5F1oTB/nk40Xtveu43NsXi408Ad5idbtw+vsH8fl89S+GilYNMfevjtT3bBoOSX36niTzcmeOiNr1AyPkVqpoxBpzRg8+96Oreu/FCDCgjBWYvLEYG0jlbvMlKQACESoaYyYBTZkUlpKHKMc6TmVa8tAalaybGTr+OwT7zHEPJp/2LmhoYGzSBTg6Np4XQibKcjnG4wKANBdoyZRpSIY21cJ7hVHnOSYe3d6bxIuF2P0xhW3ttN+9ha14XCDDPRFNLPLedcL16sZV4lErBhA7HPf9Eg93vfinP17bvd9cN5Nk9znQtbzz2d+GuqNd2zuTWTvRgSqd8t5LZPNXzQtRM1gjSTN2hryvlnC+65J8/awCmYu01Uxdo49NSA9RypSe9+5FUGUuQ7sE/luUde9fYBJxD8erxFRL4ZOfkkFzkmApH+47LLn2RHeDYiIIzodGBvJRevVAmVBYn3J1g6R6FusnNBG7cMqfp6eOeAtMiwHrpB4dRxIiNonc/1ZO0qHI2yuiWz4Mzy00Lc+loc8+x67YRsH1vZuMM0fuIlOsbWUrNni1ac6ICWyb666XX6Zs4z/K79+1Sef7TXmjmmK0g2bLBeRK6MNae5uKaNpEwTYkBInrpnGuC91m/siOZeCJUFGdin8vr6vVSWCR74VpVxjurzw4ZcLpnQFtT/ujzEuR+Q/NO9Bfjwc33hqde7xtWwcsn9dIQj1FSPZs1t7+XwgY6TKnPND64dQ/BaSwFcEhM2p7Vbq7Z8j0/MfogxYdWITn/1t+ki6KGyIGs2q9zkQrxuEXsnGRZALGg/Q37XkzVQ1dBA44EjNN3xW/qmz+FwbJDfP32QZ0oEMz9cTsnY/GtFWMZGgrOX7EpXSEuVhXzg4YuAVI3j1PvMSgOLksGp/kaBGVo1B9u1sQSCiGSCwX0CRdHleNmDijr/t3UlOPuSPpQxGhFWV6Z90LqLRA/A9fRrpPvg9QrJJJx3bXoXsecwfP9JlT//socx5SpVExVuu85Fr5zrCw8GIZGg6kCHNrclJXDkCD//dkfmuU5w+K6Gowj7rvSelZ3MVbZqvtrgFpr7P0xs2ixWN2/i1tcGLT5MxwzQhghKawv1dSqHm57m4FtVPLNay4Ab7FcsxWx08nWDW2ac7uqcNy+3HzCfrNmsgarWVsId21jeOJ9N//kczzzaR/++BJ3dcV5au8fYdh85oHqrABaN0jy4mLnJFsMvXhLG4prpCEeMtu272xTDtWJWGlgWCPNKqKPADK1Vv/+CsWWPx+CVP07xXO/20kaVsWd08e6lXUbTTSG0e8xOlrqb41dXhvivy7WF9PqmOJMiWHYR46dISsNaF+aunixZgrm+cPt2p9BCGycAfFdDESGEYPrZH2DFz54mKbXgxdKZQWrHaYyV4S5QttKi1lkeYLdWPi+8qnLjXd0ES1UShxS6X5vElhbF4nqwJy80/uiQYR0mk5J4f4KbPljqOPZcxWHsuRn3P6Ty4z8OUxaXHaaJsrenMcPinvB4Ph3LLn+S9vBMw8qs3RflxTWT2cRcJlQHjEJA5aPgNVsVs4wiMDpShY+8VuEy5nRDutLXHDbnVRjoPUu7jCJLlrnRi+Vk+dxFt8SpnG4NnCYTMLAvzvOmmr+BANx3Q61j8aO0jE1qpTCv/RjhsaPSN6NDoZyTsUiOT7xFhBCC7/59P0pJev8bEPBv8zXrIsMlhoqKdQt/64sDSCX94Ok+TLsP9uAercaDcS6HB7R1d5w1m735ePNFIdXSPMPE8ssue8IgSMMXIoSnzzQWk87D1MSiFj9u17gabr7i10z69NmUhRXC7Vv59vWn0due9m1mI72uV6OsvKuTjtJqrSrXddVUnZ1f2UPLQkyCuWyCklFsUmeSTApPLuMPrWjPaFWfTELykMIzD1rnxq71NUv3jGN2wgt/2IMUg5RNCHLWIk3Gtq9L8NNrFPZ0aOOqn69yzqVWv7GWiNPK8svPdrYEUmx9MhKv72ooMoKhUZbfzSX7MmQ7JTsy+oO7tfKx+2DHlKs5t/51k0Pc9MFS/v2cEm76YOmwka7TeArJ4nKFScq1asv3jG149b4dVB3q8qyjNdQCunJiyf1GdbiqmnG8+6JxjJsQQAQE+2sifPHuzDk1u4dmz9b+KQosvWs07WOnaeceO42Vf/TobDbB4rcnyAbquWfdLObOFZ4VBlUTtawz0L4HKbXA6qu/z5wbuyJEr68AGD35rq4PsefliRyKKQbpioBg/BStozFoYy6drc3tGFNtCxkM0jdtTtrXnW/hoBMYfnCtyEjEj2RYvLql8YVfalKsn12rMKkkTnP8amhLPTXTpkEoROPXPmUUTakYLQwfpj0YNeUUhblzj14NEs9ZXDYfRddDzaz842jPLoqqptU8kGE1eXAv4NDeJxyxsFlf35R0o9BgkPKpZMypebdszu4Klhaw8Njmom7Ga2zYWmI55Jpr8hNF3HbdJFbe282OLpWBvVpQdbBfMQqSmWFPTpFSI1urmgHefEUBqiwKEqMlEyldcblqdA/RZWoikaCibbNfjcwBvsVbZPzsKx9Fl0rqPl6zpVE+Ff7jCZWWkrOIdPw1dWAAyspgyxbCbVtZ3jCXr59VYtHd2oNRt103iSf/qvL5m7qY8qF2vvur/GvUuiEahfrZgyhCpV60EJ3+4bSpl9Kqes7isgloV97VmalZzYYhWE0ZAcPq0elzRCJUlCkWi2+8AguWdnHBl9tZsLSL0eNVxxgaaOU8zS14PKUP2+aimczImS6K8NrRWVcs/OzGWg6+VUV8QHG1lPWauqD9H8BOulafhT2ZZf+udBytaqI2t6+t28vAPhWZlFTs2kHj1z6Vnxj4JIHv4y0i3HxXjtrTd5d6E71maelQLD9rfT1s2pAgSdDwPTbTQAPNtFJHXckOmjfO8saBNse2PVjmJUBWaFeIXO+z+zxfWruHbdFBy3y+uKYqI4YGMHlOnGV3q4ytCDJ4MMEVdR7854pC15iqtKY1FuWVLRfQ8rpijz8V5bu9+vbdRr1hmQr+alXYNK1y53MxyxxlixF4+k6iUS05Rd8qzJoF69YhZs4EfB+vjyLDsV6C1zzNLClXHbvj1u3u7viwjLe1VfM5gvZ/K3U00Mwm5pJAYdPgDO+9DW3XWXOoM++C7o6ZXR5gpPjeoPLAmouomjzakl1mzyKLbh/McB+YFVN6C3mAz/4Axp2ibbFHjVP4yx5vc7Fyyf20h2cafuczlnQbC1gyCYOD2vCK4UOPbh/k+Ud7eepnuzX/rql+QllYyei48f3VPTzzcA9P/Ww3zzzcw/dX9xiveUqfbmiw+me2bj1pm2L6xHsUYM7PP3xA5fe/6GbZJ9fSNf8CooFZ1CutKK1vO2ecZmnpcOqBXZat46kHhqeRR92MQaPljt5JtpU6Kxl7zROwaT1XXVedd6GZIZOQx9xsJy2z2dOxZYv2LxiEU2qwHLt30MM4mpvpKJ9p0Q+/s1elpCS9NukbnOHoOGJ3V0w5JX1O3T0AmuUpRGbHjd4Byfs+NZGFX5zM+z41kd6BPC1Up5vkJG0B5BPvUYBuWW36g2ZB9O9L0N4nWHnpQzTM3cImdRaJhHDmhCyW8VuPj2cgFkImYSAW4q3HPbapcUMqhN+8da7Rcmcum2hWPkldaHuajAPSe+zExFzR5hYu+nyEh26pYtefa/nWZ70VmhkyCRXY3+wbyysdC/K4Xfv3X4vzHy8Pctn/2+Xsl41EqJmYLiwjkglqyqXj8IajEpp9pyCRxjm7X9vPkYMJg3TB1HEjhXM/UmFpg3TuRyqyfp6F6L/VRld4euZBJ2nQzffxFhG59IlO9Qn+8uPa7K7eLD5eRahWsT0qqhyCcMUpKSA1qOhmdcjduvNtxKuj4M6/pg+OmVKQK3a10bioLmc9gtUb40ZQVK9tsP6mEPfcA+sH4oybTIaGVkpJMgl/+mkntYd28sBN1ZaJ6jrnQlbO/qbh41215XtcdPjpnPNSSE1k+/0mJfzsxlpjOAuvbee9n5xokGsyKSkvEaw4Q/Pj5lsXw+KXTiaojW0z0rCBk9rH68vJjiKcJFg56xtk69c2K8mmrekgWN0sh/B7PsiSBjscnVwKbTw75CLozc00mYru9E2NGAXWs8EsvwoEoXKa9l1dcw0896piUavoEEIQCEhkIEjvpFpWtxyib1/cIMuqN/7KA6/+Kf2GYJDmzbnbkzlVZcs1/ppTFXZ0qghTWx9zgfKaUxVeX7+X+YvKGTNBId6f4IrT01JILclCIklJxXbtgAklriuuo3zPdJ1s2ZJ1vCcyfFfDUYTT9jHfruBmNK8rYe68oPbeeUGa15XkflM2mN0aOgqQBrlVSjxqjWcjEfqmzkxrdhHsOYyllq9TnV9zUDSZ0Cqz6QuGOTBnqrRoWLwimeDcRRM0ssdUwtJhErwo5tw6iWTDqhWTGIhZ2/qYF7tVKyZRWSb4+//0smVtL8vnWcuGNkYUKnZGEQmVih2tNF7zMVf/eOyI5AOfrmThF7UO0mPKoCYWtVznyQzf4j2KcLLcovsLP9+w9xN0SfHMF+akA3MbmKPZeLZitFZ5ywyz1ehkUTZGlIxqXk4csnRmkDXbEiQlyITktT/2UBvbxujy801kr1mPhU6COcXXqR6vE6omKhx8q4qXbW4M8+vZdhLhUYLlnzg9U/bogKaoyqhxGr2MmaDw7o9NZPkNy7Tj/S7DPvEeVTj4axsaIo4kdVQwTEzu5lIYroUiX39nV6/KS2v3MONDFYYfHqxWo5NFqVu10Sg0XAn7d2duALp6VW4y+58/eph/b9K+49WNr2olJoPB9Fb9rPzr9QLGImC+Zi+w8/z9D6ks+24e/nKPtT7tHTBGjw9R9crT+VziCQ0/uFZE5Cz+4RBdUlpbPBcPLwaG2sjSCYUG0czIFlAzB73MFdzcoAd93vepdCDJ/j77Occr8OLjPTkJKluiQ2zaLJpu/226oejXPqW1iz+KyDsxI0tw14x8vhO/SI6PkYWDKXjU/J4pFNpKJxuG4rfWkS1pIl9/px700dNbk0mZYTXae6G9tn6Pp6SNbBrj8NhRLL/8bL6+YAzLLz9bK5d4lJG3JtpjyrZrbz8fgE+8RxcOLDscJJUTWfqCFRK0yYXhKEqVjSDcOie7QdcBHzqQ4G+/TQWSbP3nvGSxZTs3OGiMR+TLzQ/DkZjhBKdecoU2Jj0R4RPv0YTDgzgilfOyZG7ZC6EIQe4HJM8Gj4XAlSCiURpXfJSKbRu0aHsgntO6KiQZwStBrVoxiZmREs67bCILr5rMgksr0/Nn+3Jj1TOGn4g8fBfmxAZVhSkTg0NKzPCKYuymjlf4Pt4i4pj1XWVpShg7Irlvo2qpG3xKDp/psDhxU3BzIbr5eO0JCF/e8ABXJX41VCFGBvJJ2vDq38zXN+0Jpu8iVjOTpnv+QN/UmRZ//VAK7nh08TrCLQHjmH1OXHBM+3iFEDVCiD8LITYIIVqEENc5HHOBEGKfEOL11L9vF2s8xxKG20D0WjLQQBZHcniUwH7/53Q35MqEsFcPnz49VXVbaL+bJsDNGHcrwrJy9jctRWZunPf/vJRhyBtOn+82717dNcVw65i/i6Y7fpupG2ZotS48lrlwRL4uoRMZxXQ1qMDXpJTzgPcC1wgh5jkc96yUcn7q33eKOJ5jBllvXhsrR//SnpOk867WlcPXmPcDkisiaL7grVuhrS39mq1CVb7ZbPYiM8Fw0PX9w+1jNM/7O/sld78W5z9ejltcNeDurikKEZm+i77pc2y6Ye2QfPy6diMh1/eTzQhojChMSOX0yNT7T1Y/b9GIV0q5S0r5aurnA8BGoLpYn3c8IePm3aCmGdXGyg2LB3NaGHlZMKa9YnTGhdQPvoYyJ2Ih9bwj0rmCRm7Vw82vp5CvqsNeZCYxEHR9f94+xmiU6OzF1IsWrQj87EHLwmee97M/Uq51cQ6CmrCeJimdP2vYI//RqFZHMjXXFV07ECmb2kzsbj5up52Y3UgIBp2/H51wP/ftLtp2ORsB4VGCYCC92MQGT14/74gE14QQ04GzgBccXn6fEOINIcT/CiHqR2I8Rxt1dWSUWTQY1cbKrYPTc1qAeUWmTU9Sw9Y72LQ1mEHqThHprMgVEXRKPba/nkK+gf9V11VTWz1KI5HqUdx2/amu7897a9/QoM2RXnd4a9Cy8JnnXdcDg7VLr/mz7TDP84WjQpx/tsjY2Xi10qNRqD8tibJ1I/W8TVTMpPGO66gYLTKI3c1t47QTa22FCVMk1zfF+e7f43zlV3HO/YDMmF/d+jfDyQgoinvlOETRg2tCiLHAX4FVUsr/sb02HkhKKQ8KIZYAd0kpZ7uc52rgaoDa2tpz2szb1WMUbkGDaBQaZrZo3RtSbbwjwXaNuGyBqnqllU3qrKxxK3Pg59RyhbfWTmLDG4pz8MMUWFOI59U6PANeIy3m42bMgHg87W5IVagiEilK8oYZqzfGjTThZFIyEFPZ/pcYt13nEihTFJTEYcscTayV/McT2hjHK5q+d8vWQd73yUrGlivozY/NVcq8BM7c4pNeA3BOXUJagmfm9YU6db2uo5VFTXOMtu/JBFSWZY7BXvkMnAN3Ttdz9TzN/+AH14YJQogQ8FvgV3bSBZBS7pdSHkz9vBYICSEmOp1LSnmflPJcKeW5lZWVxRx20RGJQMu8T6MGRtHC6UQCbWmrz2byNa8ryWkBmi2Y1/+nipbXFXfXhMn6rKPVVFO3gGQNr5EWe/XwHTvSLXC3bDHIuthyo8aIQmynRrr9MZXX1u+lqyeLT7yuzjpHJPji3ekx7lfh3QvH87OnlvP0sg56duhFxK2n8eJGcPOderUQnbqEEAzmFbm1uHlSO7FmGqicJg0rPhB0HoPZ+tfhJE/zEys0FFPVIICfARullHe4HDM5dRxCiAWp8XhpmnL8I0WwGR0niBB79W1Wv3WIW3/5Ok+fOoXnXpXOu3iHXuOtG9SMB9jiuxt8jWhkoVZ+cNYNzJ2VyLmtd93uFlrX0QVeSabQIFl4lOA/PxHiydW7+dtvezl0IIEIZPGJNzdrc6QXgZ+VoHyqbYxxQST6FC901vHDy0czsTOa0SLdi7vGzbe9d6dmZYL2/96d2d6vjcxwX6lqXrIDy5qf6qsXYTuVbRsNUziZlBw+oGYoZ8x+42lTFH75nSrHFkB9nYI7Lwux8t0h7rwsRF/n8O1ojicUzdUghHg/8CzwFqBvQv4dqAWQUv5YCHEtsAJNAXEIuEFK+Xyuc59IOl6nLeb1j3rUdzoUKq/nbTYxV9tymqpPDUVm67rdHUb9btbPSUF3RZiriuWrf62vh7FndFEaVgkEQCZherV3HWvGGLdtYHnj/PQYa2fS9MTGvN0lbl6bymmSz92uUjlNK0P5y68p9LRlns94/wY17b5ie+HFPmx64Lvuf4VQeSkD+1ReX7+XyjJRUE1kp1tmw4aTT8dbNDtfSvl/kKGssR9zN3B3scZwPMBJ4aAXm4YcAQgHtUAzDVxR/QTn3TmDyukQDsFNH1dIJkX6M/I0TF0t0WGq62j27QqheSCctqH6MWbkG6BpboZLGyfB7G7GlKtUVeaXrZVRFezuGzUGSTFJeOyogpIg3Cq1TRor+K/LQ45lHB3fX3+mp+phOWH6bsPjRvHsYzGScp/xcsdB6+Fe/fPDvEk6buGnDB9lOCkcKjq2edN3OqgFImznn+48xOTpCQJBOJCEL96tDqnwjllvKpOSg/tUbnnmELfuq2H1o68T648PKb/Z7NuVMnN7rrsW9pgWAB356F91q3DDG1pd2p/dWMuvvuutz5s+jgxyuf/HRa2/oG//AwHNVdTamiPpptB6EHb9eLtCPS0oqNTTwqkVoazKGa/++aNdBOpYgU+8IwWXdLXmZqyNJGmg8Ssf9RaAcOo1HgxmCOfLpw6NG/SAiExK+vepgCRUFhy2IFgu366TpasjnwDNULKuzOOwXHeRi2vop587V/uInGMvdDw59ONvrc3U/pqTJXoHpCf//DFYJ+io4OQMKR4NuLRhiESghdOtx3Z69Fm67E8rHHylQyk4rutNdcnQwi9ONjSrw6HFzNVNwd7HDCC2E352rcKksYILmyHsgV+Gus09mhrUom/RnfTjpD9vwxsKb75i9emaaz7071Mpm6AgTLWNnTDsXVKOU/gW70jBdmPHDh5JR+Z/t4FY9Yz0sbNmZbw9n/oOQ5HsZEv51CVDeg1bGJ5U11zjtafWxnbCbZeG6G0XbNgAM2d6q3kx1G2u+TrdovtusH9/b25NKzNueeYQH/tGJ4v/pZ2F1zjX23Abe951Otxg+4C6kh1Z5yp2RFJ9fpgLr9J6qm38v33071NPepmYV/jEO1Kw3dhNd/8hvW2tmUnTvWu1/de8eVpCgQ2awSy1rd+GBA2nbXVlmqFIdrLVfdAlQ288uZd4f2LYHrJcmXKNEYXxiubqOLA3zgt/2ENJmZVgNm1I0DCzJSsDD3Wb2xhROHJAW3QG9qm8tLbPVQNsJ9rFi61ujl9vTLstQmVB5i8qJ65q6cVO9Tbcxu6pToeXVTtP/XhTVLNwAwHBmAkKp71/Ap1/7uHrn5vP8jNKCZ99elHKg54o8JelEULXQ82svKuTjtJqag51Mrc6Ytq2Cvqmzswq+9EM5pQygSCtg9Oh4UzHfZvdq3Fpo8o5l+YuaRiNwo4u1Qii2FM+qyYqfOuzVVxxlSR2jkrlGIgPFjAZ2TLeHF4LRyK8+HiPsa1FwLuWdPPiw+mtr5E0kKVR3VC3ueFRgmcf6bEISezRfR3272DCFMl1TSoTp2kZc2PCiqFc0clLh1OqrdvYPdXpcOs2muUDImSfq77DIALp8ZdNUFi19qrcn+MD8C3eEcPKP46mfew0rXzh2GkcPpjwplxIWSt1iZbM+g4ujj67P7B0trfqZQ0NMLBXMd4rk5nR64YGOO9a1UghjcULCK5li3K5vGYmGBGAMeXWzzTmpMgaJa91MfTvYMKUw3zgi+185cFDTJwmNZINay3WZcpdo1vQOvLpBOFpPEVwENvdPxPHCKre+KuvFfMIn3hHCHbL5OU/9Lh2TbD47W7ppKuzn2YarOoHcYmrk9LuDxxT7q16WWsrvLl2EodiGjEMxDI1rq2tUDkNSwppT3+eu8oUEcSqZ7D64Ve59cGX0xloLiRhJ5jpVQrbtmmeGbMipNgaJa/dK855v1ZY5t+aA7z/8omUhU1FdAKCQADDJxrvT/D6+r2EFAgI5/O6ZevlGk80CvXBTSjEjeI5XuYnl3fC0S/va8U8w+9AUUSYM9csVf+TCWpj23jg4YscM75cj9URDGYtSmPfrc//ZBe7+3J3HNCzikrKVN61REswmF5ldU3U18OiW+KWoik9O2D9TSHvu8rUB61++FX6ptdp7c5JZaBdNt8xGy5rB4ihtEXIgkJP29Wrcl9LnJKxQQIBQTIpjbnXfx/Yp9L5XKzwjDmP2XraVMuUm0p71ufNitO8riTrteSblBg7ImnadIi+uKBix2Ya775R0zh7mLCTsQOFT7xFhPmGshBH72ZWrb2KqgMd2oHBIGzebDzlC5dvISnStQUDyQQ1sW1ae5tDnay6/X0c3q94JgWvbWt0ohl7RhdjwioiZbyEFEik3A5f/ugk/uWGoOZuSKWxPni9wv7dImtmqmUM5ZJVa6/ioZ/8ARlMj0MAX5/QURQSzQoXhi00I3rZd7uYvWSiYeFC2p0wZoLCwD6V7tf2c/OVEz0nb7i1zckFe8UxcLgWh+tX5kTcukM5YihtjHziPU5wPBKvGbELFtF07W30TZtDRVvKOujpNJ7yZZc/SXtY66wghERJxFEJGr/XTg7x4pqqYSmT4MQ5V9+RWeJPu560tZwvKTn1+Trvssrh7zlWCFIX01VWzcol99NRPpOaqlE03TGJ/lj+ZTMXXtvOez850ajRq5Pu84/2csf1k5g/J3/9naWkZQL274Kr60M51ySHch7ataCiBkdrX/rgoHYjmL7Melry+n7dFgYvu4aTkXh9H+9RwG/ueJzeGXORikLvjLn85o7HLb7NVWuvoja2LeW3C6EGS9LtbaSgo+uIYxWyvKp2pZx4DTNb2LQhYYllOZX40z477R/OV5rlFH0/miUCLT7MDY8QTU5j5ZL7tf5tIkj7bpWzP95dkMuy5lSF19fvNfTOA/tUXlu3l0CAgkgXTCUtU66dn16jeMq8078nM4xApP6lb90KySRd42pY1riOhR9oZv4nu6ifr2Z8v266Ybc2RkPNFjxR4RPvUUBMKojUEy0CAWLSGpio6u/kgbeuMzoE1E42BZaSCWr2bnOspZtXPdvUE9FKXbqOa4rAzQGbkIJj1DzfzFSn6Lujfjca1UpcujTD9IpcwSELITCXBprpCEdMCxyUjFUL0v2uWjGJyjLB84/28tTPdvP8o70cPpjwrFRwgl7ScuW7Q9zZGGJPh/AkGtC/JyMQaSr5CKRN4UAgvfAEFHb3aRJE+/frpht2WkS7elXGntHFB5e3s+DyLkrKVF/okIKv4z0K6E/5+szb0GyVvlatmJT2j/ZtY9XaqziMQgPNWheL5GaaV+6n6fA51pTWfhWUUuc9XsrCrqOVd6rr+Pydksrp2hZ2zLh08M3JP5wLTu+xXEO28zQ0aBaYDr0ZZg4/in1La949O0lKLeKJlAZ4QewvJhcP1ExWeKoA941emL6QucuGurrCC49ZZLr1n4ZNbVqx1kBAe7GkJGPhcVK/uOmG9UXUjK/+oNuIFZSGtYAtu6eweqO10NDJCN/HW0S4+a6uvn03k84abwm03Pe1yd5OanLadY2r0XyS4Qg1+7az4N8/yH415TNNJKjY0arVinVy0qXOE01O476mNxk/fZQhEdOrgxUKJ3+u59qtTtEgB+eqvVLYT1covPysMEgpw6dpO4WTj/rJv3oLQh4VRKNEF6+gYesd2mI7K5lTmZDtXOaGpw0007q9hPM+20VorPv3Fo3CP97SRaBUq3aX67u1twOSEhq/PIUDSb/1j+9qOAq4+cqJdD4X408P7KbzuRg3X5nudpQz997ktDNvDdsnRHht/Z70dm9HK43Xf0J7j5OYPXWeSLCd8ulBS4PGoRZ/yavrsR1OZpzD3+xulfOutfq8Ibuk1MlH7dYE8phAQwOR6FO0cLrWMqrkrMLFHiY/UUPJOjZFSwiNURmMp+duysRghoXe0ACv/C6t844fzG7FO2mvddKFk7vZpU+8RwHZHvCcuff6Q2PfGgaCRLcPpn2mN32G8C6toWTXhGks++yfrWRuevgqyhQjMJJMwO5t3orOuCGvrsd2NDdbiwTNmuXoXLVXCqucbiXaWbOyB/+KXM3RHSnnczQ4m/pRW1EU6W2uTb6RrrJqlp1x19AL45hO+64l3Ywerxqu9ZAiMhae1lYY2Kfw4sNV/OUntTz/q+yLk1Nyh1sQ7mSDT7zHGDxbi+vWUbNvOyLVkEsgrQRnMulu/vwjVF95Dh9eNpnq88Pc/GCvxbJ+ae0exivpiPmD1ytDikB7ze5yRCSiNcB0aIZphv0BDoesRLtu3VEi1izo6lVZdksnCz/QzD82rmfHqBoSCeFtrk3BV2OnkyMF3Av0044Jp4vlu913+SamORkYfrNLDb6Pt4goRJ+Yj3/Ua2LE//engYxgXudzsYzPeeiWqrxE815RjMSyYreCHy6Yr/28z3YRKj2CDARJJuFQTDEK/eSca9OJMhJsAnDfDbWe5tg+b+8JKVxxibAkzbjdd0VKEPR1vD5GBk5SJ90Cbd+togTdc/bNqNrfzgNrLuKpH0d4YM1FVO1vdzxOL98H6UpSTpa1btGMHqey4PIuPrC8wK2s7QLt3QyGQ8uZq5SkGwrtUFwozLK1YKlquIZ0K1P/OadCweQbqakaleHKyaqXNX0fTetbUz39NHfNC3GVlhZ47O5JTK/Ovkvx6p4ZthrBJzB8i7eIcFvJnSLqC5YWoATwmD5271txYoMSERDIpCRcIixlFvXP+9ZnqzJShvNWJTiMS0keIYFCebXkyju1ymaVZSNrperWmrnOxEhky5lFGgsuT3c3FskECgrzFk42mpJ+Zq63+XDa6dROVtx3K6bv49aXBjLTtD2kHueDfFUtvsXrY0RgL8C1YYNkR2c8fyWASyUvu1X30elBJo4RRvm+K+Yojn5Y3aIZNzFdp8EyFq9tMGzjmkEUSJNuIDg8vdpywTwP97XEeeeAtFRWG4moutmSNSq/SaitHsWl10xm8kyMpqRe58PJd5rV/2r6Pip2bEYk9LhA/sEtL9bskFQtJwlOTs/2UYZZCK8rGgdiIcaE41rPKq9KABdFvV1qtW5nIsOqC49yt0JqTlUsFosxFoeC2l1/fSPTz1xXBxs2ZJzXifS04iqSip1RGq/9GOGxo4bNeWieh/FT4PN3qPS0kWHxQvF8xs3NWmsigMMHNJ9uMAh/Vq31DVwXAY+O1eZmrctFKvvXSCCJRLDcJ403fIqHf/IEeydPQwKDCfhJS5zYoPW63eIHuupGmjpl2JNjppyiZa1l3D8+DPgW71GANX9ee7jfXDuJgViIQFKldrLCN5ZX5vZFuhRMGGpTRldVgt3C3rSJlV/7G+2dR1IR9rgWYbdpt7YTAQQ9bZpyQr9qIfSxCvqmTKfp9t8Oa0K/eR4CQY1wH7xeoWeHNg5zVD2vdOscMFvaTx+Js+AfpKM16kla5bHYQSr5zPgcna8By30SHjeKQFWV8bkH4rB3MPO63WSNTtas/ViJLFzVcpLAJ96RRGqrHpmj0EI982YNGvUWDh8I8vrDFdz39Aoe+FYVz+wlNxG4RDsypFYl8KM34vzHy3G++mic91wgs+pGXXXG9v2sotBRWm0t4PNOSiM8b55xrF5Xwk56SWlaIIJB+qbNGdbOBeZ5AC0dev9uwfqbQiytsAblhrODsJ3Er7zLueaDJ2lVHt0jXA+13Sd9yVBG12awXrebu8BJo20/dvc7g7z47b385Z4qXvzFRA7v9y1eO3ziHUnYrJdmGlBCeoFqQZwQDehWq7QRQfbAg9n9+tMVCuMC6QdaorXo0a2+865V8zIqDQvul6+x+vEWYrUzNQZJJKiJRdNa4qSpEIzJymqedQNzZyUySO+U0aT9jYkEFW2btfcOU+cCM7GdMhq+ckGQe9+K84VfapaoeRcxnMJ+O4kfSDqrATwpM/IQz3o91L4g6TBft1sSjNNuyHJsMsFgTCs8lEBh09agX5HMAb6qoYjIiNba6xAEgyioxp9Gj9MKiYybqPKBSycwKjwKgkGNlHbtYHmDrb6fCdkEDvZaqUkVvv2+kGeNrmuR6/p6ujr7WXnxT416Eaue+CeqBro0ltHNOxd/beyIpKn5zXRd4us/Qbhzu1ZKy+E9XnXLeV8HNh9vIE7jdZcS/r8/eRasmt8vhGbN4/A5eSMP8azXQ81jnVCijdGrj9cJ9iL/TWvfT/+B9MqVoVG2DTSyYQPbOblUDUUnXiHExcBdQBD4qZTy+7bXRwG/AM4B9gCXSyl3ZDvncUu8DuxoLji94PK0jGtUWZCzF5UzPiw0Uvrapwi3bXX9LAdON2721Rvj9PS7tOrx8LS6dj8wvzcYhHgczPeTlwraeVRUH1LxnWzXMYQx6TCTejKpLW6BYH4yMTcUK3GhKKivp37DI2xiLkmCBEgwd17QOn22+W1JJjmdk4t4i+pqEEIEgXuAjwDzgCuEEPNsh30R2CulnAX8ELi1mGM6qnAIhpn/NKY8LeM60p/g+d/28osFUZZffrYW7TfBLhk75/3OARxIWTGhNOk+f7eSjn95CN64bsPNvsNEwkq64M1fm0dFdbsvsW2X6kmgr8+VnXRd3QkFdOW1BPIC2r9vvSfEPZ/xntwBzoq946qYeHOz5lrSG7POSmR+pbb5PRlbYhbbx7sA2CqljEopB4E1wCW2Yy4BHkz9/ChwodBNxRMNDsEw85+mVymW530gptBKnSMhmQM4ew7DR245zAev1gpO189XLYeHRwm+cmaIfz83xA8vC/HCX0TaYvJAMu8JKexNdT/Yu1P73YJolFjNTFY3vc6tLw6wuul1YtUzHB2NGcSC92o1Tp0xctUqiB2R3LdRNdrm6KgYDY2hLmddcgHdcs2LUzKh9aIrJE7oRLKuX5FXXXW+GMp5IxEiW9bRIutRpULLFofSlbb5PRlroxebeKuBDtPvO1N/czxGSqkC+4BTijyuYxKrVkwieUgruXcopvD2E5Oom6c4EpLZwgIoGasV7x57itY5wPNW1APJXHGJ4LZLte4Ht10a4opLbOzX0EDTbY9oHYMVhb7pdTTd+ZjjgjEU600P7JghJezoUvnQinY++61M67cpqhr+VjOWnxYifMkS58Hk29eIdCDPXGgoG2fr3FY5TfKN5vTOpfugzCDZuhlp9UuABHUzBrUDimUKF+O8ZjIfHNTu59T8HssGfLFw3KgahBBXCyFeFkK83NPTc7SHUxRUTVT4+U1VdD9byyuPVjG9WnF95i0Wlt7FggIyhTyQTE6juLWVvmlzkMGUrCwYpG/mPMcFo4BdvAFd5jZtStry1V0PQkBXT6b16yQLM5r/ug3GYWei88bYcpUPfqGThV/ezrKlT9F1zoUQjRoKhaUVIdbfFGL/bpExneasr3+8pYsdnSqfu11l/JS0lOuLd6sZ62AzDemtO5u4J75c47ANb1CffJMoM4Ykw8uoX3HwSOFfkhvMZB6NaqLj1PxuH/rZjzsUm3g7gRrT71NTf3M8RgihABPQgmwWSCnvk1KeK6U8t7KyskjDPfrwWojELJWK9yd4ff1eIHemUMZDVj0j5wfmNIrr6qho22yVhrn4TwvYxWdAt3xlihsMKVMgc9FxGofhis5jMDpv1C/uJjAmwagJJVQvP48H7/tfVrcMEjsiiR2RPH1Ek6vd+1ac516Vluk0JxoESlVOv7g7I5svXA3fWHeIj/xrJ+d/rov7H1KJbH9aK4BOiBZO55q2f9M4DMXoF1fwZOKQPHL3H4b+JdkxlBX3BESxifclYLYQYoYQogRYCvzedszvgStTP18G/EkeL+HNowiLBnReiMoy4SlTqCmq+Tsl0NMP31+v5nTh5TSKm5tpvPtGxu3YTjIh2b0jyE9XKI7nLWAXnwHd8u1+tpaBvWm/uExmLjqNESVt4WILquUxGJ039Lq1Zy0uZ0xYQQRSWXdRNWv2WzSquUT0O1uvTmbO5tMHWFYe5OyPlBMaq/LjP3ZDXZ1WzP7yJ1n4pW2MvbyckjLt3Hq/uIInE4fkkamRoX9JdgzHinsCYSTkZEuAO9HkZPdLKVcJIb4DvCyl/L0QYjTwEHAW0AcslVJmpYLjVk7mhBHWCmVoehPwqytDrmqpfPScBaiwhoRoFC5tVCmd3c2YcpWqiQq3XZc5vnzrMDgdf/7ZWsHycxu1CmOLlk82Sm1C2u3jJlerr9eqvunVyWRSktgn2fh8LV+8O0F4qnUMyaTkqZ/tJhCAp27QCqi3l05FBoLIVOD1xYerhmWes+mbhw1Z7vOTsTqZn0BRRHi6oUaQraJRuK8lzvgp2vZWSkjE4a5PK/S0ORNRPtrZbFriYxFuhOxERBeOCtHQAG1dKmc3vMMHryynLBxEBAIIJBWjM1OPjxxQefaRHmpOVWi6YxKJhNZiZ0xYZSCm8NgT51F1aBckEqx+7G36pkaQpIvV/+23vcZ8OzWOfHZ17bCs1Ue7qPzJSLzHTXDthMUI+r4aGuCn1ygkU5JbITQC/uLd7uyYT4m/Yu4mi1HA/NebVHr6026XX29S6epV6R2wp2unfe8H9yo884tq/vX9pUwcE0gRs6AxYm1rc+SAyktr+4zCMWd/vJvBfs1KfeYn1Rx8eC9V+9q0CH8iQeM1H6NiZ9Tw2b/x5F6L28ipcaTulh89fmiFxwstKm9GPgo0+7EwI+/PO97hE+/Rxgj6vlpbYU+HMFpzg0a85VPd35NP48rh8N+6YTirh+nQ61eA9n8srgXA+vepJFMaNJmUjgE6J7Iy/+3ZR3oY2K+Z/1JCydhUoZyUMqHZJqIKd2xj+SdO5+tnhbjpg6U0f6/aUqAoWx+7nA1Ss2EYtMCxI5L7WuJ89sE4/7xGq3ucTYFmV6vBMN4oxwl84j3aGAJb5fvM6Bzf24GFWMZnKXfg9MBnsz7HVkr+eY32ED5xYJha60Sj9PWrw94WXK+UBmn9bcc7Kq+t28tAinz796kFNWTMWLAmK5p4ZFs7LfM+TSTYrkmqjBUw+6KbrTO1064k271hee20JNGNR4ak2W2Kqob7qnK6Vvc428bNvsnjJMxd84n3aCOLfizX9jpfnbvO8a+t28NALE0sr63PUO8ZcHrg3azPhgat8pleaDwWH6YuEw0N1s4JWeRq+eD5u1NlKtV0KnXNqQqHDyZ4/tFenr5/N53PxQraertaqObve+NGOO20IW8RnHYl2e4Ny2uDM2iQvwMgmpxG/YZH8jZ++w5bdw6V0+Gc97vfu/ZNHidh7pofXCsihho0yBVt9hTMcogmL7xDsQRqAgF46u5a1+O9Fs1RFPjO3+IEFPNrkq+fVZL13K7qhP3t2vEbNhCrnkHTnY+lK5k1vGvIASCn4YweP7QKaEcD+fZgy7hvUFEJUc/b6eI2ecR5V2+MGynZyYRW97i2ViuH6XTv2ud9w4YIsP2kCq75xFtEuBKvRwlZrqpglipQbg+Kg2pi2dIn3ZUK9uP11gamsa4+UuO4INTXW5tJJhOSyl3RdDlLFwVHptQKplcrPLDmInOPJA35Kj/MVWZ0xjnmS3wNHdnEMtbXJHOVbbQk5qIkDpMwdQPzqkpxUkX8ZIPqKq2zw1c1+BgZZNkHmt0L5oIwIpGgYtsG7alZvNgopG6kkrrtVB1UE9kCNRnHb92aMVa3zgnNzfD89dtT23dJeMdWGq/9WNax6H/WExPAlIFmPh6IMoN6pRWl9W3vW2Fzn7iUgiB24Ag/ejvpuSOHKwoITBWrro0d2UIH1tcEzRtngapSN08pKM7rFGgczsLyJyJ8i7eIcF3Js/gI7O4FIUCqKhU7UoXCd7VZLUDb+zOQr07Yfnw+n5Xr84Zi8QYC1CutbFJnpd8eGaSZBhq23kErddTNStK8zlYNyz7XwOqm1+mZfhqBoMisT5wPCtBgj3SSST4YzlyefLTBJ6PF6xNvEeF6Q9k7NxzqZNXt76NqouLsXnh3aQZ5GKSY6+lNPU1dXQOs/Pgv6BhbS83kkLvv0v706e1qvTKFw9MbJZL6k6QuuI1m9SMQidBAM63bS5gxA4KlKhPmufh4U+dSWt8mkUg/vEFU6mj1XnQ7hVtfGkAG09eeb0cOAx6c7Hb/a9Mdk+iP5b+dHwnoZLnnsFZISMr8EioK7RByMhKv72o4GmhuZuUlD9EenkkyoNA+ttbQXmZs0QJx7enUEQjArFneJWipKPrKG56jfew0klK4aj2jUahviKC0tlBfpxJtboF16/KTuzmoNNKeFcEmdRYNc7fQULKOTdESo1hVMKHwwpoq/nxvLb/6bkouZTtXXZ2wboVppZU6kmjzkySYKWNK7au7Jkxj2dKnWPilbRyODZJMaA+5XjtX31abK4jlTEaoqyMqZlLP2yjEqQ9uynAd2DW2Z3+8O3M7P0z+h6GeRrdQId2INB/N9JD0xCcZfOI9GohE6Bg3LbM7Lw6dZ6+7VGupo0NRNDL0WDxch5cMNEfXs9dyaVng5NotJGEvw2856wajgzGkatXa/ZL6wvO152mvmE0yoPDSUwcZ7E84duTIizyam2kIPZFu7KjOzJD02efdSKQwr2O5dIEeGXWoZXTtNZ4hP810PlmOJzt84j1KiMwo4bzLJrLwi5M577KJRGZokitzoOLCUSHO/+sPUeQg9byt1V1NJAoiPy8ZaG5k2NWrsuxbbSxcYa1B6xVOyXmFJOxlrAHr7s3dZiYFMykM7E/wf009jh058iKPSITWxKy0xZ0UGQuIvQNvzZ7NtFCPujmaXsdyrUIeGbXQ7HOd13dvs1VKI0tgzGExyCfL8WSHT7wjBduNetaHxlM2QSEQEJRNUDhrUWbTjYYGU5tsve5qgSnFWZUMKbiR4cp7u2nvSZIUQdrDM1k5+5tEF6/wtq2NRmkeXMzcZItGjpFBmput1mv9fJX5nyyg1oCXNjMpeCWFfMnDPGegXY95Lox5lwlqY9tYtfYqjTwXL07fD8Fg1gy26KZB6pNvau6M5JtENw06GsGFZp/rvP7g9YqRzRcQmga7Yuc2Gi8+LfNLdlgMvNxjPjT4wbUiwhI0sIWzb33hoCXAIxIqX3/vOEs42VHovq29aPpTt6i2vTJWIKmy6yeH2BSoZ8IUyZV3atlqlWUOgRgPYfyhdg/2Aq+Bn3wDRNGolnw2mOrGI4T2uz3+2FU+g5WLV2vB1FiUVWuvoqq/Mz0vWTTG9aO2smlwRjqAWLIdZs3KmNbm5sJUCU4xws2boeG0rbQOTqeOVprFJUROG5W+sGEsRXcyBtd84i0iLDeU7UZd3fQ6fTPnabKxZAKhxpEBRcvKuvtGwn9Zf9SkR3YCnv/JLnb3HEEGgoikZrk99PAFJFC4vimdMOGYoTSzRZN60UozDVqNAtsDmkHsMsFTq2cfk4kO+WaJ6Vh25bNGPV19Dh94+KLsb0pBUSTjJ6MtcNO0YOAvv6bQ2y68vD0nnO4zgE0bEmmyZxMtwTPTHzKMN+fJSLy+q2GkYNsHNt59oxFEE2qcZDCUbhR57W1Acat9OUGP6H/xtnbGntFFaIzKpk3w1tpJ1FYG0tvlLd+jblaSQICM1jXmQIxXV4l5ey+TkgN7R1GfeEMr3nKM9TJ3Cr7Zt/jzzsxURnSMrU0HUwNBOsIzPfsF6uqEsasIKFotBKfebKAtdrNna5a3ENrPhXQYaW3FqhahzjrGkb45TzD4Fm8RYVnJs6jTb335UKbb4dxS4/eRKlRt3vInk1qn4xcfrnK0pvTLufj/xTmlVhIICGRSEi4RrDhDs3i9ukq6elVW3tXJjh4YiIV4c+0kBg+ITCsrTxTiNsi1Vc+wzgNw3w21mTuEPqvrBLC6UyokD/zPEmhtJTrjQkPT7PS50Sis6YsbCxxoC/YvPhcyPvM3v5O8ENfqC+tdjvd2avfIvHn5G6OaQStJJoXh3mjZGCjK7sO3eH0UD1lkWRUhaa28FbLegMWoResEc0Rf7wnmZozpl3MgusdSQtFc6Swj2DMvRXq2qFDVRIUH/mcJz/6kmhcfruLwAYUkQdrGzWTZZ/+cV9DNosP9ThdtuzTrtKdfsnpD9kLqXsQDTsE3+1f7zt5MZYTukhAClCB09AmWLX2Srt2HLZpmp8+NRDT/uT0F1/yZL8RVo0pY5XTNLaGjkNr6mkErNIN2XlBLKx5O0jVFB9/m5CuF7hPvMYDGuaVUlAW1B6osSOPcUsvrGc0IPeoqdXjt3mDd8mt9vXLtIqPbB3n+0V6e+tlunn+0l+j2QeM1x92oG7u1tmZocs/+6G7ax9bmJcg3uwLiJp6ev6icUFkQCew5DD/eoFrmInZEsuiWON/9e5zrm+JMmCIdCcscua+aqBBXZcbC4ETOennN2skKakJLUNCvyYsMzK0+hg7zPRIIai4gDbIgIcwwyLezw3QfzOXkK4XuE+8xgFytV4ZacMSrxWwmlenVCo/dPSnnQ5dNfuX48LqxTF0dzeKStCa3ZDslFQGk1Leh3gT5ZqvdjDEp6Z4Z5rloilp9qFfeqToSlrk+saLArt5ExsKQTVblpBPWdwajx6ksuLyLDyzXiPz1zYcN6/2rP9jFRyuFp3skmZD0tAFIZoXaht39OiyJdqb7IMjJVwrdJ97jALmsHTOcHgqvFnO2LgduyFu76SY2bW4mctooWoJnos47k5aNAWom5y/Ity8EIUX7mHh/IuNY81w4FfPORVhuyRbZ5tFpodJ3BnojTCE0Iv/qHd1s78ydRRc7Ikmmat8iJRU7t3LT9XVIAmxJziISGd6qaEPNkAMs90GCk68Uuk+8xwJyPBW6Rdw4IcSdl4WYWCZcHx6nh6KYJfryJmu3aLiDeVyIIN/+nge+rY3tuqpuTtm5TWPIFFua58I+R5VlubfXhWRqOV2TfunjJqqI1BMpU+XpAqbf3Sz+pqhKTNcRJ5ME1Tjhzu2WhW1YyDKFYenParoPNgHHlnal+PBVDUWE52itR02kl8OcdO29/Ue3fXe+KIqKIzV5sSnTtE4W0+dQUaYY5y7kMwutxuUGu6qEJBBIF6KbUe2cWJJR0c5LMs4w636Hoi8/GVUNPvEWEZ5vKI9PhZfDvD4UIyFRK7S+a66WR/nAuM5+U03jzu3EamfS9MRGz9c/nLVq3WAm8sEDCm8/VcHsD/QxJqySOKSw5nZnYvcyX8NJlkOZC6f3zpzpE+9xgROOeD0+FaNGpVNTQevIc+SI9RivD0XWh3WYWMapi1BFtTQaYoZD8Jm5mYTn2vKoAFiuM5GgYkcryy8/m9WPt9A3daZncs+HuIbDEn5zq+TXG7Xuvft3wWdOU3jXLOeFwcsierSKnNvhNI8bNpx8xOuXDzoW4JRk7wC7deu0VdT9hblgD7jtOSyJXbCI8P/9CYJBYpOm0rTmFW1L3tJGY7XM2yJ26iJ0/fcyuxCbCS92RGpdN1KDG6pP2nKdwSB90+fA3Ln0TY1YA479KrELPkrTXY/TlwxlEEo+fk1d0iZNkjEvtSfMhP2BT1cSnqo9nuVTNZ3uu3BeGPQYQDZ4vS+8wEkl43VHMiz+4RMAfnDtGECUCPW0oKBSTwtRnE2RuXOtggA9p74QVATiWHRXEi1VOZGAwUGafvg/9E2vQwYV+qZMzytpQ09iWHRDJ99cf4hVL2na2PJqaUkxDgQzFRZNUZWkaVhCZFdxuMGp1KGmk1agpYWK0SIdTEskqNixmaZrb6MvHnCU3eVT+StbaclscVSzBjlUlk5TK0S7XUzkqys3J7Wc99kuxkzQ5iOfCmonGopCvEKI24QQm4QQbwohHhNChF2O2yGEeEsI8boQ4tj3HQwBrbvj3PLMIf7jlUFueeYQrbvTxc29RpyHMz2+8bpLrX8Qgr5pc4xf+6bNQaY6X8hgMK8HXyeQsy8uZ2xF0JBnLf+RSk9bmgiTiUxr1v45UpJhaWfrEqEni6zpi7PoljiPfy9olDo0S/EMiV5CpWJHK43Xf8J6zbax5Jp7nVDHlqskbGuUWe2Q7bu21AxOZQNCdqt/qDIxr8k1ZpgVIFptjXjWzELLgjJW5ZxLuk/6Eg/FsnifBE6XUr4L2Ax8M8uxH5JSzh+qz+RYx5rNKqGyIIGAIFQWZM1ma0qnl+2XY0JCgU9e+P/+xCnRjdZU5bbN2ouBABXtW9KvITMe/GzkpxOIOWkhEISKGq3bg06E4VCmNetF+mZ+kO2pwGu2WlNnL/1mgjsbQ3z7vdbEAyNp5cpzWX752YQ7t1PRttl0zdbPzpXJpRGqpH5xt8k/LQkppGVw0SitG1TX79osT3t9/V7i/Ymc2u2hysQKSUfXFy2pp4mv25tVZ5zRhWOcWryMuOMERSFeKeV6KaX+Df4dmFqMzzmeoJMuYJCvjkILWANaQe0NG7Qnb8MG7XcvqKuj8YZPUbGjVbP6urbTePeNhknXeOaEdBrzaJHx4GdrkaMTiNlqSyZg7074zf2CH14W4t/PDfGVMzMzsLwki5gfZHMqcN9hiA06p87aC5QbMJmyjXffSEUo6SlRxQ5t8RSWNvUgSCRJB9YaGpg3bjMLLu/igi+1s+DyLuadmSY6s8a3skywfJ57NqP1c7WfC/GZenEb2K1i0AKRTz+gpYkfOpBASmjbpVoWYv19Fy7TuqyUjgv6nSlSGIkZuAp42OU1CawXQkjgJ1LK+0ZgPEcF8f6EQb7JpLRkUnmMrTkiujVBA2+na95ubXDxEKfR1auy8pNr6ehNUvPoNlZtuYGqptXwl/XGMWFgeZZzZPNjrloxia//dzevrdvLWYvKGRPWasf+4nqF5nHZgzxeAkU1pypG8MpsVesEIlI/640sQWtb19Dg8NmmqFOua86Gujqtfu1ATDHa1Itkgpopo7QDolHYsIEzLu+hK1yGCAjGhOPMWtINaIE3PRlFVw081CGp6IlnVQ3U1VlVAvn6TCtGk6FuscMtmGb+HnSYF+LzLquk7zAIvcvK4nI6n4v5nSkYgsUrhHhKCPG2w79LTMesBFTgVy6neb+U8mzgI8A1QogPZvm8q4UQLwshXu7p6Sl02EcNS+coxPsTBukunZOjpgHevAgNNGfWvM2Blfd2094ntFY+p8xh5aUP5b3nc8ra0i2chzoksy4sRwh4/re9rF+9m+ce6WFPR2ZPskJgtgzNC5gAykvS7gq9PCJoi0MxI+jNzWilE9dWkIwlCCQT1B7amSaZlA/gnXANIrVQiIDgnb2ZW/t8tv9D9ft72WG4WcXG9yCkJVArJXR0HaHvsEwvhgHBuPKQ51T0Ex0Fz4CUcmG214UQ/wh8DLhQugj0pJSdqf+7hRCPAQuAZ1yOvQ+4DzQdb6HjPlqomxzipsn5aVF1/10ymfbf2S22jPbmHsqNDEc32FUrJmVoVc2EESoLMn9ROc8/2puzxKQnkanpmKq6Oh5IHZNNU1r/Odi3S3t7ICCpC24DZW5RMiAiEbR6tQ3nwKOm69BJJsX6NbEo7eGZWicKIak5NfOeyEc1MFSZmJcdhptVrFvo1Nez7Iy70teVTFAT20bFziMZWmkfGoqlargY+Dfg41LKAZdjyoQQ4/SfgUXA28UYz/GKXP67rl6V8z7/juEvHDPuCHWzkpknsqHQbrBmC/yif1D41gdUnvrzR3jgllqq/uFMi4UTCAjGTEhZm7lKTHqJELkck62ym8UaVLbRHL94eIoVuCFbBC7lyF+19ipqY9u0bh6TQ47b7mLW1igE2azirl6VZWfcRUd4JkpSRSRVo6ln47Uf81zc6WRDUTLXhBBbgVGAXhX771LKLwshqoCfSimXCCEiwGOp1xXg11LKVV7Of8JlrrkgV7aUPbc/eUjh5zdV5TTksmVWZbUg7eNRttKi1hl/MGeDARw5oPLsIz25s7e85EJ7OCZrxpiXzyhmXnAe5x6pjiP5wG1My77bRXvnkcxecnnkJfu1Go4TnGjE63ZT53pWndrQPHV37ZDGnC2V2LGVjymbKt/6B0Bmm163B3ao3Yq95Pw6HNP11zeGtRBO3hiJIhEePnf1r1+iLxnKuC+cOlA/9dM5eY31ZCReP3PtGIBbMCWXdrRQl0E2ZPMvZsjeSnZY/hAeOyprQXdHNDRokgMdiuLsj/AQRcrqu87yfkMu9eDLrH74VWLVMwzfTjbZXMb780hC8AR9UdLlghs35u8iiUbpOudCli19ioUrtrPsW22eWijZXTt9ceF4X2Tcg9Wj0zcsDF8R4BMMPvEeA7CTXe9AZjsZJxRSrzZb4gPAuIA1s6yvI/3c3HOPjbvWlXgLqZucw7ELFrH6jYE0SR08Yk1dTiScrSQPvWgcFyL9s+eksvI2b854v7HwBbUuz7++8w/U8zZK4jA7unIHIovWE6+hwVoVyUWakfU7bWhg5exv0h6eqalYepKeWijZAwwVOzZn+J1jRyQLLq1k4VWaTnf02CBxVaY/fziLAJ9g8In3GIA9BbN/X+6uA5COKt93Qy0vrtH6eeUyLHJZcA9el8osUzU51uqvKEZuxoc+pB1jcNcFtd4aczU00NXZz7LLnuA/v/U4vWo64aHp7j8MIXvECseFyMPDby+kE5s2y5DoDexVkHrqbjJBTbnVmo1Goae/sJ54uRZBR/2bw/xk/U5bW+kIR6yt5b2oWGzbm8a7b8wIlDVFVfarmlRsTEqnu6s3kf58vyKOK3ziPQZgjhrrKZjgXeqVi1vMW+Hq88OMHht0Pf8r/ye4szHEygUh7mwMGS3CdThyVy7BcWsrKy/+Ke3hmYwJK4jUAy2BvqmRYSlAYQ+sXXd5BSvv7WbhB5pZ1riOrnE1rg+/XUXQ0yYMid6baycxEAsRMEXrzWhowEiBBuf6E26wE+bND/ZaXRbv/zCmNDitDqhpfvRp39GZxSqvq6MmFkWkBiiSCW8uKZtrJnz/jzPcSJYGmynytXx+XR3GFgSypA+efPCJ9xhAuHM7yy+bz9ffXcqOX7zBoQPpB2fyKcEs7/TWHde8FdYziMDZL2w2dJygc5fFr9kySOzAEXfmr6szrK7M4i8ir3a2blaincS+fnfq94BCe3gmK5fc72pR2+VSz9+tGHMweEBw8OG9PPWTmTzw8EVUvfFXy3tbW7UkDfMuwatsyu6TnnTWeKvL4q7H0+Q3b57m4zXNj77gIkt436cmsvCL2pZ/VFkwPTfNzaza8j1myk7Ob5zIwqurqftYJT9pyeGL9uDasTTYTEoG9qnWe6q5GUImjbCqGveGea3mJGzw7hNvETGDlDA5V3DBZLKKQVOxAUAgslqUXrrjmi0TPX3TzS+sGzpu0LnL4tecMp2mO36rHeBkVTY3U3OoE5FM8Nq6vQzsU5FJmZ+2MzUHN6/8O9XnhfnwsslUnx/m5gd7gUwSi6tp17EMBOkIR1wtarsW+Df3i7SxV7KdZj0ZMxAg9v4PW6zSc94v2bdL2yV8670h1t/kMahIpk+6bIJidVkkQxnkZ17wFt2iLbRnLT6FsrBiWJ1nLS5PuxwiEapeeZp3X/8eysIhQ0Gwd3DovmjzghXvT/DGk3ut91QkYpXBmO4N8y6Nk7DBu0+8RUQz2i2VM7hg8oXtGl9j2Z7t2qNm9SV46Y5r30pPHCMcm1OaFUROMHsDHAuMg7NVGYmw6vb3UVs9iiP9CTqfi3HltIA35UM0qgXkXj3ArT9/mWn/tIAxJpKZdNZ4wLm7cEa03WM5LIuxtzFA5LRRxsU33fW4xSq98i61YE+J3ScdLhE5EyfMC56+0E6swVKAKWPLj7Pfue8wntUYTmt/eJQwyHf0OIWPf2ESP/y3KVa5nUsFKLP792Rs8O4TbxFRBxiOgmzBBdPNafHH6du2LEEKL91xzZaJELAn9cDZHzSrFZJGIAAL/kFy71txvvDLOE8fiRMuMX+upGJXW1b2KaR1vD6opmtv04qyKwqBoJVkylLZcXYSu/6Tk4gfVJBJiB9U+PJHCyzMYtty61pW0MjvQDIvT4kF9jm5Yk5+dRP0hdZS49hpy48ziQuBZzWG49ofjdK0vpW+/kTqHDLzHC4yPqtL6+Rr8O4nUBQRLUIwlxT5ZsvkMZmaXWf+AyuX3E/HXpEW7P/Dma7i/3yynHI1RbQnSOiYNw+u+XWcA8n0eyeIOMGOdvqmTKNiVxuNp5USnjVtaBPmBEXh1r8dQCppEpFSIoRAJiXhXe2suHRuhmC/kOaOTnPZ1yks+Qv2eTBH+Icz08wtC8/pOzR//uEDKi//bx8Tx4iMjMQ1W9Nt4MtLNHeDGQLY9Icex2QRx8S/unpuffBlZFCxnMNLfzzz7iqRaAEakPL4CLz5mWvHOCJC0AzUB4MWYsg7JTRL9lI+iU1OTSTND9orj0/irVetVlZZWKXxhm5mL5loWJqQaiH+nrHD1+PbDfX1rL7l16k2REFEIoFIJpChEBU7ozRe8zHCHdsyxmAmitHjVN61pJtxEx2yz0wTuPqxt1O92IRBandeFrIQ+LkfkPzTvenv7oPl1iL3AKeMLrwrsg63LLzhTCe2k/jhAyrPPNzjmPnnuJC1Kqxe84rlu6koC+Z97Sdj5ppPvEWE2w01nO3LLQ8ECeayiZZ5n3ZkYPPn6uPqj2nytcMHE0yuUHj0B1WGZl8IeP/nuwiNVXnfpyZaat+esm0Dyxvnp0/u0pJ+yIhGiV315ZS7YQ4VIUnj3FKNbLLUX9DnZcIUyZcfOMzYCk1R8fr6vVSWCcdU4ltfGsiw3la+O5S1xMOy73ZlLkrA1yd05JXqa7dw7XVuhyMd3A47if/+F93070tfrPkzHRf4hnpiB47QdMdvte9mVxuNi+qyLgROlnx1pXbvHy9c5KcMH6fIt1lgNljcv3pZSJdAnu7r1SFEOgouJbyzV2XjRs21EAxq2aolYzUC0NUIyaQkthOtW8UwJT44wQjmzIlwfs96Ljz7TL5+binLzxyTfrCztO7QXYtX3qlqfd9SQaf5i8rp2J1mzq6uAZY1rmPhl7ZxeO8Rg8j1BTFXd5COd1Rrp42UWiOfrK1oFJZ+rZvtnWk5nBJk2NPB7bCrOSaOEa6f6aQu63qoma9+6AEefmocm/77ZT5aXZLT+vaSgn0ywCfeo4DhLPtnIQYS1JFi4g0biG1t40dvxPmPl+N89dE4ixfDhaNCmB8NnZD0B83+gNVMVkgm4dCBBP/3SC+/u62X//y4IHzzvxONLNRSa5NHqB98bVi18Z54yyFwo+t8r76jnQVLu5g8MzPiP3gwTSgrP/4LLZ02oPDS+v0c2a+Z+xJtGn/zO5lVtVBzqsLr69OLUrw/oQXFUitilBnUJ99E2fCGezH7BgiWplsGSaldd77p4Fnhoaq+HqAsmxDkg5dXMvdjlVnVDiv/OJr2sdM0rfTYaaz8Y+4beThqQZ8I8Il3hBGNwk9XKEbb8XEBD1rWLA+NwT2ozGUTzaQZqmnDALG4NKLf512r0tCQmaI8sE91fbhXrZhE8pCmDjgUU3h77SkauV9zDQ0l69gUqNe6X0RLCk7FN1/eey6Q/OiNOJ99MM6/PKy1hHcVhDiYYXaL6vAB1RLxP9iX4NXfp6+zY2ytkU470A9xFGNuYoPwQlzNqlpYtWISlWWCv/9PL1vW9rJ8Xkoil1oRLR1CXBaQ1latXrFZuFIzuUAViH1C9fvFw0qmqyw+/oVJjB6n5FQ7FEKixSjsdDzC9/EWEU4+3kKi7Z7eFI3CzJmWP9364oBFDZBU4dvvC9Hbn1+AJhqFhpkt6b5uNBAJtqOg5ixx6wR7hH3/brjvSwp7OgTXN8W1hJBgqmfaDvivy0PGJecKLtnLFI4uCzL3vZOYOE0710M3KJw6ThjTt+y7XfT0S+YvKjcsfyFs/loPUXrnSWtA2fAGCVOjl2AwvcU2BzW3bYPTL+5mTFglcUhhze3W8pNdr0ZZeVcnHaXV1Bzq5BvX1fJMaZXzPDjdL5p8AMtAXL4spyCs0xxkLcPpAt/Hq8G3eEcKKSskW3tvV3gpNhKJaM5Zk0Oyom0zyUTK95hq/FhXBwMHEjz/aA9P/mwXzz/aw8ABBw2Z7dQt8z6NGhhFC6cTCWgnKrQ7clM0TboA406Fz9+hkUDltMyEEPMWP1clMLNFlUzCng7BXZ8Occv5If57aYhTxwl+87t09teCSyt590crjMChnXQLdgOlrPG6eUrGHNmt8jOWdDO9WuGVR6vofraWn9+UaeGuvKuT9tKp2ra+dCpr+sLu8+B0v6S+rCgzjMprbq4Pr66wQqrjFaznPsHgE+9IIbXVq6OVABrReSYrrwxn83k2/vB6wju2kVQlPTvg+Rs7aW7OfPBvvKs7d9lUB39qoY0W7cFEITSCBWsygJ4QYt7i2wOTPQPSUrNBJwPdNfLm2kkkk5qxp7sLXoinyXu/CqPGKhZVgv7Zw9GuxmmOegekUVvhfZ+ayH5V5kzC6CittlQYC5WXugdoZ9jqHsyYYQzE4vrYkKBhZkvGl+6lASb4JDoU+MQ7UkhZIc00MJdNmk/WK1mZnt5oZCH1g685k6TJ59n11zf46od/zv88PZottz/Djd+7mBeeThKJZPrmunpVR/efpSDNr0bT9dc3LOzgoY6KI5wsqP27NHJ6/m6FcMj9oXcqzGKOjutk0P1sLS83VXH4gGKsVfr19AxIC2mB1cI7ZTT5FXN3gD3I175bNebo3I+kLewxExTO/UiF8T43d75e6wK0CmPxvYfyC9BGIkSbW9hAPUmClFdL/qUpyWdfnMPqW35N7KovG4dm62OXDV66YvvQ4BPvSCFltUbYTkvgXajzzvROViaGayhZx6ZoiVEjd+ZM55s8Wwt3e4BjYK/i6MkolvSnMaIQLkn/Xl4C31ikoKrwwl8EXznT/aHXrTGddF9bt9ca2Ek9/c2bZjNX2UowKI0FTr8ee4W08SGrdGvx1HRFOM9kYjtw5V2drnM3epxiUVqMHpdeXNxiYKuuq6b20E5EUkUhwctPHeDwAdV5gdq+3Tq21O/meNqVd6aLK/VNr6Pp2ttcLswbYkck97VoQdF/XhPnnQPSr3ueBT7xjhQK3ZfbYC0uosEpSJ0Rcd6dtl7jqqRqYto3d2jLJEdPxrBKf0zEFD77dL5c2sE3zgrxjbNCfKneu1WlW2Nb1vbyt9/2cuhAwhodTzFXJKk14lTrTjcWuI7dmZrkikCcQHsbUk2krlOybmfa5+1Zjms7sKM3iZRQOi7I+z41kdlLJvKjNzRpVjYfqvn7LSlTGXtGFwtXbGflD6KsevtmaiuDqMES+vcneebhHjb9oSdzgcpSmEaH2Zcug0F6Z5zmrSWQC5qiKuOnpP3yn79DNT6vaK2RjmP4xDtScNqXF7A3c6qXm5LtWremNqtWj6Ynk7CrN4GiYPjmHm9SHNeEYZX+DHMbGEtgp0Ky6vHPa/O4YYNrIDKYIppDBxI8/2gvf31wN8s/8272TapGpl6UCIu/NFtc00Iot/ya2JRpxoE1e7chk3DW4nLDrRCLawSVzYc670yVBZd3ccGX2nnP0i7GhOPariU8k5Wzv2kQOmRZDD0Upulpw5L00b+v8B2N3oXDHhTVF/CitUY6juF7w48mdDJKJtNk5KIt02U4Uy5QOeVchZcem8ThA9avz3yKVSsmuaag2h9YfU2ww36OIYn4PSgzsrZnt0H35QJW+ZQZtkCkahNvqAltXBU7NmfUG9BRV2dVZpnjmhqhSI2sp9fRdOdjLG+cT6xmJgs+N53ZUyZb5GmBoEY8utVuhi6Tu+I+SX8szGvr9zKwP5GWJKZqCtfs3Ub7KXMMCZfjYujwhXb1qsz/ZDeTelUG9ir8fXUlF35dZcwExXDZHOnPrm5xQ0MDLLoFiwxw/670Aj6cmZonCnyL92gij55Uhr9VQmisyiev62bePOsx5lPYI861k/O3Xl2j1oVEUTwoMwr2KTv5XxxcOvY5qJ2sQF0djTd8ioodrYiESsWuHWkLNBqleXAxc5MtWjA0MmjxEGmEkiLGYJC+aVpN4qZ7/sD+6tqUH1cYC162tkC6VSgCgjFhLY1bCCgdG+C8yzQFxAc+VcE39j6gWfpCK3fZdMckT1/Bynu72d2nlYsce4rK3Pf30PlcjKfv383zj/Zy+KDHlkAOcOrC8Y1FihG/GM5MzRMFPvEeTZjIKFYzk9WPve3qB3OTINmku65KM2NrLiS1B9tYdcf5hYeeC3EbFNKefbfqjd/tpD5vnqPUYtWKSdRWSAIyQe2ezZp74p57CI8bxfKl5/D1K89leb2p3kBDA5HoU7RwuqZhLjnLEgytGI2RlJBMSg7HjtAVnk7f1JkGIRua4gSEQ+7SLKf+ZQBnX5xWQIwqH80zP1jNA9+qYtdfannul1X0x9wz4rLO7TvqsHWprqsjaxcOr/K0kwl+5loRkbPcna0k4Z7qCAhhbNWurg8ZD/rNfz1EyVit2EsyKRk8mODmfyjNqywk4JoFl882P1tVMK/jcTruu7+yZkLpet6BmMLbT0xierXi7InJZxLySR3Mcp2guQfuenY/ofJSrfLZ//ZS2d3Ged94b97V58yV4/RO053PxZj7sUrHLLIcQ8tAvllmbveD03m+9dmq9PTPGNQyG7c/7bmEqV8W8jjBCUO8JtjTNJMJ+NWVIYMTvvfKIMIk8pdJyea1vd6I0gyXJzavBzMLeXnlNafjnvxr+mEPBuDIoPZaMpUM8cqjVVnJxVOt2nwYy+1iTAyy8J+2kAykfcIBIXn0jtq8a+a6jd2phOhHKwVLv9ZNsFTNWJTczpPXwoo7UdtTsvXSkcb5u45Qs1frxlzV3+l4b0yYIg05W2UZfP2iOvZ2bj+piNd3NRwjqBhtbRHes8Pq8u2PWUsP9sfUwvyhLr7WvKRjWdwGXt3WTseZfcqJpHWYY8KZTTztcIueW9QHj71NrGZmxvXndZ0mV0tNbJu1VdPkUEEJCG7vcdqmr7y3m9BYFRGA0rDKOZd050yp9pJlZnbd7+hyvh/clC6Gf15XYCy5P+MG0L9zQ0OcCjZeeedjOefnREPRiFcIcbMQolMI8Xrq3xKX4y4WQrQKIbYKIb5RrPEcS3CKTTVGFPbvSpPuQzcoFk7ofuRVBlLkOxBTeW1dn+XBaNuletNhupBJXtKxLClrXrObcx1Xc6piylCDgX0K99yT/dLcoucWMpoaoemeP3jTU7tdp2nVWLX2Kmpj2ww/6TeWVxasWXXSuzoRsnmRDASgZJzqmlKdj4LA7Lof2KulXYP1fnDzC1sWbr2rs+2L1b9zi4YYqEwFJU8mFNvL/UMp5X+6vSiECAL3ABcBO4GXhBC/l1JuKPK4jioyVGSLB2kpOYurNw3SoPwvrYmZ1NUJCyfc/PJNrNz3TU1SFItSPrqMQ2OqLeddeW93zupQbtoxL9IxL1v55uZMP54Tmpvhiqsk512rWT/hEMSOpM+3asUkYzt9KLWdvubN7JXcKkbbWtkLbcxWMhL0TZ05tG4ZJo1ZVX8nD7x1nTEws2tAtzi9dhdxslad3muWBzo1tbS7JrxCX09Gj9OsaX3lmzIxyKoVk4gdkfyxRzL3Y5WcZ/v+LWNKJqiJRTMWNv3e6GlLS88E0NO22fsgTxAUzccrhLgZOJiDeN8H3CylXJz6/ZsAUsrvZTv38e7jzXAzoqIGRuUu+2hitK6HmvncT63rZqHtYbzGpoazZZGX85nnqbxa8wtOnulO+rEjkvs2apI7AKQkEB8ktlswtrrEsLKG3BMty4S5+epzBj0d3utWjtHsr51yioJEsnuPJgf7xvJKntlLQT3ZdB/suY1dlIa1wuxm/2627ysfH3Lr7rjRpy7en+DHyxeye/PzJ5WPt9gW77VCiC8ALwNfk1Lutb1eDXSYft8JvKfIYzrqyBDlJz2WfTSRcRUwbUqXq+WTD7zmcQy3ED7X+czzpPsFs1mD4VFpzSwAQpAIlTCIoGeHZmXt3wVfXpTfPGVa+jMIu5jemsWpJVVICSIAi26Jc8VVCi/8JTsBerVWzckjWhAsgZSar//7q3sydj1eSVG3SMeEUxYvVv9utu/LktCSA99f3WMN3J11C7s3X+TpvScKhuTjFUI8JYR42+HfJcC9wExgPrALuH2In3W1EOJlIcTLPT09QznVUUeGm3XWDQUVti1Eh+kErwGxvITwHpIscp3PPE/61hSyk779HEIIKqrgzsYQK98d4j8/4R7schpyV6/KXS8cNiqa7TnskvKaenPjxadREd1kLAB6ycvzrs3t2lg8NYhAI7v4IPz6/wvmlFl7CYp6TUzR1/bp1c7+/uFKhLCPeUzYY1m7EwhDIl4p5UIp5ekO/34npXxHSpmQUiaB1cACh1N0AjWm36em/ub0WfdJKc+VUp5bWVk5lGEfdWTEbNbdW1ABnULrodqDOOe8X3ri/byE8B6SLHKdzzxPlWXeHvrGiEKAtHsnmZD0tOW+Nrchr7y329K6HaCvX81cSFJvDrdvY/llZyIT0iAvvXZBLqzbmUBNaGQXCML8KxIsXpx9/fISFM232JHbgj5ciRAZ1fFiJ1/9yGKqGqaYfv0E8LbDYS8Bs4UQM4QQJcBS4PfFGtMxi0IL2xYIexDnyrtUR963W4B9nXnIpDyY0fnIrrw+9OFRgt9+VaE7KlLpq4LfXJ8kGJREIjA46E5iTkN27CK8Y3PmQmJLWw63bTV1/5CEda9Ilp1A32FboZlpsHVr9vXLTJKTK7Q2Qhm1fPMsduS2oBdap9cOO7G/ufaqgs5zPKOYwbWH0NwMEtgBfElKuUsIUQX8VEq5JHXcEuBOIAjcL6Vclevcx3twLV/knZ2WA16DOAX1hxuWN5tQwMW75UjkGlLG65FBFpz3Aj2TpjH/IxMZM0Eh3jfAdcvOJry73aqMsL05VjuLptseoW/6HCpCksa5pRpRZRnE6o1xo8qXLiu8szHE6HEq71qi9WMbiCk8drezj9bt1PkmT9jnPuqgtvF6/3n5bD9z7TjB8Ui85gDN3p3ws2sVJo31dhMPF4fp8KpOyDct1YJCVwv7+wYHtb/lcfFu85XrejKGPLiYuDLAmv9qJlQxhnjfAEuv/Sh1W/+eOQ6v16soRBO1NNCcbh66rZ5IRHMB/XqTSiyuke7zdyv0dQoqzkmrDGRS88E6BbKG9H25TGRXZz9LL/4zwXAwd+q2A7xkRPrEe5zgeCReM9k5dc91Q1evyieuTVs7b67VykHOm5eby9x0t55Saxl+wvcytowPdao6loNN3Dgw5/XY39jayuo1r1hLRu5oZflNnyl821FfT/2GR9jEXJIECZBg7ryg67xGo/DF29oNVwG4ywaH/ftSFJZd9gTbw3PySt02wy3F2IyTkXj9lOERgqX6VMp/56XL8Mp7uw15T2lY23ICWqPC07ZmrS7mlj7q1Vc3TE0zDJjdm99fr7LHYWwZjlbIW/Hh5jLPeT326FowSN/0Oeki6alODa8/9grLfjXaUqHLM5o1SzeJds4kwaz3QCQC06u8+Wgdr28ojdDq6ugIR/JO3TbD1b9sGtfbwAzvpzwh4BPvCMHSpDHVaj0Xj0SjWs68sN34kHpgB6dnrQc4VN3tcMf8zLw23hR6tYzNlEscFTOpD21GSR6hnreJRha6s78Hgsl5Pa2tRJPTtPbnySPUD77KuK5OZGoBSCYlSQn/eyBA9flhRpUF8+9FF4k4tnzPhmyyQbNC5ekjcZ57VVqvbyidP5qbLU02k0lIHFI8LcB6+cj23SpKEALCNnbTuOYCQ1zTjzv4xDtCMEfl9++CX35NybC67LVOL21UMxpRDsQ0i+GUapV/bTrMrQ++7FoTwEz2oBHcSPS8cuuxZTZme3akiwJBOr3XbLY1hJ5gU2KW1oo8UE9DyToLW1q49rQk0Y1HvBGMG0nX1VnbnzOXB++YSf++BMmkNPyUIlUv96zF5Xn3ootGNbe1Pg+RiPNaYr4XVt7bzaoVkxxlgznb6uRRbD8DkQirbn8ftdWjCARgRrXCmtsneVqAde2wlFqnj5qUb9cYu2lcQSAPI/qEgE+8IwTz9v77DSF62kSG1WUXup9ybi/nf7qSRcsnc96nJiJkCYfWxgii8k93HiY8XUEGFfYc1rbudh7Ryd6Mkeh55UYG5sI4D92QLsICkJTw600q9Q0RlNYW6utUWhOzKClLsODyLj64vJ2xZ1i39RZjbnAGDfJ3qZPlIBg3K7C5me7qOfxLU5JVL8b5l6Yk0e0YnRqEwNIdeMwEJe+MwYaG9PcTCEBJiYPlHY2y8mt/o73zSOpeiLta1Tl3NV6rFrlAl5b94mYtIPaFm7s8uVdyaodN40oAeSwHJwR84j1KcKrkb79Zz//0eCbW6g95iPcsGsebA+9CLSmjfHow3b0Rbetu5xGd7O1Wr/FwDsX/p8PhHG5kYPZBnjpOoNiEFLF4houVdy3ppjTl4x4Ttm7rLcYcQVp1uykQIDrjQvdLc7MCIxG+eC9G2/PK6fDFu9OdGgb2qciUnlem2svnmzGYzQA1pnJmLTtKa5EpUa+UwtWqzrmr8eKo93Af5NuWKad22DSuTcDJ1gneJ96jBKcbueZUJV3bNZmgLKxYBPXlkRLNQXnkCBVlitVnvCP1s4Ox55rqORydf1PniE2uZfUtv+bWvimWCLz58+w+Vvu49nRoBVou+FI75zZ2oZSqjClXDYNNBKyWk9WYk9SV7DAIpoFm90vLYgWWT7UmMYSr4aJ/UHjoliqe/E4pExSBACaOEfzr+aUZW3+nBdWMbAao8XWgMBALGSQvks790Lp6VV5au4cDe+MWRYBlV+PFUe/hPig4+82tN5xpXKcD27Oe7cSDT7xHCW49sGbKTs771EQWLq8mqA4iUsJMe5qs3Wf80A3ag+m0m7RnfS2eGtR8sA++zOqHXyVWPcPK2PlYwikTrunOx1KyK0XzhaZelmindvIr28f19p/2GNatXuA7W0TfaswJmjfOMgimdXuJu2uzuZmu+Rew7PInWXj1VpZ9cq1BkPbFINaZ5qSX/5rknvmb+frn5rN8VIejGiSXZZjNANWt4fJqyfmfruSi5VM471MTmRnqcbSqV97bzbboIM8/2mspDpR3INWDH1izYE0LwYG2rPeF7qLItzfcyQKfeI8SnLZiVRMV3v2xiYybEEAEBMmgZgE7pcmafcZX14c4dZxw3U3a5WPrdiY0d0BQMdqSAxob6FpWr5ZwyoTrm2aSXZFOzgCIDTr7le3jSiQHLdZgydjsDRmzGXNZXZuRCCsvfYj2U+aQFEF29Ag+cW039fXwnpB1MfjZtYrFnbGBedRveITo4hWO05HLMtTH3Nsvuf7ROE370gFIfcxX3qkaLqZxEwK8+59Op2p/e8ZiaP4sc1pz3gVsPPiBV62YRO3BdgJJldrYNlb97vOeWHQosb0TGX67z6MEt8LjfVMjRodagkFkMOCYzmuGS21zV1h8sKa25MTj6QQCr09LqpZgRdvmdKIBafIFkwXmkNnQNb423WctCDJBuszlZMVzuUF7aur9D03iqs8rrgXZzaSl+49f3gRXXCJoaUnP951joc/I49CWk03MpWHrHThNuWORcofrbjpSkxGAbG4O0dBgq8QWDNKXDDrW7qxZ+qTxWa+v38u7l1QwepySfwEbD9XrqyYqPPCrD1lT4w4GM47ToSfIfOfvmhvswesV9u0S+cb2Tlj4mWtFRCEZOeYMN9D0j1LmX9Ta62cY2ViN87UXg8HMgsEeUqDsmWjJpGbpWtKSL5tPV2c/Ky/+KR3hmQzuEwyKEKXjE4ZWOaRAIkl+NQXIv4uufvzosUHmLyqnLKzQs13wy68p9LSl51jnzA0bzDZ8qni9dPa7ZtQm+IczM+bz1l++7lovwzGl+4zSjHzgrt2HHesg2Mfw5Y9aF6F77oFrrimg9kceqXFOmZrrb3IuCH8yZq75xFtEFHJDmQlMpEhXewAlFTujLP/E6UOulGMhyZ3baLzmY/R1JNP1A0LbaY4vJsJ2mDUL1q3L+7McU4LLQiy77AnawzORgSDJZEoXmysd1kMdBC+pqWbo5FR9XpgxYYVAQJBMQG8bXHtWKONy62cPsmlrMJ3mOytBy5YSb5PhUERh9VuHXOtlOM7d2ad7Jj37IhQ/qPDcL6uMtyqK5p7Jo+GJNuV4r7/htRATnJzE6/t4jwGYY1nnny24cJTm99RJF1K9wqZMG5oCIQWzb/XCcWM4/50nmMk2NjBPSxyIR2igOYvQ1D1JIuMzJnSw/LL5hMtCENSaIOoyKd2tqBOmk+wodkSyumVQCwSueYXYgSOO155LvmRXGwA88K0qxlWE0trcIEyc5jy1zetKmDsvqPnR5wVpXueRdMHRh5qtzKVjSne2qJwtGNqxO27xMwdLVYvnyJzA4eZJcnTz55HKOFxF009U+BZvEZFrJdetrh1dWobam2snceSgQiik3fD/+lic8NTUuZxcAkMqPaXBvHs0I4iKSsj1czz3XzN9QJQI/3j5UwTCQaPoyuH9WiLFmHKV6VWZ7oXVG+P09SesRWqWnpMxplzlB91cEU6lGP97aWg4pjaNfCq1FVDVLXbBIpquvY2+aXOoaNvMS389wrbk5CFZvEOtdOa1EBP4Fq+PEYYuPRIiXQBHSs0iSSTgp9coxHamiG3XDhpv+BRd42o0GdTyLXkXaHFSidnqdwMQIEEdrVkznTzVgYhGYcMG4wMa+D2vrK3iUEwj20P7FN7+30kcfKuKn91oTYfVx9rTj6VITd/0OY5jytWNw01t0BhR2L8rTboP3aAMfwAon6IXeWqru3pV7lr5CD0zTkMqCnum13HWh8qo3bMZIRMoQhIaq3L+57ooC2sF79ety51TMcSEt2Ermn6iwlc1jADcrDEzGZgL4OjY0yH4z0+krK8JJTBuFF8978eaj1SkC7R4bTJ4xVWSRbeofDZVGW1NH/zrYxrB7+nQtQgwl00005A106mi4wh9VTPSlmgoCdgsXhtptFJH4oDCiw9r481mRen8ozepDARTVv+utoLKpLm1RA+PElxdH/LUkt4zTFZr7P0fpumux+lLhrwFSPPUX628t5vZSyamWxMFg+yvifDAw6ez7PInDX96aKxK4w3peyWXCsaD0MHHEOBbvCMAN1G92S8pUwVwSkpcLI2U1dQxcY4plTS/Ai3nXasa6bDBUCozayr80z0qwaBkXsk2tgXm0DLv00S2PZU106nxKx+lYkcrQlWp2NFK43WXWg6JHZFaJtuLA6xuep1Y9QzqaCUQkJnX5gCdfx68XjEK6lSUBWlcVGeMKWuWmM28X/XRw4YeeMrEIKqK8b7R41XDIH3uVcnTR9x9155gslqbrr2NvnjAvYiNHXZTMxi0bFHs19yx26E1UdtmAIs/3eleyeanj0Tgf56O860/HeKzvxjkoZ2HaN0dz38ufDjCJ94RgNs215wcML1aa+mycWP2bWC+/bPMMOtDzUqC8qmgqoKWI7OIJLbk3A7HDh7RMtVSPsX3XP/PnP/XH6Io0nBhNEVV+mbUadvfyGnc99s3+M15tzJ3rnuihxk6/+ztFPzX5SF+dWXmltW8oG3vVFn6te50MpVty171+QbDFRFSBF29ztllOat9eYHJarUnluTMKDMH0RRF01ab3A43P9hL9flhPrxsMtXnhymbEOT19XsN8o3vPUTjDZ8CoCYWTaegO9wrua51zWbVaPQZKguyZnNxiyudTPCJdwTgRpZOfslc7sChtHQPh9KlGI3kAfKPODfd/QctWULRMt9+fedarZRiQhhuyb7DGNYWQpAMjeKFH/3Ys6vTzD+z61UqzuniQ19u54NXdvHCqxoB6Ata6bgg7//0RC7+l4nc15Ky3LJs2bNll3nxXXe9GmXZlc+y8Mva/12v2lJnTVZrRdtm17Rvyzl1S/YOhWVLn6Rr92GNcPWBpq5h0lnjGTNBMaqjnbGwnMoywd//p5cta3tZXrGH8LhREAyyasv3qK0MuN4rua7V3F05EBCUjA1m3QkMR82lkwW+j3cE4JalVgi8ZnI54TNzFZqiWueHYMCamJEPzNl1Mhhk/LRguqNCiuMqRsMe84MsBH3J7Bl4Zpiz8T54ZTeBUq2GQ6BU5ca7unnmwSpqTlXY3qly1uJyg4zGT9Est+X2JBCTX8PN3wvauO1qDTtW3tVJe+lUZCBIe+lUVt61kwceNK0izc1w2mkwOEjj9Z9I1bGYQ0WZ4jrX5vq1hu/e4RrKJigIExmWTXC4H1ITVwU8kGWOc11rvD9hkK+uODBbx3YVizm5bkenyj/e0k3JuDwbbJ4k8GdiBDAUsnSDWa4zoSRV0GUwu3RHjzQX8hnm81aMFpbMt/1tKgECWnJBiuMaIwr3bVRJmgyjQrWcwVJrFw5RmnbVLP1at0G6oLlS+g6TNTqUbSFsjCgZ12xHR2l12ncaCNI7qdaQ11WMhg+W1/D9T/yRjnCEmliUVVc1UDXQlVWP5WiFO1xDuF8QG5SIgEAmJeGSwtUC6WvVknMar/0YjB1lSNiWzlEMd4OW6JJabHHeCZg3GadfrC2WZnfOcD8DxzN8HW8RUUx9oj212PhMsmhqh/AZ5vOmCVl7YN9zzQqueGd1RvvvfLSc2fDBK7sIlKqG9jd5SOGZB7WHOBqF+1rijJ+S9l+fMkzX74ZlVz5rWLwimeCDl1Uw+pQxxjwdPqDyzK93G6/XxrbxwFvXZZUSeE15Hq45tcBDKrAX3bb5NBd8qd1YLCF7JuHJqOP1Ld7jFE6kC4X1VvPyGebzWizns+ZCw58dC8bka2G74bbrJnHjXd2IUpXkIYXbrrNWKPtGdW4rdTix6rpqVt61k47SamoOdTK6otoyT6GyoMUi7iifmVOP5dUdNVxzaoEHCZuXnYDZQE8cUgiNdXbn+PCJd0QgxBAtEgdc3/Q6ldPrCASDhqUghCCZSNCzoxVx9vxh/YzhPO9Q8d5fZH/96pEZhoHrG6zzdHDvYZLJBIFAkGQyQX9sG2LmRXmd8+ffLtJgHfA2MBet91kC2JRIcHqOezbXHL/0WA3vWnI/Y8IR+mNR1jx0FT//dsfwDPgEgK9qOE7x4PWfoGdHK0lVZU/7VvZ0bCWpqvTsaOXB6z8x7J8xnOc90WCfpweu/SiHYtuQSZVDsW28ufaqoz3ErGgANgFq6v/hqFV++EAHLz58EX/5yUxefPgiDh/wSdcM38frw4cPH3nAr9Xgw4cPH8chiuLjFUI8DHrLV8JATEo53+G4HcABNNeSOtRVxIcPHz6OBxSFeKWUl+s/CyFuB/ZlOfxDUsreYozDhw8fPo5FFFXVILRw/qeBDxfzc3z48OHjeEKxfbwfAN6RUm5xeV0C64UQrwghRloF5MOHDx9HBQVbvEKIp4DJDi+tlFL+LvXzFcBvspzm/VLKTiHEJOBJIcQmKeUzLp93NSn5YG2tey8tHz58+DjWUTQ5mRBCATqBc6SUOz0cfzNwUEr5n7mO9eVkPnz4OFo41uVkC4FNbqQrhCgTQozTfwYWoSXR+PDhw8cJjWIS71JsbgYhRJUQYm3q11OB/xNCvAG8CPxRSvlEEcfjw4cPH8cEiqZqkFL+o8PfuoAlqZ+jwJnF+nwfPnz4OFbhZ6758OHDxwjDJ14fPnz4GGH4xOvDhw8fIwyfeH348OFjhOETrw8fPnyMMHzi9eHDh48Rhk+8Pnz48DHC8InXhw8fPkYYPvH68OHDxwjDJ14fPnz4GGH4xOvDhw8fIwyfeH348OFjhOETrw8fPnyMMHzi9eHDh48Rhk+8Pnz48DHC8InXhw8fPkYYPvH68OHDxwjDJ14fPnz4GGH4xOvDhw8fIwyfeH348OFjhOETrw8fPnyMMHzi9eHDh48Rhk+8Pnz48DHC8InXhw8fPkYYPvH68OHDxwjDJ14fPnz4GGH4xOvDhw8fI4whEa8QolEI0SKESAohzrW99k0hxFYhRKsQYrHL+2cIIV5IHfewEKJkKOPx4cOHj+MBQ7V43wY+CTxj/qMQYh6wFKgHLgZ+JIQIOrz/VuCHUspZwF7gi0Mcjw8fPnwc8xgS8UopN0opWx1eugRYI6U8IqXcDmwFFpgPEEII4MPAo6k/PQhcOpTx+PDhw8fxgGL5eKuBDtPvO1N/M+MUICalVLMc48OHDx8nHJRcBwghngImO7y0Ukr5u+Efkus4rgauTv16RAjx9kh9tgdMBHqP9iBM8MeTHf54ssMfT3bUDfUEOYlXSrmwgPN2AjWm36em/mbGHiAshFBSVq/TMeZx3AfcByCEeFlKea7bsSMNfzzZ4Y8nO/zxZMexOJ6hnqNYrobfA0uFEKOEEDOA2cCL5gOklBL4M3BZ6k9XAiNmQfvw4cPH0cJQ5WSfEELsBN4H/FEIsQ5AStkCPAJsAJ4ArpFSJlLvWSuEqEqd4uvADUKIrWg+358NZTw+fPjwcTwgp6shG6SUjwGPuby2Cljl8Pclpp+j2NQOHnFfAe8pJvzxZIc/nuzwx5MdJ9x4hLbj9+HDhw8fIwU/ZdiHDx8+RhjHLPEey+nIqfO9nvq3QwjxustxO4QQb6WOG3IkNMt4bhZCdJrGtMTluItTc7ZVCPGNIo7nNiHEJiHEm0KIx4QQYZfjijY/ua41Ffh9OPX6C0KI6cP5+bbPqhFC/FkIsSF1T1/ncMwFQoh9pu/w28Uaj+kzs86/0PBfqTl6UwhxdhHHUme69teFEPuFENfbjinqHAkh7hdCdJulqkKICiHEk0KILan/y13ee2XqmC1CiCtzfpiU8pj8B5yGppf7C3Cu6e/zgDeAUcAMYBsQdHj/I8DS1M8/BlYUaZy3A992eW0HMHEE5upm4F9zHBNMzVUEKEnN4bwijWcRoKR+vhW4dSTnx8u1Al8Bfpz6eSnwcBG/nynA2amfxwGbHcZzAfCHYt8r+cw/sAT4X0AA7wVeGKFxBYHdwLSRnCPgg8DZwNumv/0A+Ebq52843ctABRBN/V+e+rk822cdsxavPA7SkVOf82ngN8N97iJgAbBVShmVUg4Ca9DmctghpVwv0xmJf0fTaI8kvFzrJWj3BWj3yYWp73PYIaXcJaV8NfXzAWAjx0eW5iXAL6SGv6Pp7qeMwOdeCGyTUraNwGcZkFI+A/TZ/my+T9x4ZDHwpJSyT0q5F3gSrUaNK45Z4s2CYykd+QPAO1LKLS6vS2C9EOKVVOZdMXFtajt4v8t2yMu8FQNXoVlNTijW/Hi5VuOY1H2yD+2+KSpSLo2zgBccXn6fEOINIcT/CiHqiz0Wcs//0bpnluJuzIz0HJ0qpdyV+nk3cKrDMXnP05DkZEOFOEbSkZ3gcWxXkN3afb+UslMIMQl4UgixKbWqDut4gHuB76I9SN9Fc39cVcjnDMd49PkRQqwEVOBXLqcZtvk5HiCEGAv8FrheSrnf9vKraFvrgykf/eNoiUfFxDE3/6lYzMeBbzq8fDTmyICUUgohhkUGdlSJVx4j6ciFjE0IoaCVxDwnyzk6U/93CyEeQ9sCF3Rje50rIcRq4A8OL3mZt2EbjxDiH4GPARfKlCPM4RzDNj82eLlW/Zidqe9yAtp9UxQIIUJopPsrKeX/2F83E7GUcq0Q4kdCiIlSyqLVKPAw/8N6z3jER4BXpZTv2F84GnMEvCOEmCKl3JVys3Q7HNOJ5n/WMRUtNuWK49HVcKykIy8ENkkpdzq9KIQoE0KM039GCzgVpbCPze/2CZfPeQmYLTS1Rwnadu73RRrPxcC/AR+XUg64HFPM+fFyrb9Huy9Au0/+5LZADBUp3/HPgI1Syjtcjpms+5iFEAvQns1iLgRe5v/3wBdS6ob3AvtM2+5iwXUXOdJzlIL5PnHjkXXAIiFEecrNtyj1N3cUK0I4DBHGT6D5So4A7wDrTK+tRItatwIfMf19LVCV+jmCRshbgSZg1DCP7+fAl21/qwLWmj7/jdS/FrQteLHm6iHgLeDN1I0yxT6e1O9L0CLq24o8nq1oPq/XU/9+bB9PsefH6VqB76AtBgCjU/fF1tR9EinifLwfzQ30pmlOlgBf1u8h4NrUPLyBFpA8r1jjyTb/tjEJ4J7UHL6FSV1UpDGVoRHpBNPfRmyO0Ah/FxBPcc8X0fz+TwNbgKeAitSx5wI/Nb33qtS9tBVYluuz/Mw1Hz58+BhhHI+uBh8+fPg4ruETrw8fPnyMMHzi9eHDh48Rhk+8Pnz48DHC8InXhw8fPkYYPvH68OHDxwjDJ14fPnz4GGH4xOvDhw8fI4z/HxsjRR8r4bbzAAAAAElFTkSuQmCC
"
>
</div>

</div>

<div class="output_area">

    <div class="prompt"></div>




<div class="output_png output_subarea ">
<img src="data:image/png;base64,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
"
>
</div>

</div>

<div class="output_area">

    <div class="prompt"></div>




<div class="output_png output_subarea ">
<img src="data:image/png;base64,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
"
>
</div>

</div>

<div class="output_area">

    <div class="prompt"></div>




<div class="output_png output_subarea ">
<img src="data:image/png;base64,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
"
>
</div>

</div>

<div class="output_area">

    <div class="prompt"></div>




<div class="output_png output_subarea ">
<img src="data:image/png;base64,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
"
>
</div>

</div>

<div class="output_area">

    <div class="prompt"></div>




<div class="output_png output_subarea ">
<img src="data:image/png;base64,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
"
>
</div>

</div>

<div class="output_area">

    <div class="prompt"></div>




<div class="output_png output_subarea ">
<img src="data:image/png;base64,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
"
>
</div>

</div>

<div class="output_area">

    <div class="prompt"></div>




<div class="output_png output_subarea ">
<img src="data:image/png;base64,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
"
>
</div>

</div>

<div class="output_area">

    <div class="prompt"></div>




<div class="output_png output_subarea ">
<img src="data:image/png;base64,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
"
>
</div>

</div>

<div class="output_area">

    <div class="prompt"></div>




<div class="output_png output_subarea ">
<img src="data:image/png;base64,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
"
>
</div>

</div>

</div>
</div>

</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[9]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">m1_iterated_elo</span> <span class="o">=</span> <span class="n">findAverage</span><span class="p">(</span><span class="n">m_elo</span><span class="p">[</span><span class="mi">0</span><span class="p">])</span>
<span class="n">m1_iterated_likes</span> <span class="o">=</span> <span class="n">findAverage</span><span class="p">(</span><span class="n">m_likes</span><span class="p">[</span><span class="mi">0</span><span class="p">])</span>
<span class="n">m2_iterated_elo</span> <span class="o">=</span> <span class="n">findAverage</span><span class="p">(</span><span class="n">m_elo</span><span class="p">[</span><span class="mi">1</span><span class="p">])</span>
<span class="n">m2_iterated_likes</span> <span class="o">=</span> <span class="n">findAverage</span><span class="p">(</span><span class="n">m_likes</span><span class="p">[</span><span class="mi">1</span><span class="p">])</span>
<span class="n">m3_iterated_elo</span> <span class="o">=</span> <span class="n">findAverage</span><span class="p">(</span><span class="n">m_elo</span><span class="p">[</span><span class="mi">2</span><span class="p">])</span>
<span class="n">m3_iterated_likes</span> <span class="o">=</span> <span class="n">findAverage</span><span class="p">(</span><span class="n">m_likes</span><span class="p">[</span><span class="mi">2</span><span class="p">])</span>
<span class="n">f_iterated_elo</span> <span class="o">=</span> <span class="n">findAverage</span><span class="p">(</span><span class="n">f_elo</span><span class="p">)</span>
<span class="n">f_iterated_likes</span> <span class="o">=</span> <span class="n">findAverage</span><span class="p">(</span><span class="n">f_likes</span><span class="p">)</span>
</pre></div>

    </div>
</div>
</div>

</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[10]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">box</span><span class="o">.</span><span class="n">plotDistributions</span><span class="p">()</span>
</pre></div>

    </div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area">

    <div class="prompt"></div>




<div class="output_png output_subarea ">
<img src="data:image/png;base64,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
"
>
</div>

</div>

</div>
</div>

</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[11]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">m_elosum</span> <span class="o">=</span> <span class="p">[</span><span class="mi">0</span><span class="p">,</span><span class="mi">0</span><span class="p">,</span><span class="mi">0</span><span class="p">]</span>
<span class="n">m_ratingsum</span> <span class="o">=</span> <span class="p">[</span><span class="mi">0</span><span class="p">,</span><span class="mi">0</span><span class="p">,</span><span class="mi">0</span><span class="p">]</span>
<span class="n">f_elosum</span> <span class="o">=</span> <span class="mi">0</span>
<span class="n">f_ratingsum</span> <span class="o">=</span> <span class="mi">0</span>
<span class="k">for</span> <span class="n">i</span> <span class="ow">in</span> <span class="nb">range</span><span class="p">(</span><span class="mi">0</span><span class="p">,</span> <span class="nb">sum</span><span class="p">(</span><span class="n">m</span><span class="p">)</span><span class="o">+</span><span class="n">f</span><span class="p">):</span>
    <span class="k">if</span> <span class="n">i</span> <span class="o">&lt;</span> <span class="n">m</span><span class="p">[</span><span class="mi">0</span><span class="p">]:</span>
        <span class="n">m_elosum</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span> <span class="o">+=</span> <span class="n">box</span><span class="o">.</span><span class="n">particles</span><span class="p">[</span><span class="n">i</span><span class="p">]</span><span class="o">.</span><span class="n">elo</span>
        <span class="n">m_ratingsum</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span> <span class="o">+=</span> <span class="n">box</span><span class="o">.</span><span class="n">particles</span><span class="p">[</span><span class="n">i</span><span class="p">]</span><span class="o">.</span><span class="n">rating</span>
    <span class="k">elif</span> <span class="n">i</span> <span class="o">&lt;</span> <span class="n">m</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span> <span class="o">+</span> <span class="n">m</span><span class="p">[</span><span class="mi">1</span><span class="p">]:</span>
        <span class="n">m_elosum</span><span class="p">[</span><span class="mi">1</span><span class="p">]</span> <span class="o">+=</span> <span class="n">box</span><span class="o">.</span><span class="n">particles</span><span class="p">[</span><span class="n">i</span><span class="p">]</span><span class="o">.</span><span class="n">elo</span>
        <span class="n">m_ratingsum</span><span class="p">[</span><span class="mi">1</span><span class="p">]</span> <span class="o">+=</span> <span class="n">box</span><span class="o">.</span><span class="n">particles</span><span class="p">[</span><span class="n">i</span><span class="p">]</span><span class="o">.</span><span class="n">rating</span>
    <span class="k">elif</span> <span class="n">i</span> <span class="o">&lt;</span> <span class="n">m</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span> <span class="o">+</span> <span class="n">m</span><span class="p">[</span><span class="mi">1</span><span class="p">]</span> <span class="o">+</span> <span class="n">m</span><span class="p">[</span><span class="mi">2</span><span class="p">]:</span>
        <span class="n">m_elosum</span><span class="p">[</span><span class="mi">2</span><span class="p">]</span> <span class="o">+=</span> <span class="n">box</span><span class="o">.</span><span class="n">particles</span><span class="p">[</span><span class="n">i</span><span class="p">]</span><span class="o">.</span><span class="n">elo</span>
        <span class="n">m_ratingsum</span><span class="p">[</span><span class="mi">2</span><span class="p">]</span> <span class="o">+=</span> <span class="n">box</span><span class="o">.</span><span class="n">particles</span><span class="p">[</span><span class="n">i</span><span class="p">]</span><span class="o">.</span><span class="n">rating</span>
    <span class="k">else</span><span class="p">:</span>
        <span class="n">f_elosum</span> <span class="o">+=</span> <span class="n">box</span><span class="o">.</span><span class="n">particles</span><span class="p">[</span><span class="n">i</span><span class="p">]</span><span class="o">.</span><span class="n">elo</span>
        <span class="n">f_ratingsum</span> <span class="o">+=</span> <span class="n">box</span><span class="o">.</span><span class="n">particles</span><span class="p">[</span><span class="n">i</span><span class="p">]</span><span class="o">.</span><span class="n">rating</span>
    
<span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Standard Elo avg = &quot;</span> <span class="o">+</span> <span class="nb">str</span><span class="p">(</span><span class="n">m_elosum</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span> <span class="o">/</span> <span class="n">m</span><span class="p">[</span><span class="mi">0</span><span class="p">]))</span>
<span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Standard Rating avg = &quot;</span> <span class="o">+</span> <span class="nb">str</span><span class="p">(</span><span class="n">m_ratingsum</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span> <span class="o">/</span> <span class="n">m</span><span class="p">[</span><span class="mi">0</span><span class="p">]))</span>
<span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Half Elo avg = &quot;</span> <span class="o">+</span> <span class="nb">str</span><span class="p">(</span><span class="n">m_elosum</span><span class="p">[</span><span class="mi">1</span><span class="p">]</span> <span class="o">/</span> <span class="n">m</span><span class="p">[</span><span class="mi">1</span><span class="p">]))</span>
<span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Half Rating avg = &quot;</span> <span class="o">+</span> <span class="nb">str</span><span class="p">(</span><span class="n">m_ratingsum</span><span class="p">[</span><span class="mi">1</span><span class="p">]</span> <span class="o">/</span> <span class="n">m</span><span class="p">[</span><span class="mi">1</span><span class="p">]))</span>
<span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Allright Elo avg = &quot;</span> <span class="o">+</span> <span class="nb">str</span><span class="p">(</span><span class="n">m_elosum</span><span class="p">[</span><span class="mi">2</span><span class="p">]</span> <span class="o">/</span> <span class="n">m</span><span class="p">[</span><span class="mi">2</span><span class="p">]))</span>
<span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Allright Rating avg = &quot;</span> <span class="o">+</span> <span class="nb">str</span><span class="p">(</span><span class="n">m_ratingsum</span><span class="p">[</span><span class="mi">2</span><span class="p">]</span> <span class="o">/</span> <span class="n">m</span><span class="p">[</span><span class="mi">2</span><span class="p">]))</span>
<span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Female Elo avg = &quot;</span> <span class="o">+</span> <span class="nb">str</span><span class="p">(</span><span class="n">f_elosum</span> <span class="o">/</span> <span class="n">f</span><span class="p">))</span>
<span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Female Rating avg = &quot;</span> <span class="o">+</span> <span class="nb">str</span><span class="p">(</span><span class="n">f_ratingsum</span> <span class="o">/</span> <span class="n">f</span><span class="p">))</span>
</pre></div>

    </div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area">

    <div class="prompt"></div>


<div class="output_subarea output_stream output_stdout output_text">
<pre>Standard Elo avg = 1168.5324524984005
Standard Rating avg = 1188.465058593969
Half Elo avg = 1171.7371849446113
Half Rating avg = 1196.8357590554174
Allright Elo avg = 1074.2198687294606
Allright Rating avg = 1191.4079152906065
Female Elo avg = 1354.7586897278675
Female Rating avg = 1202.8271960384857
</pre>
</div>
</div>

</div>
</div>

</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[12]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">outperformance</span> <span class="o">=</span> <span class="mi">0</span>
<span class="n">matches</span> <span class="o">=</span> <span class="mi">0</span>
<span class="k">for</span> <span class="n">i</span> <span class="ow">in</span> <span class="nb">range</span><span class="p">(</span><span class="mi">0</span><span class="p">,</span> <span class="n">m</span><span class="p">[</span><span class="mi">0</span><span class="p">]):</span>
    <span class="k">for</span> <span class="n">right</span> <span class="ow">in</span> <span class="n">box</span><span class="o">.</span><span class="n">particles</span><span class="p">[</span><span class="n">i</span><span class="p">]</span><span class="o">.</span><span class="n">right</span><span class="o">.</span><span class="n">keys</span><span class="p">():</span>
        <span class="k">if</span> <span class="n">i</span> <span class="ow">in</span> <span class="n">box</span><span class="o">.</span><span class="n">particles</span><span class="p">[</span><span class="n">right</span><span class="p">]</span><span class="o">.</span><span class="n">right</span><span class="p">:</span>
            <span class="n">outperformance</span> <span class="o">+=</span> <span class="p">(</span><span class="n">box</span><span class="o">.</span><span class="n">particles</span><span class="p">[</span><span class="n">right</span><span class="p">]</span><span class="o">.</span><span class="n">rating</span> <span class="o">-</span> <span class="n">box</span><span class="o">.</span><span class="n">particles</span><span class="p">[</span><span class="n">i</span><span class="p">]</span><span class="o">.</span><span class="n">rating</span><span class="p">)</span>
            <span class="n">matches</span> <span class="o">+=</span> <span class="mi">1</span>
<span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Average match outperformance for standard (adjusted for rating delta): &quot;</span> <span class="o">+</span> <span class="nb">str</span><span class="p">(</span><span class="n">outperformance</span><span class="o">/</span><span class="n">matches</span> <span class="o">-</span> <span class="p">(</span><span class="n">f_ratingsum</span><span class="o">/</span><span class="n">f</span> <span class="o">-</span> <span class="n">m_ratingsum</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span><span class="o">/</span><span class="n">m</span><span class="p">[</span><span class="mi">0</span><span class="p">])))</span>
<span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Average matches for standard: &quot;</span> <span class="o">+</span> <span class="nb">str</span><span class="p">(</span><span class="n">matches</span><span class="o">/</span><span class="n">m</span><span class="p">[</span><span class="mi">0</span><span class="p">]))</span>

<span class="n">outperformance</span> <span class="o">=</span> <span class="mi">0</span>
<span class="n">matches</span> <span class="o">=</span> <span class="mi">0</span>
<span class="k">for</span> <span class="n">i</span> <span class="ow">in</span> <span class="nb">range</span><span class="p">(</span><span class="n">m</span><span class="p">[</span><span class="mi">0</span><span class="p">],</span> <span class="n">m</span><span class="p">[</span><span class="mi">1</span><span class="p">]</span> <span class="o">+</span> <span class="n">m</span><span class="p">[</span><span class="mi">2</span><span class="p">]):</span>
    <span class="k">for</span> <span class="n">right</span> <span class="ow">in</span> <span class="n">box</span><span class="o">.</span><span class="n">particles</span><span class="p">[</span><span class="n">i</span><span class="p">]</span><span class="o">.</span><span class="n">right</span><span class="o">.</span><span class="n">keys</span><span class="p">():</span>
        <span class="k">if</span> <span class="n">i</span> <span class="ow">in</span> <span class="n">box</span><span class="o">.</span><span class="n">particles</span><span class="p">[</span><span class="n">right</span><span class="p">]</span><span class="o">.</span><span class="n">right</span><span class="p">:</span>
            <span class="n">outperformance</span> <span class="o">+=</span> <span class="p">(</span><span class="n">box</span><span class="o">.</span><span class="n">particles</span><span class="p">[</span><span class="n">right</span><span class="p">]</span><span class="o">.</span><span class="n">rating</span> <span class="o">-</span> <span class="n">box</span><span class="o">.</span><span class="n">particles</span><span class="p">[</span><span class="n">i</span><span class="p">]</span><span class="o">.</span><span class="n">rating</span><span class="p">)</span>
            <span class="n">matches</span> <span class="o">+=</span> <span class="mi">1</span>
<span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Average match outperformance for half (adjusted for rating delta): &quot;</span> <span class="o">+</span> <span class="nb">str</span><span class="p">(</span><span class="n">outperformance</span><span class="o">/</span><span class="n">matches</span> <span class="o">-</span> <span class="p">(</span><span class="n">f_ratingsum</span><span class="o">/</span><span class="n">f</span> <span class="o">-</span> <span class="n">m_ratingsum</span><span class="p">[</span><span class="mi">1</span><span class="p">]</span><span class="o">/</span><span class="n">m</span><span class="p">[</span><span class="mi">1</span><span class="p">])))</span>
<span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Average matches for half: &quot;</span> <span class="o">+</span> <span class="nb">str</span><span class="p">(</span><span class="n">matches</span><span class="o">/</span><span class="n">m</span><span class="p">[</span><span class="mi">1</span><span class="p">]))</span>

<span class="n">outperformance</span> <span class="o">=</span> <span class="mi">0</span>
<span class="n">matches</span> <span class="o">=</span> <span class="mi">0</span>
<span class="k">for</span> <span class="n">i</span> <span class="ow">in</span> <span class="nb">range</span><span class="p">(</span><span class="n">m</span><span class="p">[</span><span class="mi">0</span><span class="p">]</span> <span class="o">+</span> <span class="n">m</span><span class="p">[</span><span class="mi">1</span><span class="p">],</span> <span class="nb">sum</span><span class="p">(</span><span class="n">m</span><span class="p">)):</span>
    <span class="k">for</span> <span class="n">right</span> <span class="ow">in</span> <span class="n">box</span><span class="o">.</span><span class="n">particles</span><span class="p">[</span><span class="n">i</span><span class="p">]</span><span class="o">.</span><span class="n">right</span><span class="o">.</span><span class="n">keys</span><span class="p">():</span>
        <span class="k">if</span> <span class="n">i</span> <span class="ow">in</span> <span class="n">box</span><span class="o">.</span><span class="n">particles</span><span class="p">[</span><span class="n">right</span><span class="p">]</span><span class="o">.</span><span class="n">right</span><span class="p">:</span>
            <span class="n">outperformance</span> <span class="o">+=</span> <span class="p">(</span><span class="n">box</span><span class="o">.</span><span class="n">particles</span><span class="p">[</span><span class="n">right</span><span class="p">]</span><span class="o">.</span><span class="n">rating</span> <span class="o">-</span> <span class="n">box</span><span class="o">.</span><span class="n">particles</span><span class="p">[</span><span class="n">i</span><span class="p">]</span><span class="o">.</span><span class="n">rating</span><span class="p">)</span>
            <span class="n">matches</span> <span class="o">+=</span> <span class="mi">1</span>
<span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Average match outperformance for allright (adjusted for rating delta): &quot;</span> <span class="o">+</span> <span class="nb">str</span><span class="p">(</span><span class="n">outperformance</span><span class="o">/</span><span class="n">matches</span> <span class="o">-</span> <span class="p">(</span><span class="n">f_ratingsum</span><span class="o">/</span><span class="n">f</span> <span class="o">-</span> <span class="n">m_ratingsum</span><span class="p">[</span><span class="mi">2</span><span class="p">]</span><span class="o">/</span><span class="n">m</span><span class="p">[</span><span class="mi">2</span><span class="p">])))</span>
<span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Average matches for allright: &quot;</span> <span class="o">+</span> <span class="nb">str</span><span class="p">(</span><span class="n">matches</span><span class="o">/</span><span class="n">m</span><span class="p">[</span><span class="mi">2</span><span class="p">]))</span>

<span class="n">outperformance</span> <span class="o">=</span> <span class="mi">0</span>
<span class="n">matches</span> <span class="o">=</span> <span class="mi">0</span>
<span class="k">for</span> <span class="n">i</span> <span class="ow">in</span> <span class="nb">range</span><span class="p">(</span><span class="nb">sum</span><span class="p">(</span><span class="n">m</span><span class="p">),</span> <span class="n">f</span><span class="o">+</span><span class="nb">sum</span><span class="p">(</span><span class="n">m</span><span class="p">)):</span>
    <span class="k">for</span> <span class="n">right</span> <span class="ow">in</span> <span class="n">box</span><span class="o">.</span><span class="n">particles</span><span class="p">[</span><span class="n">i</span><span class="p">]</span><span class="o">.</span><span class="n">right</span><span class="o">.</span><span class="n">keys</span><span class="p">():</span>
        <span class="k">if</span> <span class="n">i</span> <span class="ow">in</span> <span class="n">box</span><span class="o">.</span><span class="n">particles</span><span class="p">[</span><span class="n">right</span><span class="p">]</span><span class="o">.</span><span class="n">right</span><span class="p">:</span>
            <span class="n">outperformance</span> <span class="o">+=</span> <span class="p">(</span><span class="n">box</span><span class="o">.</span><span class="n">particles</span><span class="p">[</span><span class="n">right</span><span class="p">]</span><span class="o">.</span><span class="n">rating</span> <span class="o">-</span> <span class="n">box</span><span class="o">.</span><span class="n">particles</span><span class="p">[</span><span class="n">i</span><span class="p">]</span><span class="o">.</span><span class="n">rating</span><span class="p">)</span>
            <span class="n">matches</span> <span class="o">+=</span> <span class="mi">1</span>
<span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Average outperformance in matches for females (adjusted for rating delta): &quot;</span> <span class="o">+</span> <span class="nb">str</span><span class="p">(</span><span class="n">outperformance</span><span class="o">/</span><span class="n">matches</span> <span class="o">-</span> <span class="p">(</span><span class="nb">sum</span><span class="p">(</span><span class="n">m_ratingsum</span><span class="p">)</span><span class="o">/</span><span class="nb">sum</span><span class="p">(</span><span class="n">m</span><span class="p">)</span> <span class="o">-</span> <span class="n">f_ratingsum</span><span class="o">/</span><span class="n">f</span><span class="p">)))</span>
<span class="nb">print</span><span class="p">(</span><span class="s2">&quot;Average matches for females: &quot;</span> <span class="o">+</span> <span class="nb">str</span><span class="p">(</span><span class="n">matches</span><span class="o">/</span><span class="n">f</span><span class="p">))</span>
</pre></div>

    </div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area">

    <div class="prompt"></div>


<div class="output_subarea output_stream output_stdout output_text">
<pre>Average match outperformance for standard (adjusted for rating delta): -21.927480472907437
Average matches for standard: 1.3666666666666667
Average match outperformance for half (adjusted for rating delta): -167.8954769804142
Average matches for half: 2.283333333333333
Average match outperformance for allright (adjusted for rating delta): -188.5111011925627
Average matches for allright: 4.42
Average outperformance in matches for females (adjusted for rating delta): 154.67596285670035
Average matches for females: 8.07
</pre>
</div>
</div>

</div>
</div>

</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[26]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">elodf</span> <span class="o">=</span> <span class="n">pd</span><span class="o">.</span><span class="n">DataFrame</span><span class="p">(</span>
    <span class="p">{</span><span class="s1">&#39;Standard Elo&#39;</span><span class="p">:</span> <span class="n">m1_iterated_elo</span><span class="p">,</span>
     <span class="s1">&#39;Half Elo&#39;</span><span class="p">:</span> <span class="n">m2_iterated_elo</span><span class="p">,</span>
     <span class="s1">&#39;Allright Elo&#39;</span><span class="p">:</span> <span class="n">m3_iterated_elo</span>
     <span class="c1">#&#39;Female Elo&#39;: f_iterated_elo,</span>
    <span class="p">})</span>
<span class="n">elodf</span> <span class="o">=</span> <span class="n">elodf</span><span class="o">.</span><span class="n">transpose</span><span class="p">()</span>

<span class="n">likedf</span> <span class="o">=</span> <span class="n">pd</span><span class="o">.</span><span class="n">DataFrame</span><span class="p">(</span>
    <span class="p">{</span><span class="s1">&#39;Standard Elo&#39;</span><span class="p">:</span> <span class="n">m1_iterated_likes</span><span class="p">,</span>
     <span class="s1">&#39;Half Elo&#39;</span><span class="p">:</span> <span class="n">m2_iterated_likes</span><span class="p">,</span>
     <span class="s1">&#39;Allright Elo&#39;</span><span class="p">:</span> <span class="n">m3_iterated_likes</span>
     <span class="c1">#&#39;Female Elo&#39;: f_iterated_likes,</span>
    <span class="p">})</span>
<span class="n">likedf</span> <span class="o">=</span> <span class="n">likedf</span><span class="o">.</span><span class="n">transpose</span><span class="p">()</span>
</pre></div>

    </div>
</div>
</div>

</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[27]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">elodf</span><span class="o">.</span><span class="n">to_csv</span><span class="p">(</span><span class="s1">&#39;elo.csv&#39;</span><span class="p">)</span>
<span class="n">likedf</span><span class="o">.</span><span class="n">to_csv</span><span class="p">(</span><span class="s1">&#39;likedf.csv&#39;</span><span class="p">)</span>
</pre></div>

    </div>
</div>
</div>

</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[24]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">elodf</span><span class="o">.</span><span class="n">T</span><span class="o">.</span><span class="n">plot</span><span class="p">()</span>
</pre></div>

    </div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area">

    <div class="prompt output_prompt">Out[24]:</div>




<div class="output_text output_subarea output_execute_result">
<pre>&lt;AxesSubplot:&gt;</pre>
</div>

</div>

<div class="output_area">

    <div class="prompt"></div>




<div class="output_png output_subarea ">
<img src="data:image/png;base64,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
"
>
</div>

</div>

</div>
</div>

</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[25]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span><span class="n">likedf</span><span class="o">.</span><span class="n">T</span><span class="o">.</span><span class="n">plot</span><span class="p">()</span>
</pre></div>

    </div>
</div>
</div>

<div class="output_wrapper">
<div class="output">


<div class="output_area">

    <div class="prompt output_prompt">Out[25]:</div>




<div class="output_text output_subarea output_execute_result">
<pre>&lt;AxesSubplot:&gt;</pre>
</div>

</div>

<div class="output_area">

    <div class="prompt"></div>




<div class="output_png output_subarea ">
<img src="data:image/png;base64,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
"
>
</div>

</div>

</div>
</div>

</div>
<div class="cell border-box-sizing code_cell rendered">
<div class="input">
<div class="prompt input_prompt">In&nbsp;[&nbsp;]:</div>
<div class="inner_cell">
    <div class="input_area">
<div class=" highlight hl-ipython3"><pre><span></span> 
</pre></div>

    </div>
</div>
</div>

</div>
    </div>
  </div>
</body>
```
