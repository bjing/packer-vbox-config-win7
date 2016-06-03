#Custom Windows 7 Image using Packer

This is an attempt to create a VirtualBox Windows image with MS-SQL server preinstalled from an existing exported OVF file with extra configuration on top using Packer. 

# Requirements
* An existing exported VirtualBox Windows OS image, usually with .ova extension
* [Packer](https://www.packer.io/)

# Howto
## Install Packer
On OSX, use brew:
```
brew install packer
```
Alternativaly, you can download Packer binary from the [Packer website](https://www.packer.io/).

## Build the Box Image
In the root directory of the repo, do
```
packer build packer.json 
```

