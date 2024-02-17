<p align="center">
<img src="https://64.media.tumblr.com/05430d732ce5f2d785a0486a045d6de1/8d9c8026d5c4d00d-dd/s2048x3072/7eb30de9b907f2bbe6920b811d7c23b500608c2f.pnj">
<p align="center">

<p align="center">
<img src="https://64.media.tumblr.com/05430d732ce5f2d785a0486a045d6de1/8d9c8026d5c4d00d-dd/s2048x3072/7eb30de9b907f2bbe6920b811d7c23b500608c2f.pnj">
<p align="center">

<img src=

<style>
#wobble {
 
 }
</style>
 
<script type="text/javascript">
// <![CDATA[
var speed=100; // speed of wobbling, lower is faster
var height=3; // height of wobbling in pixels
 
/****************************
*    Wobbly Text Effect     *
*(c) 2003-6 mf2fm web-design*
*  http://www.mf2fm.com/rv  *
* DON'T EDIT BELOW THIS BOX *
****************************/
var wobtxt, wobble, wobcnt=0;
window.onload=function() { if (document.getElementById) {
  var i, wobli;
  wobble=document.getElementById("wobble");
  wobtxt=wobble.firstChild.nodeValue;
  while (wobble.childNodes.length) wobble.removeChild(wobble.childNodes[0]);
  for (i=0; i<wobtxt.length; i++) {
    wobli=document.createElement("span");
    wobli.setAttribute("id", "wobb"+i);
    wobli.style.position="relative";
    wobli.appendChild(document.createTextNode(wobtxt.charAt(i)));
    if (alink) {
      wobli.style.cursor="pointer";
      wobli.onclick=function() { top.location.href=alink; }
    }
    wobble.appendChild(wobli);
  }
  setInterval("wobbler()", speed);
}}
 
function wobbler() {
  for (var i=0; i<wobtxt.length; i++) document.getElementById("wobb"+i).style.top=Math.round(height*Math.sin(i+wobcnt))+"px"
  wobcnt++;
}
// ]]>
</script>
 
<div id="wobble">text</div>
