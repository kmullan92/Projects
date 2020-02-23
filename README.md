# Pure-CSS-Image-Modal-with-Overlay

<blockquote>
<p>simple pure css image modal with overlay hover effect</p>
</blockquote>
Demo: https://jsfiddle.net/cuqj0x96/11/
<p></P>
<pre><span>&lt;!DOCTYPE html&gt;
&lt;html&gt;
&lt;head&gt;
&lt;style&gt;
body {font-family: Arial, Helvetica, sans-serif;}

.thumbnail {
    max-width: 100%;
    display: inline-block!important;
}

.italic { font-style: italic; }
.small { font-size: 0.8em; }

/** LIGHTBOX MARKUP **/

.lightbox {
	/** Default lightbox to hidden */
	display: none;

	/** Position and style */
	position: fixed;
	z-index: 999;
	width: 100%;
	height: 100%;
	text-align: center;
	top: 0;
	left: 0;
	background: rgba(0,0,0,0.8);
}

.lightbox img {
		/** Pad the lightbox image */
    max-width: 60%;
    max-height: 100%;
    margin-top: 2%;
    display: inline-block!important;
}

.lightbox:target {
	/** Remove default browser outline */
	outline: none;

	/** Unhide lightbox **/
	display: block;
}

	/** Porfolio box hover **/
.container{
  padding: 1em 0;
  float: left;
  width: 50%;
}
@media screen and (max-width: 640px){
  .container{
    display: block;
    width: 100%;
  }
}

@media screen and (min-width: 900px){
  .container{
    width: 33.33333%;
  }
}

.container .title{
  color: #1a1a1a;
  text-align: center;
  margin-bottom: 10px;
}

.content {
  position: relative;
  width: 90%;
  max-width: 400px;
  margin: auto;
  overflow: hidden;
}

.content .content-overlay {
  background: rgba(0,0,0,0.7);
  position: absolute;
  height: 98%;
  width: 100%;
  left: 0;
  top: 0;
  bottom: 0;
  right: 0;
  opacity: 0;
  -webkit-transition: all 0.4s ease-in-out 0s;
  -moz-transition: all 0.4s ease-in-out 0s;
  transition: all 0.4s ease-in-out 0s;
}

.content:hover .content-overlay{
  opacity: 1;
}

.content-image{
  width: 100%;
}

.content-details {
  position: absolute;
  text-align: center;
  padding-left: 1em;
  padding-right: 1em;
  width: 100%;
  top: 50%;
  left: 50%;
  opacity: 0;
  -webkit-transform: translate(-50%, -50%);
  -moz-transform: translate(-50%, -50%);
  transform: translate(-50%, -50%);
  -webkit-transition: all 0.3s ease-in-out 0s;
  -moz-transition: all 0.3s ease-in-out 0s;
  transition: all 0.3s ease-in-out 0s;
}

.content:hover .content-details{
  top: 50%;
  left: 50%;
  opacity: 1;
}

.content-details h3 {
    color: #fff;
    font-weight: 500;
    letter-spacing: 0.15em;
    margin-bottom: 0.5em;
    text-transform: uppercase;
    font-family: sans-serif;
}

.content-details p{
  color: #fff;
  font-size: 0.8em;
}

.fadeIn-bottom{
  top: 60%;
}
&lt;/style&gt;
&lt;/head&gt;
&lt;body&gt;

&lt;div class="container"&gt;

&lt;div class="content"&gt;
    &lt;a href="#img1"&gt;
&lt;div class="content-overlay"&gt;&lt;/div&gt;
&lt;img class="content-image" src="https://kylemullan.co.uk/wp-content/uploads/2020/02/tim-stief-YFFGkE3y4F8-unsplash-1.jpg"/&gt;
&lt;div class="content-details fadeIn-bottom"&gt;
&lt;h3 class="content-title"&gt;Click to expand&lt;/h3&gt;
&lt;/div&gt;
&lt;a href="#_" class="lightbox" id="img1"&gt;&lt;br /&gt;
  &lt;img src="https://kylemullan.co.uk/wp-content/uploads/2020/02/tim-stief-YFFGkE3y4F8-unsplash-1.jpg"/&gt;
