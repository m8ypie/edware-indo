# How to compile
## This is my best attempt to document the tangled mess that is edware compilation.
1. Within the folder win_tools, there are two folders 32 and 64. Choose the folder which corresponds to the version of windows you are currently running (i.e. 32 for 32 bit windows).
2. Run and install the files contained in the chosen folder in the following order:
    - python 2.7.7
    - wxPython
    - pywin
3. Exit the folder and unzip PyInstaller
4. Exit and enter the edware-indo folder
5. Download [get-pip.py](https://bootstrap.pypa.io/get-pip.py) to a folder on your computer. Open a command prompt window and navigate to the folder containing `get-pip.py`. Then run `C:\Python27\python.exe get-pip.py`. This will install `pip`.
6. Run the following commands in a cmd prompt 
    - ```C:\Python27\Scripts\pip.exe install dis3```
    - ```C:\Python27\Scripts\pip.exe install pefile```
    - ```C:\Python27\Scripts\pip.exe install pypiwin32```
7. Running the following command in a cmd prompt ```C:\Python27\python.exe edware.py``` edware should successfully run.
8. Finally run the following command from the edware-indo folder ```C:\Python27\python.exe win_tools\PyInstaller-2.1\PyInstaller-2.1\pyinstaller.py installer\edware-win.spec```