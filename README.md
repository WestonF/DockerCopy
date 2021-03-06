# Install and Run Docker on Windows 10+
Custom and very basic template by Joshua Willis to automate Docker functions on Windows using batch scripting.

## Step 1: Install Docker
Visit the following webpage to install Docker: https://www.docker.com/get-started
During installation, you may be asked to update your WSL Kernel to the most recent version. Make sure you do this as required and restart your computer when prompted.

## Step 2: Clone Template Repository
All the scripts necessary to run basic Docker commands are found on this repository and can be freely cloned for your own adaptation. There are several ways to do this, but I recommend you use the 'Use this Template' feature on github to create a copy of this template into your github profile for your own personal use.

## Step 3: Modify the Dockerfile
Modify the dockerfile for your own use. Included is a basic template generated by Manoj Joshi.

Make sure to include a FROM directive using an acceptable image to copy from such as CentOS, RHEL, or Ubuntu and the :latest suffix to get the latest version. Alternatively, you may use :\[version] to copy a specific version.

## Step 4: Run the "build" Command to Build your Image
Run the 'build.bat' script to automatically build a new image from the Dockerfile.

You can use the command `docker image ls` to ensure your Dockerfile was successfully built into an image.

## Step 5: Run the "spinup" Command to Spin Up a new Container from that Image
Run the 'spinup.bat' script to automatically create a new container using the newly built image.

## Step 6: Run the "attach" Command to Attach to your new Container
Run the 'attach.bat' script to automatically connect to the container. Be warned that if you create more than one container, this script will only connect to the oldest without any modifications.
