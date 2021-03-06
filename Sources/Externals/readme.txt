When building on Windows, external dependencies should be placed in this folder.

C++ headers go in the 'include' folder, grouped by product, except for zlib, which goes directly to the roof of the folder.
Libraries go in the 'lib' folder, without any subfolders.

This should be the resulting directory structure:

Externals
|   readme.txt
|   
+---include/
|   +---zconf.h
|   +---zlib.h
|   |   
|   +---curl/
|   |   \---(All curl headers)
|   |       
|   +---GL/
|   |   \---(All GL headers)
|   |       
|   \---SDL2/
|       \---(All SDL headers)
|           
\---lib/
        (All libs here)

In case you're too lazy to hunt the headers and libraries, you can also donload them for you version of Visual Studio.
They're already packed in the correct layout.

Visual Studio 2010:
https://dl.dropboxusercontent.com/u/37804131/OpenSpades-Externals-Windows.zip

Visual Studio 2015:
https://www.dropbox.com/s/pfvk8tns1qgkxpr/OpenSpades-Externals-Windows-VS2015.rar?dl=1
