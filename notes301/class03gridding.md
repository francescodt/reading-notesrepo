## Grid life  

Grids are pretty cool, and kinda like flexbox. They basically make floats worthless, or well, even more so. Combined, that is. Grids define the element as a grid ontainer and establishs a new grid formatting context for it's contents. Basically, it turns your page into a grid, and allows you to move stuff how you actually think it should be moved, besides fr's. But that's in a minute.  

*grid* - generates block level grid.  
*inline-grid* - generates an inline-level grid.  


*track-size* - can be a length, percentage or fr (fraction).  
*line-name* - whatever you want it to be.   
grid-template-columns - formats by columns, can use multiple selects.   
grid-template-rows - formats by rows, can use multuple selects.  

grid-template-area - does the whole goddamn thing. Like seriously. multiple selectors for beginning and ends of columns, then rows.  

*grid-column-gap / grid-row-gap* - it's what you think it is. gaps between the row or column. Basically margin.  

#### justify content  
*start* items are placed at the start of the cell.  
*end* items are placed at the end of the cell.   
*center:* items are centered in the cell.  

#### align-items   
*start* items are placed at the top of the cell.  
*end* items are placed at the bottom of the cell.   
*center:* items are centered in the cell. 

#### align-content
*start:* items packed to the start of the container. The (more supported) flex-start honors the flex-direction while start honors the writing-mode direction.  
*end:* items packed to the end of the container. The (more support) flex-end honors the flex-direction while end honors the writing-mode direction.  
*center:* items centered in the container  
*space-between:* items evenly distributed; the first line is at the start of the container while the last one is at the end  
*space-around:* items evenly distributed with equal space around each line  
*space-evenly:* items are evenly distributed with equal space around them 


There is actually just miles of content on this stuff. Most of it just has to do with specificity, and you won't actually remember anything that you read/write until you get that "ah-ha" and then it disappears until the next time you have to look it up again. That's okay. Grid is good. Flexbox is good. That's all that matters.