FOXX Applications
=================

Foxx is an easy way to create APIs and simple web applications from
within ArangoDB. It is inspired by Sinatra, the classy Ruby web
framework.

If you have created a nice Foxx application and you want to share it with
the community out there, clone this repository, add a short description
to the "applications" folder and issue a pull request.

"hello-foxx" is the hello world example for Foxx. Its 
[description file](https://github.com/arangodb/foxx-apps/blob/master/applications/hello-foxx.json)
can be found in the applications folder.

    {
      "description": "This is 'Hallo World' for ArangoDB Foxx.",
      "author": "Frank Celler",

      "versions": {
        "1.2.0" : { "type": "github", "location": "fceller/hello-foxx", "tag": "v1.2.0" }
      }
    }

The description file is a JSON document with the attributes:

* *description*: a short description of the application
* *author*: the name of the author, an email address, or a twitter handle
* *versions*: a list of available versions

In order to install this application into your local ArangoDB
installation, you can use the foxx-manager like this

    foxx-manager install hello-foxx /hello

This will download the application into your local installation of
ArangoDB (which must be up and running) and mount it under the path
"/hello".

If you now visit

    http://localhost:8529/hello

you should see a nice fox.
