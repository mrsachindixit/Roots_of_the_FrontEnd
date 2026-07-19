# Roots of the FrontEnd

*By Sachin Dixit*

*This presentation uses a lot of material from mozilla so separate attribution is not given*

## Today's Web Architecture

<img src="assets/images/slide-2-img1.png" width="640" alt="Web Application Architecture: users interact with the Frontend (HTML, CSS, JavaScript) which exchanges Request/Response with the Backend (app logic in PHP, JavaScript, Python, Java) via a Web Server backed by a File System and Database">

- Scale
- Uptime
- Cost Efficiency
- Faster Response
- Ease of Integration
- Consistency
- Observability
- Security
- Extensible

## What is Internet

- Email
- Ftp
- Telnet
- Usenet news
- & WWW
- Is internet client server or peer to peer ?
- Dark net ?

## WWW

<table>
<tr>
<td valign="top">

- Popular method of access internet
- Works on hyper text ( what is hypertext ? )
- Hypertext document on internet are known as web pages !
- Hypermedia ?
- Hyper link [ what is normal link then ? ]
- Web pages are created using language called as HTML
- "Web" browser [ File browser ? ]
- Notion of U R L
- MIME Types

</td>
<td valign="top">

<img src="assets/images/slide-4-img1.png" width="450" alt="Layered diagram of the web: HTML, CSS, Web APIs and JavaScript sit above HTTP, which sits above DNS, UDP, TCP, TLS and IP">

</td>
</tr>
</table>

## Http

<table>
<tr>
<td valign="top">

- Stateless vs Sessionless
- Request -Response -Headers
- Cookies and regulations !!
- CSP-CORS-Vulnerabilities
- APIs : XMLHttpRequest, Fetch

</td>
<td valign="top">

<img src="assets/images/slide-5-img2.png" width="520" alt="Same-origin vs cross-origin requests: same-origin requests are always allowed while cross-origin requests are controlled by CORS">

<img src="assets/images/slide-5-img3.png" width="420" alt="Anatomy of an HTTP response showing the protocol version, status code, status message and headers">

<img src="assets/images/slide-5-img1.png" width="480" alt="Anatomy of an HTTP request showing the method (GET), path, protocol version and headers">

</td>
</tr>
</table>

## Http Evolutions

<img src="assets/images/slide-6-img1.png" width="700" alt="HTTP protocol stack transition and comparison from HTTP/1.0 through HTTP/1.1, HTTP/2 and HTTP/3, showing the move from TCP+TLS to UDP+QUIC">

Image via : <https://milestone-of-se.nesuke.com/en/l7protocol/http/http3-over-quic/>

## Http offshoots

- SSL/TLS
- PKI
- Websocket
- webDAV
- REST
- RSS, ATOM
- Vulnerabilities guides : <https://infosec.mozilla.org/guidelines/web_security> <https://owasp.org/www-project-top-ten/>
- Evolution of web : <http://www.evolutionoftheweb.com/>

## Browsers

<table>
<tr>
<td valign="top">

- Components : Own UI, Engines, Networking, JS Engines, Storages, Plugins
- Engines : Trident, Webkit, Gecko
- Multiple Specs support
- History <https://blog.mozilla.org/en/internet-culture/deep-dives/why-are-hyperlinks-blue>

</td>
<td valign="top">

<img src="assets/images/slide-8-img1.png" width="520" alt="Browser components: User Interface, Browser engine, Rendering engine, Networking, JavaScript Interpreter, UI Backend and Data Persistence">

<img src="assets/images/slide-8-img2.png" width="620" alt="Rendering flow: Parsing HTML to construct the DOM tree, Render tree construction, Layout of the render tree, Painting the render tree">

Images via <https://www.html5rocks.com/en/tutorials/internals/howbrowserswork/>

</td>
</tr>
</table>

## The Rendering

<img src="assets/images/slide-9-img1.png" width="450" alt="WebKit main flow: HTML Parser builds the DOM tree, CSS Parser builds style rules, attachment forms the render tree, then layout and painting to display">

<img src="assets/images/slide-9-img2.png" width="170" alt="Document processing stages: Lexical Analysis, Syntax Analysis, Parse Tree">

<img src="assets/images/slide-9-img3.png" width="340" alt="HTML parsing flow: Network to Tokeniser to Tree Construction to DOM, with Script Execution and document.write()">

<img src="assets/images/slide-9-img4.png" width="450" alt="Gecko main flow: Parser, Content Sink, Content Model, Frame Constructor, Frame Tree, Reflow, Painting to display">

<img src="assets/images/slide-9-img5.png" width="440" alt="Parsing a CSS rule into a CSSStyleSheet tree of CSSRule, Selectors and Declarations">

## HTML

<table>
<tr>
<td valign="top">

