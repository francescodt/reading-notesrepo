## Links
_< a>_ used to create links, with an attribute called href. Shows blue by default.  
The text between the opening and closing tag is known as link text, where possible your link text should explain where vistors will be taken if they click on it.   
You can even use something like _mailto:_ to create a link that opens to an email prompt.   
_target_ if you want a link to open in a new window, you use the target attribute on the opening a tag.  

# Key concepts for positioning elements  
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


## Function function, something something baby
Functions are great. They let you group a series of statements together to perform a specific task. If different parts of a script repeat the same task, you can reuse the function, rather than repeat the same set of statements.  

Essentially you need to define a function, by giving it a name, declare the function, which is writing the task inside curly braces of what it will do, and then call the function outside of curly braces to make it run.  

Sometimes functions use variables, which means they need information to run. When you declare the function you give it parameters inside the fucntion, which act like variables. When you call a function that has paraments, you specify the values it should use in the parentheses that follow its name. The values are called arguements and they can be proided as values or as variables.  


