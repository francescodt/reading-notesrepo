## Data storage

Persistent local storage is one of the areas where native client applications have held an advantage over web applications. For native applications, the operating system typically provides an abstraction layer for storing and retrieving application-specific data like preferences or runtime state. These values may be stored in the registry, INI files, XML files, or some other place according to platform convention. If your native client application needs local storage beyond key/value pairs, you can embed your own database, invent your own file format, or any number of other solutions.  

HTML5 storage is a way for web pages to store named key/value pairs locally, within the client web browser. Like cookies, this data persists even after you navigate away from the web site, close your browser tab, exit your browser, or what have you. Unlike cookies, this data is never transmitted to the remote web server (unless you go out of your way to send it manually). Unlike all previous attempts at providing persistent local storage, it is implemented natively in web browsers, so it is available even when third-party browser plugins are not.  

You can check!  
function supports_html5_storage() {  
  try {  
    return 'localStorage' in window && window['localStorage'] !== null;  
  } catch (e) {  
    return false;  
  }  
}  
Instead of writing this function yourself, you can use Modernizr to detect support for HTML5 Storage.  

if (Modernizr.localstorage) {  
  // window.localStorage is available!  
} else {  
  // no native support for HTML5 storage :(  
  // maybe try dojox.storage or a third-party solution  
}  

## Using that storage  
HTML5 Storage is based on named key/value pairs. You store data based on a named key, then you can retrieve that data with the same key. The named key is a string. The data can be any type supported by JavaScript, including strings, Booleans, integers, or floats. However, the data is actually stored as a string. If you are storing and retrieving anything other than strings, you will need to use functions like parseInt() or parseFloat() to coerce your retrieved data into the expected JavaScript datatype.  

interface Storage {  
  getter any getItem(in DOMString key);  
  setter creator void setItem(in DOMString key, in any data);  
};  

SQL- In 2007, Google launched Gears, an open source cross-browser plugin which included an embedded database based on SQLite. This early prototype later influenced the creation of the Web SQL Database specification. Web SQL Database (formerly known as “WebDB”) provides a thin wrapper around a SQL database, allowing you to do things like this from JavaScript:  
openDatabase('documents', '1.0', 'Local document storage', 5*1024*1024, function (db) {  
  db.changeVersion('', '1.0', function (t) {  
    t.executeSql('CREATE TABLE docids (id, name)');  
  }, error);  
});