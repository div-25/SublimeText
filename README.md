# SublimeText
Snippets and setup for competitive programming

Instructions to ready everything assuming 64 bit Windows

If you don't have mingw installed (i.e. you can't run g++ from console), do the following.

1. Install mingw64 from https://www.msys2.org/ . Follow all the steps carefully.
2. Add mingw64/bin to your environment path variable. 
In the Windows search bar, type 'settings' to open your Windows Settings.
Search for Edit environment variables for your account.
Choose the Path variable and then select Edit.
Select New and add the Mingw-w64 destination folder path to the system path. The exact path depends on which version of Mingw-w64 you have installed and where you installed it. If you used the settings above to install Mingw-w64, then add this to the path: C:\msys64\mingw64\bin.
Select OK to save the updated PATH. You will need to reopen any console windows for the new PATH location to be available.

To check that your Mingw-w64 tools are correctly installed and available, open a new Command Prompt and type:

g++ --version
gdb --version
If you don't see the expected output or g++ or gdb is not a recognized command, make sure your PATH entry matches the Mingw-w64 binary location where the compilers are located. If the compilers do not exist at that PATH entry, make sure you followed the instructions on the MSYS2 website to install Mingw-w64.

Now that you can build C++ programs, install and set up your editor.

1. Install Subilme Text 3 from https://www.sublimetext.com/3 (choose Windows 64 bit)
2. Download all the code from this repo and extract the files to a folder similar to C:\Users\<user-id-or-name>\AppData\Roaming\Sublime Text 3\Packages\User
If you can't find this folder, open Sublime Text, go to Tools > Developer > New Snippet. Click somewhere on the file that opens and click Ctrl + O. A User folder will open. If not, cancel and do Ctrl + O again. Copy the path to this folder. This is where all the files should reside.
3. Create a folder where all your codes will reside. Say, D:/Codes. Move/create the files "inputf.in" and "outputf.in" to this folder. To write code, click Ctrl + N and save as .cpp file in this folder (D:/Codes)
4. Set up the layout. Open Sublime Text and go to View > Layout > Columns 3. Again go to View > Groups > Max Column 2. Open "inputf.in" in top row of second column and "outputf.in" in bottom row of second column.
5. Open your "code.cpp" file in the bigger column. Now "inputf.in" will be your standard input and "outputf.in" will print your output. Go to Tools > Build System > cpp_io.
6. Build by running Ctrl + B on your .cpp file. You should be able to use snippets in any .cpp file. Clear everything and write "compi" and press Enter. You're ready to code!
