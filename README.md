# Github

#### kniha

https://git-scm.com/book/cs/v2

#### Html preview

http://htmlpreview.github.io/?https://.....

#### Html include

https://www.boutell.com/newfaq/creating/include.html

1) 
 So at the point in your page where you wish to insert the file includeone.html, which is found in the same folder as the page, you'll need to do this:

<span id="includeone">
</span>

And at the beginning of the body of your page, you'll need to do this:

<body onLoad="clientSideInclude('includeone', 'includeone.html');">

Of course, a long, complicated onLoad handler can be very ugly. You can avoid that problem by moving the call (or calls!) to clientSideInclude to a function in a <script> element somewhere in the <head> element of the page. Then just call your function from onLoad. 

2) 

<script>
function clientSideInclude(id, url) {
  var req = false;
  // For Safari, Firefox, and other non-MS browsers
  if (window.XMLHttpRequest) {
    try {
      req = new XMLHttpRequest();
    } catch (e) {
      req = false;
    }
  } else if (window.ActiveXObject) {
    // For Internet Explorer on Windows
    try {
      req = new ActiveXObject("Msxml2.XMLHTTP");
    } catch (e) {
      try {
        req = new ActiveXObject("Microsoft.XMLHTTP");
      } catch (e) {
        req = false;
      }
    }
  }
 var element = document.getElementById(id);
 if (!element) {
  alert("Bad id " + id +
   "passed to clientSideInclude." +
   "You need a div or span element " +
   "with this id in your page.");
  return;
 }
  if (req) {
    // Synchronous request, wait till we have it all
    req.open('GET', url, false);
    req.send(null);
    element.innerHTML = req.responseText;
  } else {
    element.innerHTML =
   "Sorry, your browser does not support " +
      "XMLHTTPRequest objects. This page requires " +
      "Internet Explorer 5 or better for Windows, " +
      "or Firefox for any system, or Safari. Other " +
      "compatible browsers may also exist.";
  }
}
</script>  

#### Html iframe 

<iframe src="http://htmlpreview.github.io/?https://...." align="left"
frameborder="0" width="90%" height="300" scrolling="yes" target="_parent"></iframe>

####  Raw githack

https://raw.githack.com/
