# BoardManagerFiles
Storage for Arduino Boards Manager JSON and package files etc

For more information see the [Wiki](https://github.com/stm32duino/wiki/wiki/). Mainly the [Getting Started page](https://github.com/stm32duino/wiki/wiki/Getting-Started).

## Troubleshooting

If you have any issue to download/use a package, you could [file an issue on Github](https://github.com/stm32duino/BoardManagerFiles/issues/new).

Or submit a topic on the [stm32duino forum](http://stm32duino.com):

 * questions on the [STM32 Core](http://stm32duino.com/viewforum.php?f=48)

 * bugs/enhancements on the [STM core: Bugs and enhancements](http://stm32duino.com/viewforum.php?f=49)

## How to generate/update board jason file

Enter the `STM32/src` directory. Clone the Arduino core and the Arduino Tools repositories into the src directory.

```
git clone https://github.com/stm32duino/Arduino_Core_STM32.git STM32
git clone https://github.com/stm32duino/Arduino_Tools.git STM32Tools
```

Now you should be able to run `./dopackage.sh`. This will generate new tarballs and will update the board file json file.

If you are on Mac OS you will need to install some additional tools:

```
brew install coreutils gnu-tar findutils gnu-sed
```
