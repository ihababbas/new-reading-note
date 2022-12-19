# Class 29
## API Deployment

### Django Settings Best Practices

* When dealing with Django settings there are some minor issues to be aware of and account for like.
  - It can be helpful to have multiple environments because each one can have it's own settings.
  - There is also sensitive data like the secret key, DB passwords, and tokens.
  - There is the need to account for human error when sharing settings between teammates
  - Django settings are python code and because of this instead of the settings being composed of key-value pairs they can sometimes have tricky logic
* The most popular approaches to dealing with this are
   - Use a settings_local.py file that is extended for all environment specific settings.
      - It has the pro of not storing secrets in VCS, but some settings can be lost with this method and it requires an example file for other developers to take advantage of it.
   - Have separate setting files for each environment where you have a shared settings directory that has the different versions of the setting file for use.
      - This approach is easy to share and has all environments in VCS, but in needs a special way to handle secrets and the inheritance of settings.
   - Use environment variables.
      - This solves the sensitive data issue, and has many pros with the only con being the developer handling of sharing the default configs.
   - There is a collection of recommendations for how to build a distributed web app that is easy to deploy and scale in the cloud and was created by Heroku.
        The twelve parts are;
        1. Codebase
        2. Dependencies
        3. Config
        4. Backing services
        5. Build, release, run
        6. Processes
        7. Port binding
        8. Concurrency
        9. Disposability
        10. Dev/prod parity
        11. Logs
        12. Admin processes
  - Each point is a recommended way to implement a specific part of the project and some are covered by instruments like Django, Python, pip and others. Some are covered by design patterns or infrastructure setup.
  - One main rule is to store configuration in the environment.
* The previous main Python method for using environment variables is os.environ but it can be tricky to use and requires extra effort to deal with errors. Nowadays, it is more recommended to use django-environ which is technically a merge of 6 other things.
  - It provides a well functioning API for reading values from ENVs or text files and has type conversion
* One thing that you can do is split settings by source rather than environments.

* Another suggestion is to follow three rules for naming conventions;
  - Give meaningful names
  - Use a prefix with the project name in custom project settings
  - Write descriptions for settings in comments.
* So in conclusion;
  - Keep settings in ENVs
  - Write default values for the production config(excluding secrets)
  - Don't hardcode sensitive settings and don't put them in VCS
  - Split settings by group
  - Follow naming conventions.




### SSH Tutorial

* Secure Shell Protocol(SSH) is a administration protocol that allows users to access, control, and modify their remote servers.
* It was created as a secure replacement for Telnet and uses cryptographic techniques to ensure communications are encrypted.
* The advantage for SSH over the previous methods is the ability to encrypt and ensure a secure transfer of information between host and client.

* There are three main encryption technologies;

  - Symmetrical Encryption
  - Asymmetrical Encryption
  - Hashing

* SSH works by using the client-server model to allow for authentication between two remote systems and encrypt the data passed between them.
* SSH defaults to TCP port 22 and the host listens for connections on port 22.
* The client must begin the connection by initiating the TCP handshake to ensure a secured symmetric connection and verify if the identity displayed matches previous records and presents the required credentials.
* When the client attempts a connection, the server presents the protocols and the versions it supports. If the client has a matching protocol and version an agreement is reached and the connection is started with that protocol.
* Once the connection is established, it uses the Diffie-Hellman Key Exchange Algorithm to create a symmetrical key and is used by the client and server to arrive at a shared key that is used for the session.
* After the algorithm generates the shared key, the final stage before access is granted is authenticating the credentials.
  - Most users use a password and are asked for the corresponding username and password.