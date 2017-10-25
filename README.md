# Github


##### Raw git - html preview

https://rawgit.com/

##### Windows editor

https://cloose.github.io/CuteMarkEd/

#### TOC generate
http://doctoc.herokuapp.com/

#### Markdown preview

http://markdownlivepreview.com/

#### Simplenote syntax

https://sourceforge.net/p/simplenotefran/wiki/markdown_syntax/

#### html to markdown

https://domchristie.github.io/to-markdown/

#### markdown to html

https://www.browserling.com/tools/markdown-to-html

#### kniha

https://git-scm.com/book/cs/v2

#### Html preview

http://htmlpreview.github.io/

http://htmlpreview.github.io/?https://.....

### Gist:

[Gist](https://gist.github.com/bedjan)

### Markdown syntaxe:

https://daringfireball.net/projects/markdown/syntax

http://jecas.cz/markdown

https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet

### Html do markdown:

[Html do markdown primo soubor](https://cloudconvert.com/html-to-md)
[Html do markdown](https://domchristie.github.io/to-markdown/)


#### Markdown to html

[Markdown do Html - pak update]{:target="_blank"}(http://trykramdown.herokuapp.com)

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


<iframe style="box-sizing: border-box;-moz-box-sizing: border-box;-webkit-box-sizing: border-box;margin: 0.5% 0.5% 0.5% 

0.5%;padding: 0.5%;" src="https://rawcdn.githack.com/bedjan/web_home/master/foot.html" align="left" frameborder="0" 

width="100%" height="auto" scrolling="no" target="_parent">https://github.com/bedjan/web_home/raw/master/....html</iframe>


<iframe src="http://htmlpreview.github.io/?https://...." align="left"
frameborder="0" width="90%" height="300" scrolling="yes" target="_parent"></iframe>

####  Raw githack

https://raw.githack.com/

Use this URL for development

example: https://raw.githack.com/bedjan/web_home/master/obsah.html

#### Permalink

http://jdem.cz/trvalink.html

#### Web s heslem

http://jdem.cz/heslo.html

#### Svg obrázek v html
<html>
<svg height="60" width="200">
 <text x="0" y="15" fill="#0D6AB7" transform="rotate(30 20,40)">"Osobní stránky"</text>
 váš web prohlížeč obrázek neumí přečíst
</svg>

</html>


#### DNS servery ČR

https://public-dns.info/nameserver/cz.html