&lt;/a&gt;

&lt;/body&gt;

<!DOCTYPE html>
<html>
<head>
<style>
body {font-family: Arial, Helvetica, sans-serif;}

.thumbnail {
    max-width: 100%;
    display: inline-block!important;
}

.italic { font-style: italic; }
.small { font-size: 0.8em; }

/** LIGHTBOX MARKUP **/

.lightbox {
	/** Default lightbox to hidden */
	display: none;

	/** Position and style */
	position: fixed;
	z-index: 999;
	width: 100%;
	height: 100%;
	text-align: center;
	top: 0;
	left: 0;
	background: rgba(0,0,0,0.8);
}

.lightbox img {
		/** Pad the lightbox image */
    max-width: 60%;
    max-height: 100%;
    margin-top: 2%;
    display: inline-block!important;
}

.lightbox:target {
	/** Remove default browser outline */
	outline: none;

	/** Unhide lightbox **/
	display: block;
}

	/** Porfolio box hover **/
.container{
  padding: 1em 0;
  float: left;
  width: 50%;
}
@media screen and (max-width: 640px){
  .container{
    display: block;
    width: 100%;
  }
}

@media screen and (min-width: 900px){
  .container{
    width: 33.33333%;
  }
}

.container .title{
  color: #1a1a1a;
  text-align: center;
  margin-bottom: 10px;
}

.content {
  position: relative;
  width: 90%;
  max-width: 400px;
  margin: auto;
  overflow: hidden;
}

.content .content-overlay {
  background: rgba(0,0,0,0.7);
  position: absolute;
  height: 98%;
  width: 100%;
  left: 0;
  top: 0;
  bottom: 0;
  right: 0;
  opacity: 0;
  -webkit-transition: all 0.4s ease-in-out 0s;
  -moz-transition: all 0.4s ease-in-out 0s;
  transition: all 0.4s ease-in-out 0s;
}

.content:hover .content-overlay{
  opacity: 1;
}

.content-image{
  width: 100%;
}

.content-details {
  position: absolute;
  text-align: center;
  padding-left: 1em;
  padding-right: 1em;
  width: 100%;
  top: 50%;
  left: 50%;
  opacity: 0;
  -webkit-transform: translate(-50%, -50%);
  -moz-transform: translate(-50%, -50%);
  transform: translate(-50%, -50%);
  -webkit-transition: all 0.3s ease-in-out 0s;
  -moz-transition: all 0.3s ease-in-out 0s;
  transition: all 0.3s ease-in-out 0s;
}

.content:hover .content-details{
  top: 50%;
  left: 50%;
  opacity: 1;
}

.content-details h3 {
    color: #fff;
    font-weight: 500;
    letter-spacing: 0.15em;
    margin-bottom: 0.5em;
    text-transform: uppercase;
    font-family: sans-serif;
}

.content-details p{
  color: #fff;
  font-size: 0.8em;
}

.fadeIn-bottom{
  top: 60%;
}
</style>
</head>
<body>

<div class="container">

<div class="content">
    <a href="#img1">
<div class="content-overlay"></div>
<img class="content-image" src="https://kylemullan.co.uk/wp-content/uploads/2020/02/tim-stief-YFFGkE3y4F8-unsplash-1.jpg"/>
<div class="content-details fadeIn-bottom">
<h3 class="content-title">Click to expand</h3>
</div>
<a href="#_" class="lightbox" id="img1"><br />
  <img src="https://kylemullan.co.uk/wp-content/uploads/2020/02/tim-stief-YFFGkE3y4F8-unsplash-1.jpg"/>
</a>

</body>
</html>
