# Tanxees Arena Edition
![Tank icon](https://github.com/dendygeeks/tanxees-arena/raw/master/tank-icon.png)

In this repository you can find the server and API for Java and Python languages.

## Building

To build the project, simply run
```
gradle copyJars
```
in the root directory. That will build everything and put into `target` directory.

## Running server

To run the server, go to its folder and there use
```
gradle run
```

## Hacking the dumb bot in Java

To use Java bot API, start with a sample `client.ai.java.dumb` project. To run the project,
enter the directory `client.ai.java.dumb` and type 
```
gradle run -PplayerId=bot1
```
(you may use `bot2` or `bot3` instead)

Start your own AI with modifying the `tanxees.client.ai.java.dumb.Main` class as you wish. Happy hacking!
