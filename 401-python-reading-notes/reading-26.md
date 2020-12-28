[Django Settings Best Practices](https://djangostars.com/blog/configuring-django-settings-best-practices/)

Setting Configuration: Different Approaches
There is no built-in universal way to configure Django settings without hardcoding them. But books, open-source and work projects provide a lot of recommendations and approaches on how to do it best. Let’s take a brief look at the most popular ones to examine their weaknesses and strengths.

ALLOWED_HOSTS = ['example.com']
DEBUG = False
DATABASES = {
    'default': {
        'ENGINE': 'django.db.backends.postgresql',
        'NAME': 'production_db',
        'USER': 'user',
        'PASSWORD': 'password',
        'HOST': 'db.example.com',
        'PORT': '5432',
        'OPTIONS': {
            'sslmode': 'require'
        }
    }
}

...

from .settings_local import *

Separate settings for each enviroment:
settings/
   ├── __init__.py
   ├── base.py
   ├── ci.py
   ├── local.py
   ├── staging.py
   ├── production.py
   └── qa.py


from .base import *


ALLOWED_HOSTS = ['localhost']
DEBUG = True
DATABASES = {
    'default': {
        'ENGINE': 'django.db.backends.postgresql',
        'NAME': 'local_db',
        'HOST': '127.0.0.1',
        'PORT': '5432',
    }
}

12 Factors
12 Factors is a collection of recommendations on how to build distributed web-apps that will be easy to deploy and scale in the Cloud. It was created by Heroku, a well-known Cloud hosting provider.

As the name suggests, the collection consists of twelve parts:

Codebase
Dependencies
Config
Backing services
Build, release, run
Processes
Port binding
Concurrency
Disposability
Dev/prod parity
Logs
Admin processes

Django Settings: Best practices
Keep settings in environment variables.
Write default values for production configuration (excluding secret keys and tokens).
Don’t hardcode sensitive settings, and don’t put them in VCS.
Split settings into groups: Django, third-party, project.
Follow naming conventions for custom (project) settings

Conclusion
The Settings file is a small but very important part of any Django project. If you do it wrong, you’ll have a lot of issues during all phases of development. But if you do it right, it will be a good basis for your project that will allow it to grow and scale in the future.

Using the environment variables approach, you can easily switch from a monolith to microservice architecture, wrap your project in Docker containers, and deploy it in any VPS or Cloud hosting platform such as: Amazon, Google Cloud, or your own Kubernetes cluster.

[SSH Tutorial](https://www.hostinger.com/tutorials/ssh-tutorial-how-does-ssh-work)

What is SSH
SSH, or Secure Shell, is a remote administration protocol that allows users to control and modify their remote servers over the Internet. The service was created as a secure replacement for the unencrypted Telnet and uses cryptographic techniques to ensure that all communication to and from the remote server happens in an encrypted manner. It provides a mechanism for authenticating a remote user, transferring inputs from the client to the host, and relaying the output back to the client.

Three Different Encryption Types:
Symmetrical encryption
Asymmetrical encryption
Hashing.

Symmetrical Encrpytion
The process of creating a symmetric key is carried out by a key exchange algorithm. What makes this algorithm particularly secure is the fact that the key is never transmitted between the client and the host. Instead, the two computers share public pieces of data and then manipulate it to independently calculate the secret key. Even if another machine captures the publically shared data, it won’t be able to calculate the key because the key exchange algorithm is not known.

Asymmetrical Encryption
Unlike symmetrical encryption, asymmetrical encryption uses two separate keys for encryption and decryption. These two keys are known as the public key and the private key. Together, both these keys form a public-private key pair.

Hashing
One-way hashing is another form of cryptography used in Secure Shell Connections. One-way-hash functions differ from the above two forms of encryption in the sense that they are never meant to be decrypted. They generate a unique value of a fixed length for each input that shows no clear trend which can exploited. This makes them practically impossible to reverse.

Exchange Algorithm
Both the client and the server agree on a very large prime number, which of course does not have any factor in common. This prime number value is also known as the seed value.
Next, the two parties agree on a common encryption mechanism to generate another set of values by manipulating the seed values in a specific algorithmic manner. These mechanisms, also known as encryption generators, perform large operations on the seed. An example of such a generator is AES (Advanced Encryption Standard).
Both the parties independently generate another prime number. This is used as a secret private key for the interaction.
This newly generated private key, with the shared number and encryption algorithm (e.g. AES), is used to compute a public key which is distributed to the other computer.
The parties then use their personal private key, the other machine’s shared public key and the original prime number to create a final shared key. This key is independently computed by both computers but will create the same encryption key on both sides.
Now that both sides have a shared key, they can symmetrically encrypt the entire SSH session. The same key can be used to encrypt and decrypt messages (read: section on symmetrical encryption).


[Back To Homepage](https://leethomas13.github.io/201-reading-notes/)