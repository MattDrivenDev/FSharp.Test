# FSharp.Test

.NET 4 F# Console App, to test against platforms.

## Runs on Ubuntu 12.04 LTS, Just Fine:

Make sure that you have `VirtualBox` and `Vagrant` installed, then you can do the following (I'm using `Cygwin`)

```
# Just use the 'getting started' Ubuntu box from Vagrant Docs
vagrant init precise32 http://files.vagrantup.com/precise32.box
vagrant up

# SSH into the box
vagrant ssh
# ---- Now in the virtual Ubuntu machine

# Install Git
sudo apt-get install git-core

# Grab this app from Github and put it in a 'test' folder
git clone https://github.com/saxonmatt/FSharp.Test.git test

# Install the Mono runtime
sudo apt-get install mono-runtime

# Run the compiled FSharp app
mono test/FSharp.Test helloworld
```
