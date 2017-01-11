# 2017 Development Environment Installation (Ubuntu)

#### Step 1: Install JDK and FRC Toolchain
1. Open a terminal using **Ctrl-Alt-t** and enter these commands:
```bash
sudo add-apt-repository -y ppa:wpilib/toolchain
sudo apt update
sudo apt -y install openjdk-8-jdk frc-toolchain
```

#### Step 3: Download Eclipse
1. Go to http://www.eclipse.org/downloads/eclipse-packages/
2. Scroll down to **Eclipse IDE for C/C++ Developers**
3. Select **64-bit** and then **Download**
4. Once the download is finished, open your **Downloads Folder**
5. Right click the Eclipse zip file and extract/unzip it.

#### Step 4: Run Eclipse
1. Go into the extracted folder and run **eclipse**
2. Click **OK** to select the default workspace
3. Exit out of the **Welcome** tab

#### Step 5: Add FRC Plugin Repository to Eclipse
1. Select "Help"
2. Click "Install new software"
3. Push the "Add..." button then fill in the following information:
4. Name: FRC Plugins
5. Location: http://first.wpi.edu/FRC/roborio/release/eclipse/
6. Press **OK**

#### Step 6: Install FRC Eclipse Plugin
1. Click the arrows if necessary to expand the WPILib Robot Development menu.
2. Select **Robot C++ Development**
3. Click Next, then click Next again, then Accept the License Agreement, then click Finish
4. If you receive a Security Warning prompt, click OK to continue.
5. When prompted, restart Eclipse.

#### Step 7: Configure WPILib Plugin
1. In **Eclipse**, select **Window > Preferences > WPILib Preferences** and set the **Team Number** to **1421**
2. Press **OK**

#### Step 8: Install CTRE Toolsuite
1. Go to http://www.ctr-electronics.com/hro.html
2. Click on **Tech Resources**
3. Download **CTRE Toolsuite (No Installer) package**
4. Go to your **Downloads Folder** and open the zip file
5. In the file browser, open your home folder, then open the folder **wpilib/user/cpp**
5. Back in the zip file viewer, open the **cpp** folder and drag the contents (**include** and **lib**) over to the file browser.

#### Additional Help
- https://wpilib.screenstepslive.com/s/4485/m/13810
