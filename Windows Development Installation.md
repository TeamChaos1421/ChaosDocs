# Development Environment Installation (Windows)

#### Step 1: Download and Install JDK
- Go to http://www.oracle.com/technetwork/java/javase/downloads/index.html
- Select the download for **Java Platform (JDK)**
- Accept the license agreement
- Download the JDK for **Windows x64**
- Once it has downloaded, run it to install.

#### Step 2: Install the FRC Toolchain
- Go to http://first.wpi.edu/FRC/roborio/toolchains/
- Download and run the **2017 Windows Installer**

#### Step 3: Download Eclipse
1. Go to http://www.eclipse.org/downloads/eclipse-packages/
2. Scroll down to **Eclipse IDE for C/C++ Developers**
3. Select **64-bit** and then **Download**
4. Once the download is finished, open your **Downloads Folder**
5. Right click the Eclipse zip file and extract it.

#### Step 4: Run Eclipse
1. Go into the extracted folder and run **eclipse**
2. Click **OK** to select the default workspace
3. Exit out of the **Welcome** tab

#### Step 5: Add FRC Plugin Repository to Eclipse
1. Select "Help"
2. Click "Install new software"
3. From here you need to add a software update site, the location where the plugins will be downloaded. Push the "Add..." button then fill in the "Add Repository" dialog with:
4. Name: FRC Plugins
5. Location: http://first.wpi.edu/FRC/roborio/release/eclipse/
6. Press **OK**

#### Step 6: Install FRC Eclipse Plugin
1. Click the arrows if necessary to expand the WPILib Robot Development menu.
2. Select **Robot C++ Development**
3. Click Next, Next on the next page, then click the radio button to accept the license agreement and click Finish
4. If you receive a Security Warning prompt, click OK to continue.
5. When prompted, restart Eclipse. After Eclipse restarts and you select your Workspace (if prompted) you will see a dialog that says Installing Tools. This details the installation progress of the plugins, wait for the install to complete before proceeding. This dialog should only appear when the plugins are first installed or updated.

#### Step 7: Configure WPILib Plugin
1. In **Eclipse**, select **Window > Preferences > WPILib Preferences** and set the **Team Number** to **1421**
2. Press **OK**

#### Step 8: Install CTRE Toolsuite
1. Go to http://www.ctr-electronics.com/hro.html
2. Click on **Tech Resources**
3. Download **CTRE Toolsuite Installer**
4. Go to your **Downloads Folder** and extract the zip file
5. Open the extracted zip file and run the installer.
6. If Windows gets all high and mighty, select **More Info** and then **Run Anyway**

#### Additional Help
- https://wpilib.screenstepslive.com/s/4485/m/13810