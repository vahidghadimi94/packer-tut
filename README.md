# packer-tut
Packer is a tool for building identical machine images for multiple platforms from a single source configuration.
# how to install packer in linux machine

1. Download the required package from here. https://www.packer.io/downloads.html

2. Unzip the package and set the path variable in ~/.bashrc

     export PATH=$PATH:/path/to/packer

3. Refresh terminal

     source ~/.bashrc


4. Verify packer installation by executing the packer command.

     packer version


# Step-by-step instructions to build the AMI
Follow the steps below in order to build the AMI
# Step 1: Prep Packer template
my template is first-template.json
# supplies the values for all the dynamic variables 
my var file is vars.json
# Build AMI
packer build -var-file=vars.json first-template.json
