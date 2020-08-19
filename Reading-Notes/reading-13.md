# Local Storage

[Website:](http://diveinto.html5doctor.com/storage.html)
<br>

Local storage is advantageous over things like cookies because they have layers of abstraction and can load quicker than anything else. Cookies can also bog down processing time in your waterfall. Cookies also send unencrypted data over the internet which is dangerous to the user. Cookies are also limited to 4kb of data. What we really want is alot of storage space on the clients side that persists beyond a page refresh and isnt transmitted to the server. 
<br>

HTML5 storage is based on named key/value pairs. You store data based on a named key, then you can retrieve that data with the same key. The named key is a string. The data can be any type supported by Javascript, including strings, booleans, integers, or floaters. However, the data is actually stored as a string. If you are storing and retrieving anything other than a string, you will need to use functions like parseInt() or parseFloat() to coerce your retrieved data into the expected JS datatype. 

[Back To Homepage](https://leethomas13.github.io/201-reading-notes/)