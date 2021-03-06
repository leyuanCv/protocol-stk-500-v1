This project provides an Android implementation of the STK500 protocol, in order to be able to program a microcontroller board such as the bq ZUM or Arduino Uno by a Bluetooth connection.

This project is a gradle implementation for Android projects of the STK500-Android project created by the group Prosjekt2-09arduino. You can find the STK500-Android project here: 
https://github.com/Prosjekt2-09arduino/STK500-Android


===================
protocol-stk-500-v1
===================

protocol-stk-500-v1 is a library project to program a microcontroller board such as the bq ZUM or Arduino Uno by a Bluetooth connection. 

It allows you to program the microcontroller board without using avr-dude or any native code. 

There is an example project, SendHexToInoByBluetooth, where you can see how can the library be used. 
  
If you have any questions you can contact us through the `DIY forum <http://diy.bq.com/forums/forum/forum/>`_  or sending an email to diy@bq.com.


Usage
=====

#. Clone the repository::

    git clone https://github.com/bq/protocol-stk-500-v1.git

#. Install in your local repository::
  
    cd protocol-stk-500-v1/ProtocolSTK500v1_Library
    gradle publishToMavenLocal

#. Add your local repository to your root project's build.gradle file::

    repositories {
        mavenLocal()
    }

#. Add the protocol-stk-500-v1 dependency to your app's build.gradle file::

    dependencies {
        compile('com.bq.robotic:protocol-stk-500-v1:1.0@jar')
    }


Installation
============

#. Install `Android Studio <https://developer.android.com/sdk/installing/studio.html>`_ and `Gradle <http://www.gradle.org/downloads>`_.

#. If you use a 64 bits Linux, you will need to install ia32-libs-multiarch::

    sudo apt-get update
    sudo apt-get upgrade
    sudo apt-get install ia32-libs-multiarch 

#. Clone the repository::

    git clone https://github.com/bq/protocol-stk-500-v1.git

#. Install the drag-drop-grid library in your local repository::
  
    cd protocol-stk-500-v1/ProtocolSTK500v1_Library
    gradle publishToMavenLocal

#. In Android Studio go to ``File`` > ``Open`` and select the ProtocolSTK500v1_Library gradle project inside the previous cloned project (that with the green robot icon, the ProtocolSTK500v1_Library folder not the repository one with the example project inside too).

#. If your are going to use protocol-stk-500-v1 for one of your projects, follow the instructions of the `Usage section <https://github.com/bq/protocol-stk-500-v1#usage>`_ in order to installing it in your local repository and add to it the dependency needed.


Requirements
============

- `Java JDK <http://www.oracle.com/technetwork/es/java/javase/downloads/jdk7-downloads-1880260.html>`_ 

- `Android Studio <https://developer.android.com/sdk/installing/studio.html>`_ 

- `Maven <http://maven.apache.org/download.cgi>`_. If you use Ubuntu::
    
    sudo apt-get update
    sudo apt-get install maven

- `Gradle <http://www.gradle.org/downloads>`_ recommended version 1.10

- Arduino board


License
=======

drag-drop-grid is distributed in terms of LGPL license. See http://www.gnu.org/licenses/lgpl.html for more details.
