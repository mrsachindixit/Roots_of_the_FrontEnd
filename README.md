# Roots of the FrontEnd

*By Sachin Dixit*

## Today's Web Architecture

![Web Application Architecture: users interact with the Frontend (HTML, CSS, JavaScript) which exchanges Request/Response with the Backend (app logic in PHP, JavaScript, Python, Java) via a Web Server backed by a File System and Database](assets/images/slide-2-img1.png)

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

- Popular method of access internet
- Works on hyper text ( what is hypertext ?)
- Hypertext document on internet are known as web pages !
- Hypermedia ?
- Hyper link [ what is normal link then ? ]
- Web pages are created using language called as HTML
- "Web" browser [ File browser ? ]
- Notion of U R L
- MIME Types

![Layered diagram of the web: HTML, CSS, Web APIs and JavaScript sit above HTTP, which sits above DNS, UDP, TCP, TLS and IP](assets/images/slide-4-img1.png)

## Http

- Stateless vs Sessionless
- Request -Response -Headers
- Cookies and regulations !!
- CSP-CORS-Vulnerabilities
- APIs : XMLHttpRequest, Fetch

![Anatomy of an HTTP response showing the protocol version, status code, status message and headers](assets/images/slide-5-img3.png)

![Same-origin vs cross-origin requests: same-origin requests are always allowed while cross-origin requests are controlled by CORS](assets/images/slide-5-img2.png)

![Anatomy of an HTTP request showing the method (GET), path, protocol version and headers](assets/images/slide-5-img1.png)

## Http Evolutions

![HTTP protocol stack transition and comparison from HTTP/1.0 through HTTP/1.1, HTTP/2 and HTTP/3, showing the move from TCP+TLS to UDP+QUIC](assets/images/slide-6-img1.png)

Image via: <https://milestone-of-se.nesuke.com/en/l7protocol/http/http3-over-quic/>

## Http offshoots

- SSL/TLS
- PKI
- Websocket
- webDAV
- REST
- RSS, ATOM
- Vulnerabilities guides: <https://infosec.mozilla.org/guidelines/web_security> <https://owasp.org/www-project-top-ten/>
- Evolution of web: <http://www.evolutionoftheweb.com/>

## Browsers

- Components : Own UI, Engines, Networking, JS Engines, Storages, Plugins
- Engines : Trident, Webkit, Gecko
- Multiple Specs support
- History <https://blog.mozilla.org/en/internet-culture/deep-dives/why-are-hyperlinks-blue>

![Browser components: User Interface, Browser engine, Rendering engine, Networking, JavaScript Interpreter, UI Backend and Data Persistence](assets/images/slide-8-img1.png)

![Rendering flow: Parsing HTML to construct the DOM tree, Render tree construction, Layout of the render tree, Painting the render tree](assets/images/slide-8-img2.png)

Images via <https://www.html5rocks.com/en/tutorials/internals/howbrowserswork/>

## The Rendering

![WebKit main flow: HTML Parser builds the DOM tree, CSS Parser builds style rules, attachment forms the render tree, then layout and painting to display](assets/images/slide-9-img1.png)

![Document processing stages: Lexical Analysis, Syntax Analysis, Parse Tree](assets/images/slide-9-img2.png)

![HTML parsing flow: Network to Tokeniser to Tree Construction to DOM, with Script Execution and document.write()](assets/images/slide-9-img3.png)

![Gecko main flow: Parser, Content Sink, Content Model, Frame Constructor, Frame Tree, Reflow, Painting to display](assets/images/slide-9-img4.png)

![Parsing a CSS rule into a CSSStyleSheet tree of CSSRule, Selectors and Declarations](assets/images/slide-9-img5.png)

## HTML

- HTML ⇒ Structure, CSS ⇒ Presentation, JS ⇒ Behaviour
- Links, Documents, Tags, Resources
- UI elements, validations,
- Animations, Accessibility
- MultiMedia tags
- Storage : Webstorage, IndexedDB
- Service workers, PWA
- FORM as element of interaction

![Stacked layers of HTML, CSS and JavaScript](assets/images/slide-10-img3.png)

![HTML element with an attribute: a paragraph with class "editor-note"](assets/images/slide-10-img2.png)

![Anatomy of an HTML element: opening tag, content, closing tag](assets/images/slide-10-img1.png)

## CSS

- Style-Sheet
- Cascading, Inheritance
- Selectors-specificity : Universal(*), Elements, Type, ID, Class, Attribute, Pseudo-class, combinators
- Font, color(RGB, HSL, hex, CMYK), space, sizes(pixel, %, em), viewport
- Tables - Divs
- Box : FlexBox, Grids, Floats, Layouts, Animations
- RWD, media query
- CSS versions, Browser compatibility

![Anatomy of a CSS declaration: selector, property and property value](assets/images/slide-11-img1.png)

![Flow of loading and parsing HTML and CSS to create the DOM tree and attach styles for display](assets/images/slide-11-img3.png)

![The CSS box model: content, padding, border and margin edges](assets/images/slide-11-img2.png)

![Flexbox layout showing the main axis, cross axis and flex items in a flex container](assets/images/slide-11-img4.png)

![CSS grid layout showing columns, gutters and rows of content](assets/images/slide-11-img5.png)

## JS

- Dynamic programming language for browser (& nodejs), Single threaded, Interpreted, functional, Object based
- Basic programming constructs
- Events, REPL, Async
- JSON !!
- Browser APIs: DOM, XMLHttpRequest, Geolocation, Canvas, Storage, ServiceWorkers, WebGL, WebRTC, Codes
- Versions : ES16, ES20

![Event capturing and bubbling when a <video> element is clicked, showing how ancestors are checked for onclick handlers](assets/images/slide-12-img1.png)

![AJAX data flow: client exchanges HTTP Request/Response with AJAX, which stores and requests data across DB and offline states for data, treatments and display](assets/images/slide-12-img2.png)

## Document and server pages

- Applet, Flash
- Active pages : JSP / ASP
- JSF, Portlet
- JSP : Taglibs, EL

![Applet lifecycle: init(), start(), paint(), stop() and destroy() methods](assets/images/slide-13-img1.png)

![Model-View-Controller with a web browser calling a Servlet/Filter controller, JSP pages view and JavaBeans model backed by data sources](assets/images/slide-13-img2.png)

![Tag handler INIT PROTOCOL state diagram for properties, pageContext, parent and attributes](assets/images/slide-13-img5.png)

![Portlet container action and render sequence between client, portal and portlets](assets/images/slide-13-img3.png)

![JSF request lifecycle: Restore View, Apply Requests, Process Events, Process Validations, Update Model Values, Invoke Application and Render Response](assets/images/slide-13-img4.png)

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

![Angular architecture sketch: template, component, metadata, directive, injector and service with property binding and event binding](assets/images/slide-17-img1.png)

## Vue

![Vue instance lifecycle diagram from new Vue() through beforeCreate, created, beforeMount, mounted, beforeUpdate, updated, beforeDestroy and destroyed hooks](assets/images/slide-18-img1.png)
