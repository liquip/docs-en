# Installation
To install the plugin you currently need to build it by yourself. In the following guide you will be taught to do so step by step.

## Prerequisites
To build the plugin you need the following:
* Java 17 or higher
* Git

## Installing Java
To install Java you can go to [Adoptium](https://adoptium.net). They provide prebuilt Java-binaries and even installers for Java.

## Installing Git
To install Git you can go to <https://git-scm.com/downloads> and install git from there.

## Setup
To set up the project you first need to clone the repository. To do so create a directory somewhere and open your terminal there and run the following command:
```sh
git clone https://github.com/liquip/liquip-plugin.git .
```
This will clone the repository into the current directory. Note that the directory must be empty to do so.

## Building
To now build the plugin you run the following command in the directory you cloned to:

For Linux / macOS:
```sh
./gradlew build
```
For Windows:

```bat
.\gradlew.bat build
```
If you have the gradle-cli installed you may also run the following:
```sh
gradle build
```
This should start gradle and build the plugin. The plugin is seperated into three submodules, being 'core', 'example-plugin' and 'gui'. The core-module is the Liquip-plugin. The example-plugin contains some experimental features. The gui-module contains the code for the inventory-guis. All three modules will be built but you most likely are just interested in the core-module. The output can be found in the `core/build/libs` directory. You want to take the jar-file without any '-dev' or '-all' in it and put it inside your plugins-directory.
