# Update and Delete

[Link to Article](https://developer.mozilla.org/en-US/docs/Learn/HTML/Forms/Sending_and_retrieving_form_data)


The GET method is the method used by the browser to ask the server to send back a given resource: "Hey server, I want to get this resource." In this case, the browser sends an empty body. Because the body is empty, if a form is sent using this method the data sent to the server is appended to the URL.

The POST method is a little different. It's the method the browser uses to talk to the server when asking for a response that takes into account the data provided in the body of the HTTP request: "Hey server, take a look at this data and send me back an appropriate result." If a form is sent using this method, the data is appended to the body of the HTTP request.

PHP offers some global objects to access the data. Assuming you've used the POST method, the following example just takes the data and displays it to the user. Of course, what you do with the data is up to you. You might display it, store it into a database, send it by email, or process it in some other way.


There are many other server-side technologies you can use for form handling, including Perl, Java, .Net, Ruby, etc. Just pick the one you like best. That said, it's worth noting that it's very uncommon to use these technologies directly because this can be tricky. It's more common to use one of the many high quality frameworks that make handling forms easier, such as:

Django for Python (a bit more heavyweight than Flask, but with more tools and options).
Express for Node.js.
Laravel for PHP.
Ruby On Rails for Ruby.
It's worth noting that even using these frameworks, working with forms isn't necessarily easy. But it's much easier than trying to write all the functionality yourself from scratch, and will save you a lot of time.


<form method="post" action="https://www.foo.com" enctype="multipart/form-data">
  <div>
    <label for="file">Choose a file</label>
    <input type="file" id="file" name="myFile">
  </div>
  <div>
    <button>Send the file</button>
  </div>
</form>



Be paranoid: Never trust your users
So, how do you fight these threats? This is a topic far beyond this guide, but there are a few rules to keep in mind. The most important rule is: never ever trust your users, including yourself; even a trusted user could have been hijacked.

All data that comes to your server must be checked and sanitized. Always. No exception.

Escape potentially dangerous characters. The specific characters you should be cautious with vary depending on the context in which the data is used and the server platform you employ, but all server-side languages have functions for this. Things to watch out for are character sequences that look like executable code (such as JavaScript or SQL commands).
Limit the incoming amount of data to allow only what's necessary.
Sandbox uploaded files. Store them on a different server and allow access to the file only through a different subdomain or even better through a completely different domain.
You should avoid many/most problems if you follow these three rules, but it's always a good idea to get a security review performed by a competent third party. Don't assume that you've seen all the possible problems.

[Back To Homepage](https://leethomas13.github.io/201-reading-notes/)