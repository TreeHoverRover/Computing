# Background
A rover based on a version of the Sawppy project, Curio. Plan is to experiment with robotic movement, sensing, data collection and analysis in under-the-canopy surveys for optimised woodland mensuration initially. The build process requires hardware and software setup which is the topic of the following guidelines. Information on how to setup the Raspberry Pi and the ROS was mostly taken from [here](https://www.intorobotics.com/how-to-install-ros-melodic-rosserial-and-more-on-raspberry-pi-4-raspbian-buster/).

# Raspberry Pi
The Raspberry Pi 4 Model B 8GB is the computer of choice to *manage hardware components and run algorithms to control the robot*. At the time of writing, this version is capable of running ROS, algorithms to detect objects, and deep learning algorithms. 

## List of components
* Raspberry Pi 4 Model B with 8GB of RAM
* Power Supply 5V 3A USB-C adapter (used the one from my smartphone)
* An unofficial 1TB MicroSD card (PNY)
* Full-size USB adapter for the microSD card
* A keyboard and a mouse
* A screen with HDMI input

## How to install Raspberry Pi OS on Raspberry Pi 4
In this part of the tutorial, we explain how to install Raspberry Pi OS on the Raspberry Pi 4. We choose to install this for two reasons:
1. It is the official operating system of the Raspberry Pi computers;
2. It is compatible with ROS Melodic. Melodic is a Long Term Support release which ends in 2023;

Raspberry Pi OS is a computer operating system officially provided by the Raspberry Pi Foundation as the primary operating system for the family of Raspberry Pi. The operating system includes a set of basic programs and utilities that helps you to develop and execute programs. It performs as a bridge between you and the hardware of Pi and manages the CPU, memory, memory disk, GPIO (General Purpose Input/Output) pins, and more.

Installing the Raspberry Pi  operating system has become much easier by using the Raspberry Pi Imager software. The program includes the option to erase and to write the microSD memory card used for Pi.

1. [Download](https://www.raspberrypi.org/software/) and install Raspberry Pi Imager to a computer with an SD card reader. Put the SD card you'll use with your Raspberry Pi into the reader and run Raspberry Pi Imager. We used the Windows version in this case.
**Note:** *If the memory card used is new, you don’t need to erase and format the card. Otherwise, you have to use the Raspberry Pi Imager to erase and format the card.*
2. Select the Raspberry Pi OS (32bit) as the Operating System, your SD card and click *write.
![install](https://user-images.githubusercontent.com/54486032/103786697-a1529f00-5034-11eb-9433-5fd7df63586c.png)
![done](https://user-images.githubusercontent.com/54486032/103786921-e5de3a80-5034-11eb-9e44-60554ada0315.png)

After the process of writing the image of the operating system on the memory card is finished, insert the microSD card into the Raspberry Pi’s slot and power up the board.


# How to communicate with Raspberry Pi

Enable SSH for remote access
Secure Shell (SSH) is a network protocol that allows us to operate the Pi board securely over an unsecured network like the internet. We can achieve this by logging into our Raspberry Pi via SSH using the user and the IP address from our laptop.

Using this service, we can run commands on Pi without needing to plug in a display, a keyboard, a mouse or moving ourselves to the location of the Raspberry Pi each time. This service is indispensible in the situation where the Pi board is running on a mobile robot like the one we are building.

