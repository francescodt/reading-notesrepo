## Dom Tree  
As a browser loads a web page, it creates a model of that page. The model is called a DOM tree, and it is stored in the memory. It consists of four types of nodes.  
_Document node_ - Every element, attribute and line of text in the HTML is represented by it's DOM node, and at the top of that tree is the document node. When the document is added, it represents the entire page, and is related to the document object.  
_element nodes_ - HTML elements describe the structure of an HTML page. 
_attribute nodes_ - The opening tags of HTML elements can carry attributes and these are reprensented by attribute nodes in the DOM tree.  
_text nodes_ once you have accessed an element node, you can then reach the text within that element. That is stores in it's own text node.  

Acessing and updating the DOM tree involes two steps:  
 - Locate the node that represents the element you want to work with  
 - Use it's text content, child elements, and attributes  

#### Select an individual element node  
_getElementById()_ uses the value of an element id attribute  
_querySelector()_ Uses a CSS selector, and returns the first matching element.

#### Select multiple elements  
_getElementsByClassName_ selects all elements that have a specific value for their class attribute  
_getElementsByTagNAme_ Selects all elements that have the specified tag name  
_querySelectorAll()_ Uses a css selector to select all matching elements  

#### Traversing between element nodes  
_parentNode_ Selects the parent of the current element node.  
_previousSibling/nextSib_ Selects the previous or next sibling
_firstChild/lastChild_ select the first or last child of the current element

#### Nodelists  
When a DOM method can return more than one element, it returns a NodeList (even if it only finds one matching Element.)  
NodeLists look like arrays and are numbered like them, but are actually an object called a collection.  
 - The length property tells you how many items are in the nodelist.
 - The item method returns a specific node from the NodeList when you tell it the index number of the item that you want.  

 