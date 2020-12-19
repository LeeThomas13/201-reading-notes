[Beginners Guide to Docker](https://wsvincent.com/beginners-guide-to-docker/)

Docker is a way to runn entire appllications. No longer have to mess around with venv's. Downside to that is that it is complex.

Containers VS VENV's
Virtual environments are used to isolate Python software packages locally. We can create an isolated box for individual projects so one can use Python 2.7 and Django 1.5 while another can use Python 3.5 and Django 2.1 on the same computer. Virtual environments are great.

Also we can’t run a production database or other services within virtual environments so compared to Docker containers they are far more limited.

Docker must be installed.

You can use docker for images, Image libraries, Image layers, etc.

Conclusion
That last example with Django probably felt a bit too fast to fully understand. And that’s ok. I wanted to show a working example without getting too bogged down in the complexity of images and containers.

The important takeaways from this tutorial are this:

Docker is a way to run Linux containers
Containers are a lightweight alternative to Virtual Machines
Dockerfile is a list of instructions for creating an image
Images are made up of one or more layers
Containers are a running instance of an image
docker-compose.yml controls how to run the container
Containers are stateless and ephemeral in nature. We can link the local filesystem via volumes but things become more complex with databases (which we didn’t cover here).

[Django API's Library](https://djangoforapis.com/library-website-and-api/)

Serializers
A serializer translates data into a format that is easy to consume over the internet, typically JSON, and is displayed at an API endpoint. We will also cover serializers and JSON in more depth in following chapters. For now I want to demonstrate how easy it is to create a serializer with Django REST Framework to convert Django models to JSON.

cURL
We want to see what our API endpoint looks like. We know it should return JSON at the URL http://127.0.0.1:8000/api/. Let’s ensure that our local Django server is running:

(library) $ python manage.py runserver
Now open a new, second command line console. We will use it to access the API running in the existing command line console.

We can use the popular cURL program to execute HTTP requests via the command line. All we need for a basic GET request it to specify curl and the URL we want to call.

Browsable API
With the local server still running in the first command line console, navigate to our API endpoint in the web browser at http://127.0.0.1:8000/api/.



[Back To Homepage](https://leethomas13.github.io/201-reading-notes/)