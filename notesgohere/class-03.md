## Listing items  
_Ordered lists_ done with < ol>  
 - listed items done with < li> are fit inside the ordered lists.  
Ordered lists and their listed items will go in sequential order.  

_Unordered lists_ done with < ul>  
 - Similar to before, use < li>  
Unordered lists and their listed items will bullet, or whatever you decide to style as.  

_Definition lists_ created by < dl>  
 - Inside the definition lists at < dt> and < dd> elements.  
_dt_ is used to contain the term being defined.  
_dd_ is used to contain the definition.  

_Nested lists_ you can put other < ul> and < li> pairings inside each other.  
 - The further nested lists will identify differently   

 ## Box Sizing and being able to control them  
 Box width and height is something you are able to modify.  
 Popular forms are:  
 - pixels  
 - percentages  
 - ems  

 Pixels are more direct and exact sizing, percentages are relative to the browser window or another box if it is inside of it, and ems are base the size of the box off of the text within it.  

_Overflowing content_ allows you to take text that wouldn't fit and either hide, or add a scroll option to an element.  

## Box model  
Border, margin, and padding allow you to control the box model.  
_Border_ The space between one box and another.  
_Margin_ Sits outside the border, can create gaps between boxes.
_Padding_ The seperation of content and the box.  

_Border width_ the width of the border.  
 - Can be assigned with thin, medium, thick.  
 - Border-*-width (*top, right, bottom, left)  

 _Border-style_ Styles the border  
 - solid, single solid line  
 - dotted, series of square dots  
 - dashed, series of short dashes  
 - double, two solid lines  
 - groove, "carves" into the page  
 - ridge, "pops" from the page  
 - inset, embeds into the page  
 - outset, looks like it's coming out of the screen  
 - hidden/none, no border  

 _Border-color_ You can color the border with the same styling as border width.  


 ## Statements
 _If Statements_ evaluates a condition.  
 - If the condition evaluates true, any statement in the subsequent code block are executed.  
 _If else statements_ checks a condition.  
 - If it resolves as true, the first code is executed. If the condition resolves as false, the second code will run instead.  
 _Switch statements_ Runs a possible value for a variable and runs if the variable matches the code.  
 - [See](notesgohere/craigatwork/) for a solid example of switch statements. 
 
 _Truthy Falsy nonsense_  
 Falsy values are treated as if they are false. What doesn't return as falsy, is truthy. Since more things are truthy than falsy, those are therefore easier to define, and more important.   
 - Traditional boolean false (false)  
 - The number zero (0)  
 - NaN ( ' ' )  
 - Empty value ( 10/'score')  
 - Literal nothing (variables with no value)
 
 ## Loops
 Loops check a condition, if it returns tru, a code block will run. Then it is run again, if it is still true, it will run. It will condition to do this until it returns false.  
 Types of loops:  
_For_ If you need to run code a specific number of time, use a for loop.  
_While_ If you do not know how many times it should run, use a while loop.  
_Do while_ similar to while, but it will always run the statements inside curly braces at least once, even if false.  



