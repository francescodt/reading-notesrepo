## Former? I hardly even know her!  
Google makes forms, so basically it's everything that is important.  
Forms allow you to collect data. Like log in information, to textual input, radio buttons or file uploads.  
A user fills in a form and the presses a button which relays information to the server.  

### Structure  
_< form>_ Acts like body/head/etc for forms  
_action_ attribute that usually carries a url for the page on the server that will receive the information  
_input_ input element allows the creation of several different form controls.  
    - _name_ useful for login form, tracks where the data comes from.
    - _maxlength_ limits characters for the member to enter  
    - type _password_ blocks out characters, so peepers can't see
    - _textarea_ used to create a multiline text input. Needs to have a closing tag  
__radio buttons__   
type _radio_ allows pick of a number of options  
_value_ attribute indicates the value that is sent to the server for the selected option.  
_checked_ attribute can be used to indicate which value should be selected when the page loads.  
__check box__   
type _checkbox_ Allow users to select one or more options in an answer.  
__drop down list box__  
a drop down box, allows users to select one option from a drop down list.  
Uses < option> element to specify the options that the user can select from.  
There are a lot of these options, and most of them do the same thing.  

### HTML5 form stuff  
Validation helps ensure the suer enters information in a form that the server will be able to udnerstand when the form is submitted. Validating the contents of the form before it is sent to the server helps reduce work, and enables users to see if there are problems with the form faster.  
Date input helps gather information such as dates, email address, and urls.   
Email and url input allows vistors to enter email addresses and urls.  
Search input allows for specific searches to be performed.  


## List tables and forms  
Bullet point styles are ol, li, and ul type tags. The bullet type can be modified in css to a different __list-style-type__. This includes images for the bullets, like __list-style-image__.
You are able to position the bullets as well, with the inside /outside pair in liststyleposition  

_Table properties_  
 - width  
 - padding  
 - text-transform  
 - letter-spacing, font-size  
 - border-top, bottom, etc  
 - text-align  
 - background-color  
 - :hover  
_empty-cells_ allow you to show / hide empty cells in CSS  
_border-spacing, border-collapse_ controls the distance between adjacent cells  


## Events  
Events are triggered or raised. When an event has occured it is often described as having fired. Events trigger scripts and functions, when the click event fires on the element in this diagram, it could trigger a script that enlarges the selected item.  

Select the element nodes you want the script to respond to. Indicate which event on the selected nodes will trigger the response. State the code you want to run when the event occurs.   

When an event occurs, the event object tells you information about the event and the element it happened upon. Everytime an event fires, the event object contains helpful data about the event. The event object is passed to any function that is the event handler or listener. If you need to apss arguements to a named function,the event object will first be passed to the anonymous wrapped function. Then you must specify it as a parameter of the named function. When the event object is passed into a function, it is often given the parameter name e. It is wildly used shorthand. Note, however, that some programmers also use the parameter name e to refer to an error onject.  

