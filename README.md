# tensorflow-installation-guide

Supposing u have installed the GPU drivers

Download cuda toolkit 
* once the download is complete, open a terminal in the directory the base installer is and run the follow commands
* sudo dpkg -i cuda-repo-ubuntu1704-9-0-local_9.0.176-1_amd64.deb
* sudo apt-key add /var/cuda-repo-9-0-local/7fa2af80.pub (open the file with correct version) 
* sudo apt-get update
* sudo apt-get install cuda

Install CUDNN

* download the cuDNN v7.0.5 Library for Linux (tar file)(whatever the current version is )
* open a terminal in the directory the tar file is located
* unzip the tar file using the command
* tar -xzvf cudnn-9.0-linux-x64-v7.tgz
* run the following commands to move the appropriate files to the CUDA folder
* sudo cp cuda/include/cudnn.h /usr/local/cuda/include
* sudo cp cuda/lib64/libcudnn* /usr/local/cuda/lib64
* sudo chmod a+r /usr/local/cuda/include/cudnn.h /usr/local/cuda/lib64/libcudnn*
