go
==

[Go](https://golang.org/) is an open source programming language that makes it easy to build simple, reliable, and efficient software. You can easily add it to your Lando app by adding an entry to the `services` key in your app's `.lando.yml`.

Supported versions
------------------

*   [1.8.4](https://hub.docker.com/_/golang/)
*   **[1.8](https://hub.docker.com/_/golang/)** **(default)**
*   custom

Using patch versions
--------------------

While Lando does not "officially" support specifying a patch version of this service you can try specifying one using [overrides](https://docs.devwithlando.io/config/advanced.html#overriding-with-docker-compose) if you need to. **This is not guaranteed to work** so use at your own risk and take some care to make sure you are using a `debian` flavored patch version that also matches up with the `major` and `minor` versions of the service that we indicate above in "Supported versions".

[Here](https://hub.docker.com/r/library/golang/tags/) are all the tags that are available for this service.

Example
-------

{% codesnippet "./../examples/go/.lando.yml" %}{% endcodesnippet %}

You will need to rebuild your app with `lando rebuild` to apply the changes to this file. You can check out the full code for this example [over here](https://github.com/lando/lando/tree/master/examples/go).
