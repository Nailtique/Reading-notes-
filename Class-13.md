A  brief history of local storage hacks before the HTML 5:

so in the beggning, only th einternet explorer was available, microsoft manplulated the scene those days, made everyone believe hT 
SO microsoft had DHTML behaviors : 
This topic documents a feature of Binary Behaviors, which are obsolete as of Internet Explorer 10.

Dynamic HTML (DHTML) behaviors are components that encapsulate specific functionality or behavior on a page. When applied to a standard HTML element on a page, a behavior enhances that element's default behavior. An element behavior enables you to add a custom element to pages. And a ViewLink enables a document tree to be encapsulated in 
an HTML Component (HTC) file, separate from the content of the main Web page.
userData allows web pages to store up to 64 KB of data per domain, in a hierarchical XML-based structure. (Trusted domains, such as intranet sites, can store 10 times that amount. And hey, 640 KB ought to be enough for anybody.) IE does not present any form of permissions dialog, and there is no allowance for inc
reasing the amount of storage available.
HTML5 defines the <canvas> element as “a resolution-dependent bitmap canvas that can be used for rendering graphs, game graphics, or other visual images on the fly.” A canvas is a rectangle in your page where you can use JavaScript to draw anything you want. HTML5 defines a set of functions (“the canvas API”) for drawing shapes, defining paths, creating gradients, and applying transformations.

Checking for the canvas API uses detection technique #2. If your browser supports the canvas API, the DOM object it creates to represent a <canvas> element will have a getContext() method. If your browser doesn’t support the canvas API, the DOM object it creates for a <canvas> element will only have the set of common properties, but not anything canvas-specific.

function supports_canvas() {
  return !!document.createElement('canvas').getContext;
}
This function starts by creating a dummy <canvas> element. But the element is never attached to your page, so no one will ever see it. It’s just floating in memory, going nowhere and doing nothing, like a canoe on a lazy river.

return !!document.createElement('canvas').getContext;
As soon as you create the dummy <canvas> element, you test for the presence of a getContext() method. This method will only exist if your browser supports the canvas API.

return !!document.createElement('canvas').getContext;
Finally, you use the double-negative trick to force the result to a Boolean value (true or false).

return !!document.createElement('canvas').getContext;
This function will detect support for most of the canvas API, including shapes, paths, gradients & patterns. It will not detect the third-party explorercanvas library that implements the canvas API in Microsoft Internet Explorer.

Instead of writing this function yourself, you can use Modernizr to detect support for the canvas API.

↶ check for canvas support

if (Modernizr.canvas) {
  // let's draw some shapes!
} else {
  // no native canvas support available :(
}
There is a separate test for the canvas text API, which I will demonstrate next.

❧Local Storage for Web Applications
Local storage is part of the HTML5 Web Storage API and it allows you to store data in the browser. Unlike cookies, data stored using local storage isn’t sent back to the server. All data stays on the client, and you can currently store from 2MB to 10MB. This limit is tied to the specific browser, protocol (HTTP or HTTPS), port, and top level domain in use.

Potentially Dealbreaking Downsides:

Cookies are included with every HTTP request, thereby slowing down your web application by needlessly transmitting the same data over and over
Cookies are included with every HTTP request, thereby sending data unencrypted over the internet (unless your entire web application is served over SSL)
Cookies are limited to about 4 KB of data — enough to slow down your application (see above), but not enough to be terribly useful
LOCAL STORAGE HACKS BEFORE HTML5:
userData allows web pages to store up to 64 KB of data per domain, in a hierarchical XML-based structure.
intranet sites:Trusted domains can store 10 times that amount.And hey, 640 KB ought to be enough for anybody.
Local Shared Objects allows Flash objects to store up to 100 KB of data per domain.

### HTML5 STORAGE

HTML5 Storage: it’s a way for web pages to store named key/value pairs locally, within the client web browser.

### STORAGEEVENT OBJECT

PROPERTY	DESCRIPTION
key	named key that was added, removed, or modified
oldValue	the previous value (now overwritten), or null if a new item was added
newValue	the new value, or null if an item was removed
url*	the page which called a method that triggered this change
Use HTML local storage:
Remove Single Row:
<script type="text/javascript> localStorage.removeItem(key); //Remove A Single Desired KEY From Local Storage </script>

Insert A Single Row:
<script type="text/javascript> localStorage.setItem("key", "value"); //Set A Single Desired KEY-VALUE In Local Storage </script>

Get A Single Row:
<script type="text/javascript> var getValue = localStorage.getItem("key"); //Get A Single Desired KEY's VALUE From Local Storage </script>

Remove All Rows:
<script type="text/javascript> localStorage.clear(); //Clear All Local Storage KEY-VALUE </script>
