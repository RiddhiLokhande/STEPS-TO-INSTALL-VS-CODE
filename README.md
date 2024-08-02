
## Aim-Install Visual Studio Code

The steps to install Visual Studio Code (VS Code) using MinGW (Minimalist GNU for Windows).

## Prerequisites

- Windows operating system
- Administrator privileges
- Internet connection

## Step 1: Download and Install MinGW

1. **Download MinGW:**
   - Go to the MinGW official website: [MinGW](http://www.mingw.org/)
   - Click on the "Download Installer" button to download the MinGW installation manager.

2. **Install MinGW:**
   - Run the downloaded installer (`mingw-get-setup.exe`).
   - Click `Install` to proceed with the installation.
   - Choose the installation directory (default is `C:\MinGW`).
   - Once the installation is complete, launch the MinGW Installation Manager.

3. **Select Packages to Install:**
   - In the MinGW Installation Manager, mark the following packages for installation:
     - `mingw32-base`
     - `mingw32-gcc-g++`
     - `mingw32-gcc-objc`
   - To do this, right-click on each package and select `Mark for Installation`.

4. **Apply Changes:**
   - After marking the packages, click on `Installation` in the top menu and select `Apply Changes`.
   - Click `Apply` in the dialog that appears to start the installation process.
   - Wait for the installation to complete.

5. **Add MinGW to System Path:**
   - Open the Start menu, search for "Environment Variables" and select "Edit the system environment variables".
   - In the System Properties window, click on `Environment Variables`.
   - In the Environment Variables window, under `System variables`, find and select the `Path` variable, then click `Edit`.
   - Click `New` and add the path to your MinGW `bin` directory (e.g., `C:\MinGW\bin`).
   - Click `OK` to close all the windows.

## Step 2: Download and Install Visual Studio Code

1. **Download VS Code:**
   - Go to the Visual Studio Code official website: [Visual Studio Code](https://code.visualstudio.com/)
   - Click on the "Download for Windows" button to download the VS Code installer.

2. **Install VS Code:**
   - Run the downloaded installer (`VSCodeUserSetup-{version}.exe`).
   - Follow the installation wizard instructions to install VS Code.
   - Choose the installation location (default is usually fine).
   - Select the additional tasks you want (e.g., creating a desktop icon, adding to PATH).

3. **Launch VS Code:**
   - Once the installation is complete, launch VS Code from the Start menu or desktop icon.

## Step 3: Configure VS Code for MinGW

1. **Open VS Code and Install C/C++ Extension:**
   - Open VS Code.
   - Go to the Extensions view by clicking on the Extensions icon in the Activity Bar on the side of the window.
   - Search for "C/C++" and click `Install` on the Microsoft C/C++ extension.

2. **Configure VS Code to Use MinGW:**
   - Open the Command Palette (F1 or `Ctrl+Shift+P`).
   - Type `C/C++: Edit Configurations (UI)` and select it.
   - In the configurations UI, set the `compilerPath` to the path of your MinGW compiler (e.g., `C:/MinGW/bin/gcc.exe`).

3. **Create a New C++ Project:**
   - Open a new folder for your C++ project.
   - Create a new file with a `.cpp` extension (e.g., `main.cpp`).
   - Write your C++ code in this file.

4. **Build and Run Your C++ Code:**
   - Open the terminal in VS Code (``Ctrl+` ``).
   - Navigate to your project directory.
   - Compile your C++ code using the MinGW compiler: `g++ -o main main.cpp`.
   - Run your compiled program: `./main`.

## Conclusion

Successfully installed Visual Studio Code and  to work with MinGW on Windows system.
