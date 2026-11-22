# Roller

Roller is a Java-based, full-featured, multi-user and group-blog server
suitable for blog sites large and small. Roller is typically run with
Apache Tomcat and MySQL.
Roller is made up of the following Maven projects:

* _roller-project_:         Top level project
* _app_:                    Roller Weblogger webapp, JSP pages, Velocity templates
* _assembly-release_:       Used to create official distributions of Roller
* _docs_:                   Roller documentation in ODT format
* _it-selenium_:            Integrated browser tests for Roller using Selenium

## Documentation

The User and Template Guides are in `docs/`, in ODT format (for
OpenOffice or LibreOffice). Building, configuring and running the webapp
on Tomcat is described in `AGENTS.md`.

## Quick start

Assuming you've got a UNIX shell, Java and Maven:

Build and test the code:

    $ mvn clean install

Run Roller in Jetty with Derby database:

    $ cd app
    $ mvn jetty:run

Browse to http://localhost:8080/roller
