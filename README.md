<p align="center"><a href="https://auklet.io"><img src="https://s3.amazonaws.com/auklet/static/github_readme_java.png" alt="Auklet - Problem Solving Software for Java"></a></p>

# Auklet for Java
[![Maintainability](https://api.codeclimate.com/v1/badges/e1ced62442c7cf49d58a/maintainability)](https://codeclimate.com/github/aukletio/Auklet-Agent-Java/maintainability)

This is the Java agent for Auklet, officially supporting JVMs running Java 8+.
We test the agent on the Oracle JVM. 

# Features

* Automatic report of unhandled exceptions.
* Location, and system metrics identification for all issues.


# Quickstart

* Download the agent JAR using Maven or Gradle from https://bintray.com/aukletio/agent-java/auklet-agent-java.
* Initialize the agent at the very beginning of `main` using your app ID and API key:
```
import io.auklet.agent.Auklet;

public class demo {

   public static void main(String []arg) {
       Auklet.init(new Auklet.Config()
           .setAppId("...")
           .setApiKey("...")
       );
       ...
   }
}
```

* The agent needs a dedicated folder to create and store its configuration files. The agent will create these files 
on startup if they do not exist, or will use files that are already available on disk.

# Authorization

To authorize your application you need to provide both an API key and app ID.
These values are available in the connection settings of your application as well as during initial setup.

# Questions? Problems? Ideas?

To get support, report a bug or suggest future ideas for Auklet, go to https://help.auklet.io and click the blue button in the lower-right corner to send a message to our support team.
