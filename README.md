# aspace-vagrant

After cloning the repository to your machine, you will need to [download a JDK.tar.gz](http://www.oracle.com/technetwork/java/javase/downloads/jdk8-downloads-2133151.html) and place it in the /apps/dist directory.

Additionally, you will want to take a look at [aspace.sh](https://github.com/brialparker/aspace-vagrant/blob/develop/scripts/aspace.sh#L6) and change the download link to whichever version/release candidate you want

```
wget https://github.com/archivesspace/archivesspace/releases/download/v1.5.1/archivesspace-v1.5.1.zip
```
Once those files are in place/edited, from the vagrant directory run

```
vagrant up
```

A lot of stuff will go by on the screen. It's mesmerizing. Once the vagrant is created and running:

```
vagrant ssh
```

Now it's time to fire up ArchivesSpace! navigate to /vagrant/apps/aspace/archivesspace*, then...

```
./archivesspace.sh
```

<i>Cue confetti</i>

*This path can be changed in [aspace.sh](https://github.com/brialparker/aspace-vagrant/blob/develop/scripts/aspace.sh#L8), this is just a local practice when setting up vagrants.

**Note: I have edited the [vagrantfile](https://github.com/brialparker/aspace-vagrant/blob/develop/Vagrantfile) to forward ports to 9XXX but this can be changed back to 8XXX.
