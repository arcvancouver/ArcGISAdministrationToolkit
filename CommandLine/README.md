-----------------------------------------------------------
How to add your own functions and rebuild the agsAdmin.exe
-----------------------------------------------------------
The agsAdmin.py has the code for the agsAdmin.exe file.
You can modify the setup.py file to control the creation of the .exe and not include Python dlls. (Make sure Python is installed on that machine if you do)


1) Modify the agsAdmin.py file with your own functions.

2) Download and install Py2exe: http://www.py2exe.org/
-This module allows the creation of an .exe from a python script
-Make sure you download the version specific to your version of Python (2.6, 2.7, etc)

3) The setup.py script has been provided as the template to creating a self-contained .exe. Update and modify if necessary

4) Run the following command from a command prompt: 
c:\myFolder>   c:\Python27\ArcGIS10.1\python.exe setup.py py2exe


5) The .exe will be created in the /dist folder under the directory of your setup.py/agsAdmin.py scripts
