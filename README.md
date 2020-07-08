# kiss-glibc-repo
This is a repository containing an unofficial port of KISS Linux to the x86_64 architecture based on Glibc.

# Installation as chroot

The chroot script and tarball can be downloaded from the Releases page of this respository.

Unpack the tarball in a directory of your choice and then chroot in that directory. 

# Installation as main system

It has not been tested as a main system. My use is for a chroot, so I don't know
if it works as a main system. Be careful, like testing it on a virtual machine before
installing this version on a productive computer. 

# Notes 

## Repositories

To ease maintenance the build files from the KISS distribution are reused. With this version, `python` and `gawk`
are necessary (dependencies of glibc). Python is in the extra repository and `gawk` in community. So community is
enabled by default. 

## KISS paths

To avoid creating new builds of some packages, only packages with specific build instruction for glibc are available. 
The other are reused from the KISS distribution. So be careful in your KISS paths (`/etc/profile.d/kiss_path.sh`). 
