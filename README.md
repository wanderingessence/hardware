# hardware
Altium repository for pod V. This project is set up to provide all documentation, design and data validation required for the Badgerloop Pod V PCBs. This repository builds off of our previous work the podiv-altium repository. 

## Prerequisites
Altium only works on Windows. See  [Altium System Requirements](https://www.altium.com/documentation/18.0/display/ADES/Altium+Designer+-+((System+Requirements))") for more information. An internet connection is required to connect to the license server and dual monitors are nice to have. Microsoft Excel is required for BOM generation.

## Installation
1. Contact Ezra Boley, Shelby Riggleman or Ryan Castle to be added to the Badgerloop Team AltiumLive Account and the Badgerloop [Github](https://github.com/badgerloop-software"). You will receive an email from Altium with your account information. You may continue to step to step 8 without requiring an active license. If there is a delay for some reason, you can work on Altium training and practice on CAE computers or through [Citrix](https://remote.engr.wisc.edu/vpn/index.html), but we are usually able to add new users within 24 hours. CAE currently runs Altium 16, which has similar features but has a different interface and some bugs. Badgerloop currently supports Altium 19.0.10. 
2. Download the latest version of [Altium Designer](https://www.altium.com/products/downloads) 
3. Install Altium. Default file paths will work.
4. Insall [Git Bash](https://gitforwindows.org/") Git Bash (or whatever BASH emulation tool you are comfortable with)
5. Open Git Bash
6. Type the following commands into the command prompt window:
   + cd ../..
   + mkdir git
   + cd git
   + git clone https://github.com/badgerloop-software/hardware.git
   + cd hardware
   + git checkout -b <your-username_training>
   + Open Altium and sign in. You are now on a training branch that you will complete your first getting started project on if you are new to Altium. 
7. Go to User (Silhouette in the top right corner) -> License Management. Then Click Sign In and enter your username and password associated with Altium Live and accept the warning. It's also a good idea to check Sign me in when I start Altium Designer if you'd like to save a little time.

_NOTE: If you go click "Sign In" directly from User, you will be asked for a server address. This is not what you want. Go back to step 7 and hit License Management instead of Sign In._ 

8. Click Use to claim a license. If you are not using a valid license, you will be able to view files in Altium Designer but you will not be able to make edits. Ensure that you are choosing an Altium Designer License and not our PDN License. That's something else. 
9. You are now ready to use Altium. See [Training](#training) for more details on how to get started. 

## Training
+ View the [Badgerloop Altium Presentation](https://uwmadison.box.com/s/2sdt8kfaeyde04sg8edn62u7vtrdsiyx") for a getting started project. You can work locally for this project. Git-specific training will be posted at a later date. 
+ If you are new to using Git, read through the [Altium Git Guide](https://uwmadison.app.box.com/file/324684243638) which provides some common commands to get you started. 
+ Multivibrator Project: The Multivibrator Project from Altium is hands down the best training resource for getting started with Altium. We ask that everyone new to PCB design complete this tutorial on their own prior to working on Badgerloop schematics or boards. While we want to help everyone as much as possible, it's on you to get a bit of a background. Feel free to ask Ezra, Shelby or Ryan if you have any issues with the tutorial. [Multivibrator Tutorial] (https://www.altium.com/documentation/18.0/display/ADES/From+Idea+to+Manufacture+-+Driving+a+PCB+Design+through+Altium+Designer). This guide goes "From Idea to Manufacture" and drives a design all the way though rough-drawing your circuit, making library symbols and footprints, schematic capture, placement, layout, and routing, as well as manufacturing outputs. 

## Github Basics
TODO @Kevin 

## Acknowledgements
+ [Altium](www.altium.com), for being an amazing sponsor! 
+ Dave Jones of the EEVBlog, as we'd have no idea what we were doing without his videos.
