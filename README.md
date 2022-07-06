# Browser Rendering



Table of Contains :



 - [What is Browser Rendering](#what-is-browser-rendering)
 - [Browser Rendering Process](#browser-rendering-process)
   - [From Raw Bytes Of HTML To DOM](#from-raw-bytes-of-html-to-dom)
   - [From Raw Bytes Of CSS To CSSOM](#from-raw-bytes-of-css-to-cssom)
   - [Render Tree](#render-tree)
   - [Layout](#layout)
   - [Paint](#paint)
 - [References](#references)
 

## What Is Browser Rendering

Rendering offering is a process used in web development that converts website code into interactive pages that users see when they visit a website. The term usually refers to the use of HTML, CSS, and JavaScript codes. The process is completed by a rendering engine, software used by a web browser to render a web page. Because of its close relationship with web browsers, rendering engines are often referred to as browser engines.



## Browser Rendering Process 


Browser rendering process has five step 
1. From Raw Bytes Of HTML To DOM
2. From Raw Bytes Of CSS To CSSOM
3. Render Tree
4. Layout
5. Paint




![image](https://user-images.githubusercontent.com/108331918/177538510-7da1434e-d291-45b0-aa8b-d6ce2a443c68.png)
<div align="center">
<p><strong>Figure:</strong> Rendering Process</p>
</div>


  
### From Raw Bytes Of HTML To DOM


While loading a web page, the web server sends a folder of files containing HTML, CSS, and JavaScript code to the user's web browser.
Browser engine converts this data (bytes) into characters (HTML code).
It divides the letters into tokens , and then divides them into nodes .
The browser engine connects the nodes to a tree-like structure known as the Document Object Model (DOM). DOM stands for JavaScript HTML.


![image](https://user-images.githubusercontent.com/108331918/177538369-a369796e-0672-404c-9f2a-401328aeafe2.png)
<div align="center">
<p><strong>Figure:</strong> HTML to DOM</p>
</div>


### From Raw Bytes Of CSS To CSSOM


Browser engine converts this data (bytes) into characters (CSS code).
It divides the letters into tokens , and then divides them into nodes .
The browser engine connects the nodes to a tree-like structure known as the CSS Object Model (CSSOM). CSSOM stands for CSS.


![image](https://user-images.githubusercontent.com/108331918/177538897-14f62ee0-b26c-434b-b856-93c4aa6d95e3.png)
<div align="center">
<p><strong>Figure:</strong> CSS to CSSOM</p>
</div>

### Render Tree


The browser engine combines the DOM and CSSOM to create a tree-like structure called a Render Tree. The Render Tree contains the style and content information browsers need to populate a webpage for viewers to see, calculate the layout for each visible element of a webpage and paint them on the screen for the end user's view.

![image](https://user-images.githubusercontent.com/108331918/177542654-14f7df85-23e6-4f77-8efc-57981e875dda.png)
<div align="center">
<p><strong>Figure:</strong> Render Tree </p>
</div>

### Layout

The layout operation is the next step. Using the Render Tree, the browser engine calculates the position of each visible element of a web page.

### Paint 

Finally, the browser engine adds, or paints, the elements on the screen for the end-users view. The web page has now been rendered.

## References
- [What is Rendering](https://www.seobility.net/en/wiki/Rendering#:~:text=Rendering%20is%20a%20process%20used,to%20render%20a%20web%20page)
- [what is Rendring Process](https://web.dev/critical-rendering-path-render-tree-construction/)






