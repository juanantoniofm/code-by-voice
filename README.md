code-by-voice
=============

In this repository you will find all the support files for my "code by voice" setup using Dragon Naturally Speaking and DragonFly. I was inspired to do this by Tavis Rudd (https://github.com/tavisrudd). You can see his excelent presentation from PyCon here: http://youtu.be/8SkdfdXWYaI

### !!! WORK IN PROGRESS !!!

## Requirements

This is the rough list of the software you are going to need. For the detailed installation order, please see below

* Dragnon Naturally Speaking - You can use any edition (including home). The advantage of using the Premium Edition, based on talking to the rep from Nuance, is that the Premium edition will let you backup the voice traning directly from DNS.
* Windows 8.1
* DragonFly
* Natlink / Unicode
* Python 2.7
* Virtualization Software (VMWare, VirtualBox, Parallels) if you are setting this up on Mac OS X or Linux

## Resources

* Dragon Naturally Speaking (http://www.nuance.com/dragon/index.htm)
* DragonFly (http://code.google.com/p/dragonfly/)
* Unimacro (http://qh.antenna.nl/unimacro/index.html)


## Getting Started

Here are the steps to get your system installed and running.

!!! These are a work in progress !!!

### Initial dependencies

1. Install Windows (8, 7 and XP work)
1. Install Dragon Naturally Speaking (and go through the training)
1. Download Python 2.7 for nat link (http://sourceforge.net/projects/natlink/files/pythonfornatlink/python2.7.zip/download), not any python
2. Extract the download
1. Install python-2.7
2. Install pywin32-218.win32-py2.7
3. Install PyXML-0.8.4.win32-py2.7
1. Install wxPython2.8-win32-ansi-2.8.12.1-py27
1. Add PATH enviroment variable for C:\Python27 and C:\Python27\Script (Right click on computer, click on Advanced system settings, click on Enviroment Variables)
1. Download easy_install.py (https://bitbucket.org/pypa/setuptools/raw/bootstrap/ez_setup.py)
2. Install easy_install.py with `python ez_setup.py`

### Installing NatLink and specific dependencies 

1. Download Natlink (http://qh.antenna.nl/unimacro/installation/installation.html)
2. Install Natlink (Just double click the installer)
1. Download DragonFly Zip File, not the windows installer (http://code.google.com/p/dragonfly/downloads/list)
1. Exract dragonfly-0.6.5.zip
1. Install DragonFly (inside the dragonfly-0.6.5 directory run "python setup.py install")
1. Enable Natlink via GUI (using the start menu). If it doesn't find your installation, try specifying the folders manually. The ini files directory refers to ..\All Users\%App Data%\Nuance\... , where you should find nssystem.ini

### Enabling custom scripts

1. Download the repo to a temporary location.

https://github.com/juanantoniofm/code-by-voice/archive/master.zip

2. Extract the zip file

3. Copy the content of the "macros" folder to the MacroSystem folder in your natlink installation (usually `C:\NatLink\NatLink\MacroSystem`)


### Ready to roll

1. Restart Dragon NaturallySpeaking

Look at the output of natlink.

If the window doesn't show up, make sure that natlink is properly enabled.

If you can not import dragonfly, make sure that your python path is correct, and that you can do so from a normal python repl



