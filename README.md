MotionCam
---------

A quick project written in Python that utilizes a Raspberry-Pi and Camera to detect motion.
In short, it constantly captures images and compares the pixels' RGB values to identify motion. 
Once motion is detected, it logs the event and captures the image.
If consective images are captures, a video recording will occur.
User defines thresholds and other settings via **config.py**.


Prerequisites
-------------

Raspberry-Pi with Camera Module

Python3


Installation
------------

Before getting the installation started, be sure to update & upgrade your current packages
```
$ sudo apt-get update && sudo apt-get upgrade
```

Also be sure you have python-picamera library installed
```
$ sudo apt-get install python-picamera
```

To download the MotionCam project use the following:

git
```
$ git clone https://github.com/FancyJesse/motioncam
```


Usage
-----

Before executing the program, review and adjust any settings with **config.py**
```
$ cd
$ nano config.py
```

To execute the program, simply call **motioncam.py**
```
$ cd
$ ./motioncam.py
```

Ideally you will want the program to run in the background, enter the following command for this:
```
$ screen -d -m -S [screen-name] [application-to-run] 
```

To reattach the screen use:
```
$ screen -r [screen-name]
```

The program will continue running until the storage limit defined within **config.py** is reached. 

You can view the captured images and logs found in the directories defined within **config.py** as well.


Release History
---------------

* 0.3.0
    * Initial Release


License
-------

See the file "LICENSE" for information on the history of this software,
terms & conditions for usage, and a DISCLAIMER OF ALL WARRANTIES.


Authors
-------

FancyJesse