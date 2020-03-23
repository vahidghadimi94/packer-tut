# packer-tut
Packer is a tool for building identical machine images for multiple platforms from a single source configuration.
# Step-by-step instructions
Follow the steps below in order to build the AMI
# Step 1: Prep Packer template
my template is first-template.json
# supplies the values for all the dynamic variables 
my var file is vars.json
# Build AMI
packer build -var-file=vars.json first-template.json
