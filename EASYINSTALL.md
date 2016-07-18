This file can be used to build NimgOS in a couple steps.

To use this file, you will not need to download a copy of this repository. 
You will just need a copy of the following script.

```bash
#!/bin/bash

echo "##################################################################################"
echo "# Thanks for trying out NimgOS, this script was developed to easily build NimgOS #"
echo "#  This script may request for root privilges to install git and other packages  #"
echo "##################################################################################"

sleep 2

echo ""

echo "################## NOTICE #####################"
echo "# This script may only work on a Debian/Ubntu #"
echo "#                 based system                #"
echo "###############################################"

echo ""

sleep 5

echo "################################"
echo "# Installing a few packages... #"
echo "################################"

sleep 5
sudo apt install git xtightvncviewer nasm qemu

echo ""

echo "##############################"
echo "# Cloning the git repository #"
echo "##############################"

echo ""

git clone https://github.com/Njifra/NimgOS.git
cd NimgOS
sleep 5

echo ""

echo "################################"
echo "# Making the 'build' directory #"
echo "################################"

mkdir build

echo ""

echo "#######################################"
echo "# Making the b4_linux file executable #"
echo "#######################################"

chmod +x b4_linux

echo ""

echo "########################################"
echo "# Done building NimgOS. To run the OS, #"
echo "#         run ./NimgOS/b4_linux        #"
echo "########################################"

echo ""
sleep 5
echo "This script was created by xerox123 (xerox123official)"
```

Place this file into a directory where you want NimgOS to be cloned and name it 'easy_install.sh'.

Then execute the following commands:

```bash
# Make the file executable.
chmod +x easy_install.sh
# Run the file.
./easy_install.sh
```