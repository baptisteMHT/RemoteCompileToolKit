# RemoteCompileToolKit

This repository is a step-by-step guide on how to setup a cross-compilation pipeline.
**There is no guarantee it will work.**

## Tools

- git
- gcc
- rsync

## Steps


### Build from source

### Copy folder from remote to local
Now that the remote machine is done building, run the code below to copy the build files to your local machine.

'''
rsync --rsh='ssh -p<PORT>' -avz <USER>@<REMOTEIP>:compile/<FOLDER> ./compile/
'''

### Complete the install
