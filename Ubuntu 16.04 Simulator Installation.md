# 2017 FRCSim Installation (Ubuntu 16.04)

#### Step 1: Run this Script

```bash
# Warning: This line downloads roughly 200MB and uses about 1.5GB of disk space
sudo apt-get install gazebo7 libgazebo7-dev cmake libprotobuf-dev libprotoc-dev protobuf-compiler

# Download Files
wget http://first.wpi.edu/FRC/roborio/maven/release/edu/wpi/first/wpilib/simulation/simulation/2017.1.1/simulation-2017.1.1.zip
wget -O models.zip https://usfirst.collab.net/sf/frs/do/downloadFile/projects.wpilib/frs.simulation.frcsim_gazebo_models/frs1160?dl=1

# Unzips
unzip simulation-2017.1.1.zip -d ~/wpilib/simulation
unzip models.zip -d ~/wpilib/simulation

# Moves into place
mv ~/wpilib/simulation/frcsim-gazebo-models-4/* ~/wpilib/simulation/
rmdir ~/wpilib/simulation/frcsim-gazebo-models-4

# Build and Install gz_msgs
cd ~/wpilib/simulation/gz_msgs
mkdir build
cd build
cmake ..
make install

# Link files
sudo ln -s ~/wpilib/simulation/frcsim /usr/bin/frcsim
sudo ln -s ~/wpilib/simulation/sim_ds /usr/bin/sim_ds
```

#### Step 2: ????
#### Step 3: Profit
