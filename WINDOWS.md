Network stats relies on pcapy, which is a bit tricky to install on Windows. It is recommended to use a Linux machine or virtual machine, if one is available.

These instructions have been adapted from and updated from https://github.com/helpsystems/pcapy/wiki/Compiling-Pcapy-on-Windows-Guide (do not follow these instructions, the relevant commands are below).

1. Install Wireshark as administrator
   1. Right click on the installer icon and select 'Run as administrator'
   2. When npcap install screen comes up, check the winpcap compatibility box

2. Install Python 3.8

3. Install Build Tools for Visual Studio 2019
   1. Download the tool: https://visualstudio.microsoft.com/downloads/ (open up Tools for Visual Studio 2019 then download Build Tools for Visual Studio 2019)
   2. Select C++ build tools

4. Download and extract WinPcap developer's pack (https://www.winpcap.org/devel.htm)

5. Add new system environment variable (not a user environment variable) WPDPACK_BASE with the value equal to the location of the WpdPack folder (including the WpdPack) extracted from step 4.

6. Open a new command line window as administrator and type 'pip install pcapy', followed by 'pip install impacket'

At this point, all prerequisites are installed and you should be ready to start running network stats.
