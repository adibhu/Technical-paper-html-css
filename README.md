# Technical-paper-html-css
## Introduction To HTML
- HTML stands for Hyper Text Markup Language.
- HTML is the standard markup language for creating Web pages.
- HTML describes the structure of a Web page.
- HTML consists of a series of elements.
- HTML elements tell the browser how to display the content.
- HTML elements label pieces of content such as "this is a heading", "this is a paragraph", "this is a link", etc.

### HTML Documents
- All HTML documents must start with a document type declaration: <!DOCTYPE html>.
- The HTML document itself begins with <html> and ends with </html>.
- The visible part of the HTML document is between <body> and </body>. 

### The <!DOCTYPE> Declaration
- The <!DOCTYPE> declaration represents the document type, and helps browsers to display web pages correctly.
- It must only appear once, at the top of the page (before any HTML tags). 
- The <!DOCTYPE> declaration is not case sensitive.

### Nested HTML Elements
- HTML elements can be nested (this means that elements can contain other elements).
- All HTML documents consist of nested HTML elements.

### HTML Attributes
- All HTML elements can have attributes.
- Attributes provide additional information about elements.
- Attributes are always specified in the start tag.
- Attributes usually come in name/value pairs like: name="value".

## Introduction to CSS
- CSS stands for Cascading Style Sheets.
- CSS describes how HTML elements are to be displayed on screen, paper, or in other media.
- CSS saves a lot of work. It can control the layout of multiple web pages all at once.
- External stylesheets are stored in CSS files.

### Box Model
- The CSS box model is essentially a box that wraps around every HTML element. It consists of: margins, borders, padding, and the actual content. The image   below illustrates the box model.

    - Content - The content of the box, where text and images appear.
    - Padding - Clears an area around the content. The padding is transparent.
    - Border - A border that goes around the padding and content.
    - Margin - Clears an area outside the border. The margin is transparent.
    
 ### Inline versus Block Elements
 #### Block-level Elements
 - A block-level element always starts on a new line, and the browsers automatically add some space (a margin) before and after the element.
 - A block-level element always takes up the full width available (stretches out to the left and right as far as it can).
 - Two commonly used block elements are ```<p>``` and ```<div>```.
 - The ```<p>``` element defines a paragraph in an HTML document.
 - The ```<div>``` element defines a division or a section in an HTML document.
 
 #### Inline Elements
 - An inline element does not start on a new line.
 - An inline element only takes up as much width as necessary.
 - ```<span>``` element is an example of Inline Elements.

 ### Positioning: Relative/Absolute
 - An element with position: relative; is positioned relative to its normal position.
 - Setting the top, right, bottom, and left properties of a relatively-positioned element will cause it to be adjusted away from its normal position. Other    content will not be adjusted to fit into any gap left by the element.
 - An element with position absolute; is positioned relative to the nearest positioned ancestor (instead of positioned relative to the viewport, like          fixed).
 - However; if an absolute positioned element has no positioned ancestors, it uses the document body, and moves along with page scrolling.
 - Absolute positioned elements are removed from the normal flow, and can overlap elements.
 
 ### Common CSS structural classes
 - Structural pseudo classes allow access to the child elements present within the hierarchy of parent elements. We can select first-child element, last-      child element, alternate elements present within the hierarchy of parent elements.
   1. :first-child
   2. :nth-child(n)
   3. :last-child
   4. :nth-last-child(n)
   5. :only-child
   6. :first-of-type
   7. :nth-of-type(n)
   8. :last-of-type
   9. :nth-last-of-type(n)
  
  ### CSS Specificity
  - If there are two or more CSS rules that point to the same element, the selector with the highest specificity value will "win", and its style               declaration will be applied to that HTML element.
  - Think of specificity as a score/rank that determines which style declaration are ultimately applied to an element.
  #### Specificity Hierarchy 
  - Inline styles
  - IDs
  - Classes, pseudo-classes, attribute selectors
  - Elements and pseudo-elements

  ### CSS Responsive Queries
  - Media query is a CSS technique introduced in CSS3.
  - It uses the @media rule to include a block of CSS properties only if a certain condition is true.
   #### Always Design for Mobile First
   - Mobile First means designing for mobile before designing for desktop or any other device (This will make the page display faster on smaller devices).
   - This means that we must make some changes in our CSS.
   - Instead of changing styles when the width gets smaller than 768px, we should change the design when the width gets larger than 768px.
  
  ### Flexbox
  - The Flexbox (or Flexible Box) layout model is a one-dimensional CSS layout model that allows you to create responsive layouts for your web application.
  - The key feature of the Flexbox model is that it adjusts the layout of your web page automatically based on the size of your content. You only need to       define the direction and the wrap behavior of the Flexbox with the flex-direction and flex-wrap properties.
  - The flexibility of the Flexbox model allows you to distribute unused space between elements that are vertically or horizontally aligned.

  ### Grid
  - The CSS Grid Layout Module offers a grid-based layout system, with rows and columns, making it easier to design web pages without having to use floats     and positioning.
  - A grid layout consists of a parent element, with one or more child elements.
  - All direct children of the grid container automatically become grid items.
  
  ### Common header meta tags
  - The ```<meta>``` tag defines metadata about an HTML document. Metadata is data (information) about data.
  - ```<meta>``` tags always go inside the ```<head>``` element, and are typically used to specify character set, page description, keywords, author of the     document, and viewport settings.
  - Metadata will not be displayed on the page, but is machine parsable.
  - Metadata is used by browsers (how to display content or reload page), search engines (keywords), and other web services.
  #### Attributes
  - charset
  - content
  - http-equiv
  - name
  #### Setting the Viewport
  - The viewport is the user's visible area of a web page. It varies with the device - it will be smaller on a mobile phone than on a computer screen.
  - This gives the browser instructions on how to control the page's dimensions and scaling.
  - The ```width=device-width``` part sets the width of the page to follow the screen-width of the device (which will vary depending on the device).
  - The ```initial-scale=1.0``` part sets the initial zoom level when the page is first loaded by the browser.
