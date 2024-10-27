# dim-light
setting the brightness of your monitor to your desired percent, also adjusting jamma so you can reduce blue light at night.

## Description

this scripts helps to set the level of brightness and jamma for your monitor, the main tool is xrandr.
you can add this scripts to crontabs to run automatically with specified values for night for example.

## Table of Contents
- [Installation](#installation)
- [Usage](#usage)
- [Tips](#tips)

## installation
1. Clone the repository:
  ```bash
  git clone git@github.com:Alaa-Atwa/dim-light.git
  ```
2. Install dependencies:
  xrandr 
  ```bash
  sudo apt install xrandr || sudo apt install x11-xserver-utils
  ```
  notify-send
  ```bash
  sudo apt install notfiy-send
  ```
## Usage 
  ```bash
  ./bright [brightness] [gamma]
  ```
  basic usage: setting brightness level [0.1 : 1.0], one is for default brightness.
  ```bash
  ./bright .9
  ```
  setting brightness and jamma:
  jamma values are [red:green:blue], 1.0 for default value.
  ```bash
  ./bright .9 1.0:1.0:.85 
  # reducing the blue gamma to .85
  ```
  setting for night (reducing blue light)
  ```bash
  ./bright 1 night
  ```
  resetting values 
  ```bash
  ./bright 1 1
  ```
## Tips
1. you can add this script to your PATH 
  ```bash
  echo $PATH
  # just add "bright" file to one of these paths.
  ```
2. you can add this to run as a crontab at a specified time.
  ```bash
  crontab -e 
  # add the end of the crontabs and specify time to run "bright"
  ```




