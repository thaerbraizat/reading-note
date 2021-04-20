![LOCAL STORAGE](https://res.cloudinary.com/de4rvmslk/image/upload/f_auto,q_auto,w_1440/LocalStorage-cover_photo.png)
# LOCAL STORAGE BEFORE HTML5
there was only Internet Explorer,Microsoft invented a great many things and included them in their browser-to-end-all-browser-wars, 
Internet Explorer, One of these things was called *DHTML Behaviors*, and one of these behaviors was called *userData*.
# INTRODUCING HTML5 STORAGE
“HTML5 Storage” is a specification named Web Storage, which was at one time part of the HTML5 specification proper,
 but was split out into its own specification for uninteresting political reasons,
 Certain browser vendors also refer to it as *Local Storage* or *DOM Storage*.
* HTML5 Storage Simply put, it’s a way for web pages to store named key/value pairs locally, within the client web browser.
* From your JavaScript code, you’ll access HTML5 Storage through the localStorage object on the global window object.
* HTML5 Storage is based on named key/value pairs. You store data based on a named key, then you can retrieve that data with the same key. 
The named key is a string, the data can be any type supported by JavaScript, including strings, Booleans, integers, or floats. 
* The storage event is fired on the window object whenever setItem(), removeItem(), or clear() .
* Web SQL Database specification ,This specification has reached an impasse: all interested implementors have used the same SQL backend (Sqlite),
 but we need multiple independent implementations to proceed along a standardisation path. Until another implementor is interested in implementing this spec,
 the description of the SQL dialect has been left as simply a reference to Sqlite, which isn't acceptable for a standard.
* The Indexed Database API exposes what’s called an object store. An object store shares many concepts with a SQL database. There are **databases** with records,
 and each record has a set number of fields. Each field has a specific datatype, which is defined when the database is created.

### Resource
* [THE PAST, PRESENT & FUTURE OF LOCAL STORAGE FOR WEB APPLICATIONS](http://diveinto.html5doctor.com/storage.html)