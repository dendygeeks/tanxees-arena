# Tanxees Arena Edition
![Tank icon](https://github.com/dendygeeks/tanxees-arena/raw/master/tank-icon.png)

First of all, to give this project a try, [download our release](https://github.com/dendygeeks/tanxees-arena/releases/tag/0.1-alpha).
It contains the UI client for this game (the only component which source isn't published here)

![Client screenshot](https://cloud.githubusercontent.com/assets/317189/15685211/cde2c34c-277b-11e6-990b-fa687f4b8915.png)



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

## Hacking the dumb bot in Python

To use Python bot API, start with a sample `client.ai.python.dumb` repository. To run the project do the following:
* Get new enough Python (2.7 or >=3.4 will do)
* Run "pip install websocket-client wsaccel"
* Launch the server
* Add full path to `client.ai.python/src` to `PYTHONPATH` environment variable (that's the directory that holds Python API, not yet available as a package), e.g. like this:
``` shell
export PYTHONPATH=/path/to/client.ai.python/src:$PYTHONPATH
```
* Launch "python Bot.py bot1"

Happy hacking! Start with Bot.py as a sample and create a fun-to-watch or clever AI.
