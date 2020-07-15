# Santorini Board Game

<img src="gameLogo.png" width="300" height="300" />

Santorini is a highly accessible pure-strategy game where you play as a youthful Greek God or Goddess competing to best aid the island's citizens in building a beautiful village in the middle of the Aegean sea.

## Authors
| Personal Data | Username | Email |
|:-----------------------|:------------------------------------:|:------------------------------------:|
| Di Gennaro Marco | [@marcoDige](https://github.com/marcoDige) | marco1.digennaro@mail.polimi.it |
| De Bartolomeis Piersilvio | [@pierobartolo](https://github.com/pierobartolo) | piersilvio.debartolomeis@mail.polimi.it |
| Di Maio Alessandro | [@aledimaio](https://github.com/aledimaio) | alessandro1.dimaio@mail.polimi.it |

## Implemented functionality

| Functionality | State |
|:-----------------------|:------------------------------------:|
| Basic rules | [![GREEN](https://placehold.it/15/44bb44/44bb44)](#) |
| Complete rules | [![GREEN](https://placehold.it/15/44bb44/44bb44)](#) |
| Socket | [![GREEN](https://placehold.it/15/44bb44/44bb44)](#) |
| GUI | [![GREEN](https://placehold.it/15/44bb44/44bb44)](#) |
| CLI | [![GREEN](https://placehold.it/15/44bb44/44bb44)](#) |
| Multiple games | [![GREEN](https://placehold.it/15/44bb44/44bb44)](#) |
| Persistence | [![RED](https://placehold.it/15/f03c15/f03c15)](#) |
| Advanced Gods | [![GREEN](https://placehold.it/15/44bb44/44bb44)](#) |
| Undo | [![RED](https://placehold.it/15/f03c15/f03c15)](#) |

<!--
[![RED](https://placehold.it/15/f03c15/f03c15)](#)
[![YELLOW](https://placehold.it/15/ffdd00/ffdd00)](#)
[![GREEN](https://placehold.it/15/44bb44/44bb44)](#)
-->


## Instructions for build and execution:

The jar is the same for both server and client. You can build it under your preferred OS and launch it following the instructions below.
The project has been developed using JAVA 13 and JavaFX 14. 
The following terminals have been tested for the CLI: WSL (Ubuntu 18.04 and Debian), Windows Terminal and iTerm.

### Build instructions:

The jar is built using "Maven Shade Plugin", in IntelliJ IDE clone the repository and launch "install" under "lifecycle" section in Maven toolbar.
The generated jar will be placed in the "shade" folder in your project's root.

If you want use to Maven in the terminal execute:
```
mvn install
```
In the project's root folder (same folder of "pom.xml").
The generated jar will be placed in the "shade" folder in your project's root.

### Execution instructions:

#### Server

In terminal execute:

```
java -jar AM10.jar -server
```
The server will be execute listening on the default port ```1234```.

Execute in the terminal:

```
java -jar AM10.jar -server PORT
```

Where instead of ```PORT``` put the port number where you want the server to listen. Example: ```java -jar AM10.jar -server 8080```

#### Client

To launch the program in the command line interface (cli) first make sure you have the terminal in fullscreen,
then execute in the terminal (opened in the same folder where the jar is):

```
java -jar AM10.jar -client -cli
```

To launch the program with the graphical user interface (gui), double-click on the jar (on Ubuntu 20.04 first make sure to mark as executable the jar file).
You can also execute in the terminal:

```
java -jar AM10.jar -client -gui
```
or simply:
```
java -jar AM10.jar
```

## Note

- The pdf file "Unit test coverage" in "Deliverables" only serves to provide an overview and a small comment of the data on the test coverage.
- In "JARs" folder under "Deliverable" folder you can find the jars generated on different operating system.
