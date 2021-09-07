# API Deployment

## Configuring Django Settings: Best Practices

#### Managing Django Settings: Issues

* Different environments. Usually, you have several environments: local, dev, ci, qa, staging, production, etc. Each environment can have its own specific settings (for example: DEBUG = True, more verbose logging, additional apps, some mocked data, etc). You need an approach that allows you to keep all these Django setting configurations.

* Sensitive data. You have SECRET_KEY in each Django project. On top of this there can be DB passwords and tokens for third-party APIs like Amazon or Twitter. This data cannot be stored in VCS.

* Sharing settings between team members. You need a general approach to eliminate human error when working with the settings. For example, a developer may add a third-party app or some API integration and fail to add specific settings. On large (or even mid-size) projects, this can cause real issues.

* Django settings are a Python code. This is a curse and a blessing at the same time. It gives you a lot of flexibility, but can also be a problem – instead of key-value pairs, settings.py can have a very tricky logic.


#### Setting Configuration: Different Approaches
* There is no built-in universal way to configure Django settings without hardcoding them. But books, open-source and work projects provide a lot of recommendations and approaches on how to do it best. Let’s take a brief look at the most popular ones to examine their weaknesses and strengths.

**12 Factors** 
<br>

* 12 Factors is a collection of recommendations on how to build distributed web-apps that will be easy to deploy and scale in the Cloud. It was created by Heroku, a well-known Cloud hosting provider.

* As the name suggests, the collection consists of twelve parts:

    * Codebase
    * Dependencies
    * Config
    * Backing services
    * Build, release, run
    * Processes
    * Port binding
    * Concurrency   
    * Disposability
    * Dev/prod parity
    * Logs
    * Admin processes
* Each point describes a recommended way to implement a specific aspect of the project. Some of these points are covered by instruments like Django, Python, pip. Some are covered by design patterns or the infrastructure setup.

#### Django Settings: Best practices

* Keep settings in environment variables.

* Write default values for production configuration (excluding secret keys and tokens).

* Don’t hardcode sensitive settings, and don’t put them in VCS.

* Split settings into groups: Django, third-party, project.

* Follow naming conventions for custom (project) settings.

## SSH 

**What is SSH**: SSH, or Secure Shell, is a remote administration protocol that allows users to control and modify their remote servers over the Internet. The service was created as a secure replacement for the unencrypted Telnet and uses cryptographic techniques to ensure that all communication to and from the remote server happens in an encrypted manner. It provides a mechanism for authenticating a remote user, transferring inputs from the client to the host, and relaying the output back to the client.