# BYU CS340 Settlers of Catan

This is a web game that allows four players to play the Settlers of Catan game.

## Prerequisites

#### Oracle JDK 8

Oracle JDK 8 must be installed. This will *not* work with any later version or any other JDK implementation. To install it:

* Log into ```oracle.com```.

* Go to the downloads page

* Download the .tar.gz file for JDK 8. To do this, you'll have to accept the license agreement.

* ```$ cd ~/Downloads```

* ```$ sudo mkdir /opt/java```

* ```$ sudo tar zxvf jdk-8u241-linux-x64.tar.gz -C /opt/java8/```

* Add the following lines to your ```.bashrc```:

```
export JAVA_HOME="/opt/java8/jdk1.8.0_241"
export PATH="$PATH:$JAVA_HOME/bin"
```

* ```$ sudo ln -s /opt/java8/jdk1.8.0_241/bin/java /usr/bin/java```



## To Run the Server

```$ ant clean```

```$ ant jar-web-server```

```$ java -jar web-server.jar <port-num> <num-saves> <data-wipe> <storage>```

Parameters:

* port-num: Default is 8081

* num-saves: number of changes in state. default is 50.

* data-wipe: reset the persistent storage devices. Possible values are ```true``` or ```false```.

* storage: Values are ```file```, ```mongo```, ```sqlite```

## Play

* Locate the dashboard at `http://localhost:8081/index.html`

* Click login.html

* Register, create a game, and have fun

## Fork

Web version originally cloned from https://github.com/reedcwilson/catan
