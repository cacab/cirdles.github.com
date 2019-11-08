---
layout: project-page
help: topsoil
title: Onboarding Tutorial
category: Help
reference: OnboardingTutorial
---

## Step 1: Clone Topsoil from GitHub

1. Navigate to the [Topsoil GitHub Repo](https://github.com/CIRDLES/Topsoil)

2. copy and paste this into your terminal: 

`git clone https://github.com/CIRDLES/Topsoil.git` 

## Step 2: Utilizing Topsoil

There are a few different ways to display and utilize the topsoil repository on your computer. If you’re using an integrated development environment (IDE), the project import process will depend on which one you have. 

Topsoil uses Gradle as a build tool. The main class of Topsoil is located in Topsoil/app/src/main/java/org/cirdles/topsoil/app/ and is called MainWindow.java.

1. Terminal (classic)

     * Once you have the source code, navigate to the root directory in a terminal and execute the command
`./gradlew build`. This will import the required resources and build Topsoil. 

     * After that, you can create a JAR file by running `./gradlew jarWithDependencies`.

          Here is what my terminal looks like: <img src="/assets/images/topsoil-imgs/TerminalDownloadScreen.png" width="100%">

     * Download your [Java JDK](https://www.oracle.com/technetwork/java/javase/downloads/jre8-downloads-2133155.html) (this might require account creation, but it is complimentary)

     * The resulting JAR file will be in Topsoil/app/build/libs with the name topsoil-[version].jar. (Typically the largest one) <img src="/assets/images/topsoil-imgs/JARFileLocation.png" width="100%">

     
     * Open jar file by double-clicking or typing “ java -jar topsoil-[version].jar” into the command line

2. NetBeans

     * Download [Netbeans](https://netbeans.apache.org/download/index.html) (Version 8.2)

          * What is it?

               * “NetBeans IDE lets you quickly and easily develop Java desktop, mobile, and web applications, as well as HTML5 applications with HTML, JavaScript, and CSS. The IDE also provides a great set of tools for PHP and C/C++ developers. It is free and open-source and has a large community of users and developers around the world.”

     * [Instructions on Installing NetBeans](https://netbeans.org/community/releases/82/install.html)

     * [Download & Install Gradle Plugin](http://plugins.netbeans.org/plugin/44510/gradle-support) (Make sure it is for Netbeans 8.2)
          * What is it?
               * open-source build automation tool that is designed to be flexible enough to build almost any type of software (gradle.org)
          * Why do we use it?

               * Gradle models its builds as Directed Acyclic Graphs (DAGs) of tasks (units of work). What this means is that a build essentially configures a set of tasks and wires them together — based on their dependencies — to create that DAG. Once the task graph has been created, Gradle determines which tasks need to be run in which order and then proceeds to execute them. (gradle.org)

          * How to build gradle projects from terminal? (generic commands)

               * `gradle` To see what version we have installed 

               * `gradle clean build` To build out your gradle project         
               
     * [Download & Install SceneBuilder Plugin](https://docs.oracle.com/javafx/scenebuilder/1/installation_1-1/jsbpub-installation_1-1.htm)

     * [Scene Builder Installation Tutorial](https://www.youtube.com/watch?v=dQSTffLSSZY)

     * Open the Topsoil Project
              
          * File > Open > Topsoil (go to the location where Topsoil is cloned on your computer

          * This is what your screen should look like <img src="/assets/images/topsoil-imgs/FinalNetBeansScreen.png" width="100%">