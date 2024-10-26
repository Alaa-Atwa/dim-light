# dim-light
settings the brightness of your monitor to your desired percent, also adjusting jamma so you can reduce blue light at night.

## Description

this scripts helps to set the level of brightness and jamma for your monitor, the main tool is xrandr.
you can add this scripts to crontabs to run automatically with specified values for night for example.

## Table of Contents
- [Installation](#installation)
- [Usage](#usage)

## installation
1. Clone the repository:
  ```bash
  git clone git@github.com:Alaa-Atwa/dim-light.git
  ```
2. Install dependencies:
  1. xrandr 
  ```bash
  sudo apt install xrandr || sudo apt install x11-xserver-utils
  ```
  2. notify-send
  ```bash
  sudo apt install notfiy-send
  ```
  

