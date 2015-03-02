## android-gradle-mulchannel-plugin

Gradle plugin for multiple channel apks

## Overview

This plugin generates multiple apks from different channel.
Generation has to be invoked as additions gradle task.

##Supported features

 * inputFile-config input file
 * tempDir-config unzip dir
 * outputDir-config output dir
 * channels-config multiple channels

##Use plugin

1.Use gradle install command,To install the plug in local maven

2.Add dependency to the top-level build.gradle file.
    ```
    buildscript {
        repositories {
            mavenLocal()
        }
        dependencies {
            classpath 'me.zhangls:mulchannel:0.0.1'
        }
    }
    ```

3.Apply plugin and add configuration to build.gradle of the application, eg:
    ```
    apply plugin: 'mulchannel'
    ```

4.Config mulchannel extension(inputFile,tempDir,outputDir,channels)

5.Use gradle mulchannel to make multiple channel apks

##License

MIT License
See LICENSE file.
