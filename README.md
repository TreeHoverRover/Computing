# Background
A rover based on a version of the Sawppy project, Curio. Plan is to experiment with robotic movement, sensing, data collection and analysis in under-the-canopy surveys for optimised woodland mensuration initially. The build process requires hardware and software setup which is the topic of the following guidelines.

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
2. Insert your MicroSD card into the memory card adapter and insert that adapter into the card reader of your computer. **Note: *If the memory card used is new, you don’t need to erase and format the card. Otherwise, you have to use the Raspberry Pi Imager to erase and format the card.*



