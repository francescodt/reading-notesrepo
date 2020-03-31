## jQuery
jQuery is a JavaScript file that you include into your webpages. It allows you to find elements using css-style selectors and then do something with jquery methods.  

First you find the element using CSS style selectors.  
$('li.hot') - finds all of the li elements with the class hot.  

Now do something with it.  
$('li.hot).addClass('complete'); -This would add a new value to the class attribute.  

When you select one or more elements, a jQuery object is returned. It is also known as a matched set or a jquery selection. If a jQuery selection holds more than one element, and a method is used to get information from the selected elements, it will retrieve information from the first element in the matched set. If a jQuery selection holds more than one element, and a method is used to update information on the page, it will update all elements in the matched set, not just the first.  

For reference:  
Getting information - first element  
Setting information - all of the elements  

When you create a selection with jQuery, it stores a reference to the corresponding nodes in the DOM tree. It does not create copies of them. A jQuery object sotres references to the elements. Caching a jQuery objects stores a reference to it in a variable.  

The .css() method allows you to retrieve and set the values of css properties.  
var backgroundColor = $('li').css('background-color');  
$('li').css(background-color', '#00000');  

The first line gets the information, the second line sets that information. The properties are separated with a comma as well, not a colon.  