- HTML ⇒ Structure, CSS ⇒ Presentation, JS ⇒ Behaviour
- Links, Documents, Tags, Resources
- UI elements, validations,
- Animations, Accessibility
- MultiMedia tags
- Storage : Webstorage, IndexedDB
- Service workers, PWA
- FORM as element of interaction

</td>
<td valign="top">

<img src="assets/images/slide-10-img3.png" width="180" alt="Stacked layers of HTML, CSS and JavaScript">

<img src="assets/images/slide-10-img2.png" width="450" alt="HTML element with an attribute: a paragraph with class 'editor-note'">

<img src="assets/images/slide-10-img1.png" width="450" alt="Anatomy of an HTML element: opening tag, content, closing tag">

</td>
</tr>
</table>

## CSS

<table>
<tr>
<td valign="top">

- Style-Sheet
- Cascading, Inheritance
- Selectors-specificity : Universal(*), Elements, Type, ID, Class, Attribute, Pseudo-class, combinators
- Font, color(RGB, HSL, hex, CMYK), space, sizes(pixel, %, em), viewport
- Tables - Divs
- Box : FlexBox, Grids, Floats, Layouts, Animations
- RWD, media query
- CSS versions, Browser compatibility

</td>
<td valign="top">

<img src="assets/images/slide-11-img1.png" width="300" alt="Anatomy of a CSS declaration: selector, property and property value">

<img src="assets/images/slide-11-img3.png" width="430" alt="Flow of loading and parsing HTML and CSS to create the DOM tree and attach styles for display">

<img src="assets/images/slide-11-img2.png" width="330" alt="The CSS box model: content, padding, border and margin edges">

<img src="assets/images/slide-11-img4.png" width="330" alt="Flexbox layout showing the main axis, cross axis and flex items in a flex container">

<img src="assets/images/slide-11-img5.png" width="330" alt="CSS grid layout showing columns, gutters and rows of content">

</td>
</tr>
</table>

## JS

<table>
<tr>
<td valign="top">

- Dynamic programming language for browser (& nodejs), Single threaded, Interpreted, functional, Object based
- Basic programming constructs
- Events, REPL, Async
- JSON !!
- Browser APIs: DOM, XMLHttpRequest, Geolocation, Canvas, Storage, ServiceWorkers, WebGL, WebRTC, Codes
- Versions : ES16, ES20

</td>
<td valign="top">

<img src="assets/images/slide-12-img1.png" width="470" alt="Event capturing and bubbling when a <video> element is clicked, showing how ancestors are checked for onclick handlers">

<img src="assets/images/slide-12-img2.png" width="340" alt="AJAX data flow: client exchanges HTTP Request/Response with AJAX, which stores and requests data across DB and offline states for data, treatments and display">

</td>
</tr>
</table>

## Document and server pages

<table>
<tr>
<td valign="top">

- Applet, Flash
- Active pages : JSP / ASP
- JSF, Portlet
- JSP : Taglibs, EL

</td>
<td valign="top">

<img src="assets/images/slide-13-img1.png" width="230" alt="Applet lifecycle: init(), start(), paint(), stop() and destroy() methods">

<img src="assets/images/slide-13-img2.png" width="450" alt="Model-View-Controller with a web browser calling a Servlet/Filter controller, JSP pages view and JavaBeans model backed by data sources">

<img src="assets/images/slide-13-img5.png" width="300" alt="Tag handler INIT PROTOCOL state diagram for properties, pageContext, parent and attributes">

<img src="assets/images/slide-13-img3.png" width="330" alt="Portlet container action and render sequence between client, portal and portlets">

<img src="assets/images/slide-13-img4.png" width="450" alt="JSF request lifecycle: Restore View, Apply Requests, Process Events, Process Validations, Update Model Values, Invoke Application and Render Response">

</td>
</tr>
</table>

## AJAX and Jquery

- What ajax enabled
- The achievement of jQuery
- Dichotomy of layout vs event

## Componentization of web

- Ext and Angular.js what problem they set out to solve
- Routing
- Binding
- Layout
- Components (lifecycles )
- Styling
- Modules
- Menu
- Templates

| Framework | Browser support | Preferred DSL | Supported DSLs |
| --- | --- | --- | --- |
| Angular | IE9+ | TypeScript | HTML-based; TypeScript |
| React | Modern (IE9+ with Polyfills) | JSX | JSX; TypeScript |
| Vue | IE9+ | HTML-based | HTML-based, JSX, Pug |

## Popular UI libraries

- How each library solved the problem
- Angular - react - vue - polymer
- Ethical web design principles : <https://www.w3.org/TR/design-principles/#one-time-events>

## Angular

<img src="assets/images/slide-17-img1.png" width="600" alt="Angular architecture sketch: template, component, metadata, directive, injector and service with property binding and event binding">

## Vue

<img src="assets/images/slide-18-img1.png" width="360" alt="Vue instance lifecycle diagram from new Vue() through beforeCreate, created, beforeMount, mounted, beforeUpdate, updated, beforeDestroy and destroyed hooks">
