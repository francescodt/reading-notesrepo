## CSS 2: electric boogaloo: why it's my least favorite of everything  
CSS associates style rules with HTML elements. A CSS rule will contain a selector and a declaration.  
CSS properties affect how elements are displayed. Inside the curly brackets is a property and a value, seperated by colons. You can specify multiple properties in one declaration.  

### Building blocks  
Css treats HTML elements as if it is in it's own box. (see box model). This is either inline or block level.  
_block level_ starts a new line  
_inline_ keeps text inline, and allows flow in between surrounding text. wow. who would've guessed. 

### containing elements
if one block-level element sits inside another block-level element then the outer box is known as the containg or parent element.  
_example_ div tags are ways to group multiple child elements  

### Position, position, position
_normal_ every block level element appears on a new lnie, causing each item to appear lower down the page than the previous one.  
_relative_ this moves an element from the position it would be in normal flow, shifting it to the top, right bottom or left of where it would be placed.  
_absolute_ this positions the element in relation to it's containing element, it is taken out of normal slow, meaning it does not affect the position of any usrronding elements.  
_box offset_ Used to indicated where a box should be positioned. tells the browser how far from the TRBL it should be placed.  
_fixed_ form of absolute positioning that positions the element in relation to the browser window, as opposed to the containing element.  
_floating_ it's the worst, just don't do it.  
_static:_ In normal flow, each block-level element sits on top of the next one. Since this is the defaul way in which browsers treat HTML elements, you do not need a CSS property to indicate that elements should appear in normal flow.  

### fixed width layouts  
Advantages
 - Pixels values are accurate at controlling size and positioning of elements  
 - The designed has far greater control
 - The size of an image will always remain the same relative to the rest of the page  

Disadvantages  
 - You can end up with big gaps around the ends  
 - If the users screen is a higher resolution, the page can look smaller and be harder to read  
 - The design works best on devices that have a site or resolution similar  
 - pages take up more vertical space than a liquid layout with same content  

 ### Liquid layouts
 Advantages  
 - Pages exapnd to fill the entire browser window so there are no spaces around the page  
 - if the user has a small window, the page can contract to fit it withou the user having to scroll to the side  
 - the design is tolerant of user setting fotn sizes larger than the designer intended  

Disadvantages  
 -  If you do not control th width of sections, the design can look very different than intended  
 - If the user has a wide window, lines of text can become long which make it hard to look at  
 - if th user has a very narrow window, words may be squashed and you can end up with few words on each line  

