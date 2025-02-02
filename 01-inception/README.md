# 01 - Inception

We started learning react from scratch. Environment setup was clearly explained. Started with creating a simple Hello world program . First, using only html, then we tried to implement the same through javascript. Finally, we created a simple hello world program using React. Everything was done without installing any package. Unlike other courses which starts with create-react-app as first session, we tried writing the react code from zero.

#### Topic Covered:

<ul>
  <li>Getting started with React</li>
  <li>React vs ReactDOM</li>
  <li>Create react element</li>
  <li>Nested react Element</li>
</ul>

## Notes:

- [Handwritten [PDF]](https://github.com/deltanode/react-playground/blob/main/00-React-Notes/Chapter%2001%20-%20Inception%20-%20HandWritten%20Notes.pdf) 
- [Digital [PDF]](https://github.com/deltanode/react-playground/blob/main/00-React-Notes/Chapter%2001%20-%20Inception%20-%20Digital%20Notes.pdf)
- [Notes.md](https://github.com/deltanode/react-playground/blob/main/01-inception/notes.md)

 > **Credit**: 
`Digital Notes:` [Arpan Kesh](https://www.linkedin.com/in/arpan-kesh-687740194/) | 
`Handwritten Notes:`[Ashraya KK](https://github.com/Ashrayaa/Namaste-React) | 
`Notes.md:` [Harshitha Solai](https://github.com/Learn-React-With-Harshi)  

## Theory:

<!-- ************************** -->
<details>
<summary>What is `Emmet`?</summary><br>
<blockquote> 
  
Emmet is a free <strong>add-on</strong> for your text editor that allows you to type shortcuts that are then expanded into full pieces of code.

Most useful emmet abbreviations are :

`HTML`

1. `html:5` - generates html5 boilerplate
2. `ui>li` - nested elements
3. `h1.#heading.container.con` - create h1 element with id heading and classes container and con
4. `div[data-name=harshi]` - Custom attribute <div data-name="Harshi"></div>
5. `header+div+footer` - generate siblings <header></header> <div></div> <footer></footer>

`CSS`

1. `m10-10-10-10` - Margin on all sides margin: 10px 10px 10px 10px;
</blockquote><br>
</details>

<!-- ************************** -->

<details>
<summary>Difference between a `Module` and `Package`?</summary><br>
<blockquote>

A `module` is a single JavaScript file that has some reasonable functionality.
A `package` is a directory with one or more modules inside of it and a package.json file which has metadata about the package.

A package can be very simple for example, `underscore` just has a single JavaScript file (we see two versions of it, regular and minified version and package.json)

Whereas a more complex package like `Express` has one JavaScript file in the root, but inside its sub-directories has quite a few more JavaScript files and more within sub-directories of that

Now it's very common for people to refer to a package as a module.

_More_:-

`npm` has some official definations:-

- A `package` is a file or directory that is described by a package.json file.
- A `module` is any file or directory in the node_modules directory that can be loaded by the Node.js require() function.
- <b>Note</b>: Since modules are not required to have a package.json file, not all modules are packages. Only modules that have a package.json file are also packages.

For `node.js`

- Modules are libraries for Node.js.

> Node.js has a simple module loading system. In Node.js, files and modules are in one-to-one correspondence.

- Examples of modules:

  - Circle.js
  - Rectangle.js
  - Square.js

- A package is one or more modules (libraries) grouped (or packaged) together. These are commonly used by other packages or a project of your own. Node.js uses a package manager, where you can find and install thousands of packages.

- Example of a package:

```
Shapes             <- Package name
  - Circle.js      <-
  - Rectangle.js   <- Modules that belong to the Shapes package
  - Square.js      <-
```

Essentially, you could install the package, Shapes, and have access to the Circle, Rectangle, and Square modules.

</blockquote><br>
</details>

<!-- ************************** -->
<details>
<summary>Difference between a `Library` and `Framework`?</summary><br>
<blockquote>

A `library` is a collection of packages that perform specific operations whereas
a `framework` contains the basic flow and architecture of an application.

A key difference between the two is the is the <b>inversion of control</b> & <b>complexity</b> :- <br>

- `Libraries` contain a number of methods that a developer can just call whenever they write code. If a `library` is used, the application calls the code from the library. `Eg: React, JQuery, Lodash`

- The `framework` provides the flow of a software application and tells the developer what it needs and calls the code provided by the developer as required. `Eg: Node JS, Angular, Spring`

<b>NOTE:</b> When using a library, the control remains with the developer who tells the application when to call library functions. When using a framework, the control is reversed, which means that the framework tells the developer where code needs to be provided and calls it as it requires.

<br>

_More_:-

- A <strong>library</strong> is like going to Ikea. You already have a home, but you need a bit of help with furniture. You don’t feel like making your own table from scratch. Ikea allows you to pick and choose different things to go in your home. You are in control. <br><br>
- A <strong>framework</strong>, on the other hand, is like building a model home. You have a set of blueprints and a few limited choices when it comes to architecture and design. Ultimately, the contractor and blueprint are in control. And they will let you know when and where you can provide your input. <br><br>
- <strong>Both Frameworks and Libraries</strong> are code written by someone else that is used to help solve common problems or to optimise performance. <br><br>
- A key difference between the two is the <strong>inversion of control</strong>. When using a library, the control remains with the developer who tells the application when to call library functions. When using a framework, the control is reversed, which means that the framework tells the developer where code needs to be provided and calls it as it requires.
</blockquote> <br>
</details>

<!-- ************************** -->
<details>
<summary>What is `CDN`? Why do we use it?</summary><br>
<blockquote>
- A CDN (content delivery network), also called a content distribution network, is a group of geographically distributed and interconnected servers. They provide cached internet content from a network location closest to a user to speed up its delivery. <br><br>
- The primary goal of a CDN is to improve web performance by reducing the time needed to send content and rich media to users. <br><br>
- CDN architecture is also designed to reduce network latency caused by hauling traffic over long distances and across several networks. Eliminating latency is important as more dynamic content, video and software as a service are delivered to an increasing number of mobile devices.
</blockquote><br>
</details>

<!-- ************************** -->
<details>
<summary>Why is `React` known as React?</summary><br>
<blockquote>    
- React is a JavaScript library that helps developers to build user interfaces – the things you interact with on websites. It has become popular because of its simplicity and flexibility. <br><br>      
- React is named <strong>React</strong> because of its ability to react to changes in data. When the data in a React component changes, React will automatically re-render the component so that it reflects the new data. This makes it easy to create performant user interfaces that always look up-to-date. <br><br>
- React was created by Jordan Walke, a software engineer at Facebook. It was first used internally at Facebook to power News Feed and other user interface elements. After seeing how well it performed, Jordan open-sourced React and made it available to the world.
</blockquote><br>
</details>

<!-- ************************** -->
<details>
<summary>What is `crossorigin` in script tag?</summary><br>
<blockquote>

- The crossorigin attribute provides support for `CORS` , defining how the element handles cross-origin requests. CORS stands for Cross-Origin Resource Sharing. If cross-origin is set to "user-credential", then user authentication is required to access the file.

_More_:-

- The crossorigin attribute sets the <strong>mode</strong> of the request to an HTTP CORS Request. <br><br>
- Web pages often make requests to load resources on other servers. Here is where CORS comes in. <br><br>
- A cross-origin request is a request for a resource (e.g. style sheets, iframes, images, fonts, or scripts) from another domain. <br><br>
- CORS is used to manage cross-origin requests. <br><br>
- CORS stands for Cross-Origin Resource Sharing, and is a mechanism that allows resources on a web page to be requested from another domain outside their own domain. It defines a way of how a browser and server can interact to determine whether it is safe to allow the cross-origin request. CORS allows servers to specify who can access the assets on the server, among many other things. <br><br>
- <strong>Tip:</strong> The opposite of cross-origin requests is <strong>same-origin</strong> requests. This means that a web page can only interact with other documents that are also on the same server. This policy enforces that documents that interact with each other must have the same origin (domain). <br><br>
- CORS is a standard mechanism used to retrieve files from other domains.
</blockquote><br>
</details>

<!-- ************************** -->
<details>
<summary>What is difference between `React` and `ReactDOM` ?</summary><br>
<blockquote>

`React` is a JavaScript library for building User Interfaces whereas `ReactDOM` is also JavaScript library that allows `React to interact with the DOM`.
<br><br>
The react package contains `React.createElement()`, `React.Component`, `React.Children`, and other helpers related to elements and component classes. You can think of these as the isomorphic or universal helpers that you need to build components.
<br><br>
The react-dom package contains `ReactDOM.render()`, and in react-dom/server we have server-side rendering support with `ReactDOMServer.renderToString()` and `ReactDOMServer.renderToStaticMarkup()`.

<br>
  
*More*:-

- In order to work with <strong>React</strong> in the <strong>browsers</strong>, we need to include 2 libraries: `React` and `ReactDOM`. <br><br>
- <strong>React</strong> library is responsible for creating views and <strong>ReactDOM</strong> library is responsible to actually render UI in the browser. <br><br>
- Include these two libraries before your main JavaScript file.
</blockquote><br>
</details>

<!-- ************************** -->
<details>
<summary>What is difference between `react.development.js` and `react.production.js` files via CDN ?</summary><br>
<blockquote>

`react.production.js` - production code of react library that is minified and production ready. <br>
`react.development.js` - More readable and developer friendly react library code that can be used to debug.

_More_:-

- react.production.js are the minified files. <br><br>
- Both react.development.js and react.production.js contains the similar code. The code difference between both files is nothing. <br><br>
- But, react.production.js is much more optimised for production use. The size of react.production.js will be very less then react.development.js
</blockquote><br>
</details>

<!-- ************************** -->
<details>
<summary>What is `async` and `defer` ?</summary><br>
<blockquote>

`Without async/defer` : Browser stops the html parsing once script tag is encountered.
It resumes parsing only after script is fetched and executed.

`Async` : Html parsing is done in parallel while scripts are being fetched from the network and executed.
Once the script is done with execution, html parsing is resumed. This can be used for external scripts like google analytics.
It is better to avoid async for scripts that are dependent on other scripts since we dont know in which order script will be executed.

`Defer` : Similar to async, Html parsing is done in parallel while scripts are being fetched from the network. But scripts are executed only after the
html parsing is done.

_More_:-

- When we load a webpage then 2 major things happens, <strong>HTML Parshing</strong> and <strong>Loading of scripts</strong>.<br>
- Now, <strong>Loading of scripts</strong> contains 2 parts, <strong>Fetching the script from the network</strong> & <strong>Executing it line by line</strong>. <br>
- Now, there are 3 scenario: <strong>Normal</strong>, using <strong>Async</strong> & using <strong>Defer</strong>. <br><br>
  - `Normal Case`: <script src="..." > <br>
  - In Normal case, during HTML parshing, when the browser encounter the script tag, it pauses the HTML parshing & start fetching the scripts from the network & then it executed them & again continues the HTML parshing after that. <br><br>
  - `Using Async`: <script async src="..." > <br>
  - In Async case, during HTML parshing, the browser parallelly fetches the script from the network. After fetching the script, it pauses the the HTML parshing & starts executing the script & then it again continues the HTML parshing after that.<br><br>
  - `Using Defer`: <script defer src="..." > <br>
  - In Async case, during HTML parshing, the browser parallelly fetches the script from the network. Now, when the HTML parshing completes, it then start executing the script at last. <br><br>
  - Also know, the Async does not guarantee the <strong>order of execution</strong> of the scripts but Defer does. <br><br>
    <img src="async-vs-defer-attributes.jpg"> <br><br>
  - When it comes to loading external JavaScript files on your website, should you use async or defer? <br><br>
  - Async allows your script to run as soon as it’s loaded, without blocking other elements on the page. Defer means your script will only execute after the page has finished loading. In most cases, async is the better option — but there are exceptions. Understanding when to use each one will help you create a faster and more efficient website. <br><br>
    - <strong>Async</strong> in script tag in JavaScript is a way to load scripts asynchronously. That means, if a script is async, it will be loaded independently of other scripts on the page, and will not block the page from loading. <br>
  - If you have a page with several external scripts, loading them all asynchronously can speed up the page load time, because the browser can download and execute them in parallel. <br>
  - To use async, simply add the async attribute to your script tag: <script async src="script.js"></script> <br><br>
  - By using the <strong>Defer</strong> attribute in HTML, the browser will load the script only after parsing (loading) the page. This can be helpful if you have a script that is dependent on other scripts, or if you want to improve the loading time of your page by loading scripts after the initial page load. <br>
  - To use defer, simply add the defer attribute to your script tag: <script defer src="script.js"></script> <br><br>
  - <a href="https://www.youtube.com/watch?v=IrHmpdORLu8"> reference video</a>
  </blockquote><br>
  </details>

<!-- ************************** -->
<!--
<details>
<summary>Question</summary><br>
<blockquote>

Answer
</blockquote><br>
</details>
-->
<!-- ************************** -->

## Coding:

- Set up all the tools in your laptop
  - VS Code
  - Chrome
  - Extensions of Chrome
- Build your first Hello World program using,
  - [Using just HTML](index.html)
  - [Using JS to manipulate the DOM](index.html)
  - [Using React](App.js)
    - use CDN Links
    - Create an Element
    - Create nested React Elements
    - Use root.render
- Learn about Arrow Functions before the next chapter.

## References:

- https://beta.reactjs.org/apis/react/createElement
