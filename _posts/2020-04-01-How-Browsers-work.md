## The components of a browser
![browser components](https://miro.medium.com/max/500/1*7Z5Yr1rxyZsevxYxWSgYQA.png)
* UI Interface is just the interface a user can see on the browser, such as Forward/backward buttons, address bar etc.
* Browser Engine is a medium between the UI interface with Rendering engine
* Rendering engine is the most important part of the browser and what developers care the most, it is all about how the resources are processed, see details below
* Networking is the component to communiate with server and fetch all the resources
* JS interpreter is the engine to interprete the JS files
* UI backend is the layer to communiate with OS and paint stuff on screen
* Data Persistence is where the cookies, localStorage etc. store

## How Rendering Engine Works
* First, it gets assets from Networking component
* Then, the HTML parser parses the HTML files and produce the DOM Tree, the CSS parser parses CSS files and produce CSSOM Tree
* Render Tree is produced by combining DOM Tree and CSSOM Tree, but hidden DOMs will be omitted in Render Tree and won't be painted onto screen
![create render tree](https://developers.google.com/web/fundamentals/performance/critical-rendering-path/images/render-tree-construction.png)
* Render Tree goes through Layout process, so all nodes in Render Tree know their positions in the page
* Paint the Layout onto screen by using UI backend.


