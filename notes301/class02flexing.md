## Flexicution

Flexbox is great for stuff that has undefined sizes, or just as an almost replacement to floating in general. The main idea behind the flex layout is to give the container the ability to alter its items’ width/height (and order) to best fill the available space (mostly to accommodate to all kind of display devices and screen sizes). A flex container expands items to fill available free space or shrinks them to prevent overflow.  

Terms  
*row (default):* left to right in ltr; right to left in rtl  
*row-reverse:* right to left in ltr; left to right in rtl  
*column:* same as row but top to bottom  
*column-reverse:* same as row-reverse but bottom to top  

All of the above apply to flex direction. Rows are across and columns are up and down. Essentially you can move elements inside of a container that is flexing. 



*nowrap (default):* all flex items will be on one line  
*wrap:* flex items will wrap onto multiple lines, from top to bottom.  
*wrap-reverse:* flex items will wrap onto multiple lines from bottom to top.  

The above applies to flex wrapping. How it moves across the screen. If it's too big, wrapping through or not and shrinking, or being to small and stretching across.  


*flex-end:* items are packed toward the end of the flex-direction.  
*start:* items are packed toward the start of the writing-mode direction.  
*end:* items are packed toward the end of the writing-mode direction.  
*left:* items are packed toward left edge of the container, unless that doesn’t make sense with the flex-direction, then it behaves like start.  
*right:* items are packed toward right edge of the container, unless that doesn’t make sense with the flex-direction, then it behaves like start.  
*center:* items are centered along the line  
*space-between:* items are evenly distributed in the line; first item is on the start line, last item on the end line  
*space-around:* items are evenly distributed in the line with equal space around them. Note that visually the spaces aren’t equal, since all the items have equal space on both sides. The first item will have one unit of space against the container edge, but two units of space between the next item because that next item has its own spacing that applies.  
*space-evenly:* items are distributed so that the spacing between any two items (and the space to the edges) is equal.  

Justifying the content moves it around the screen as you think it should.   

*flex-start / start / self-start:* items are placed at the start of the cross axis. The difference between these is subtle, and is about respecting the flex-direction rules or the writing-mode rules.  
*flex-end / end / self-end:* items are placed at the end of the cross axis. The difference again is subtle and is about respecting flex-direction rules vs. writing-mode rules.  
*center:* items are centered in the cross-axis  
*baseline:* items are aligned such as their baselines align  

This defines the default behavior for how flex items are laid out along the cross axis on the current line. This is the other axis to justify content.  



*flex-start / start:* items packed to the start of the container. The (more supported) flex-start honors the flex-direction while start honors the writing-mode direction.  
*flex-end / end:* items packed to the end of the container. The (more support) flex-end honors the flex-direction while end honors the writing-mode direction.  
*center:* items centered in the container  
*space-between:* items evenly distributed; the first line is at the start of the container while the last one is at the end  
*space-around:* items evenly distributed with equal space around each line  
*space-evenly:* items are evenly distributed with equal space around them  

This aligns a flex container’s lines within when there is extra space in the cross-axis.  

All of the above is for containers, but there is flexing for items too.  

Flex grow can allow specific items to grow across the container. Starts with 1, but an object with grow 2 will take up twice the amount of space. Flex shrink is the reverse.  



