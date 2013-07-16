This is a repo of the intermediate files from running User massive quine relay at:

https://github.com/mame/quine-relay

I also 

## Additional execution information

I ran this on Linux Mint 12.  Here are the steps beyond those shown in the link above that I had to follow to get this working.

### Ruby ###

I was fortunate enough to already have 1.9.3 installed and set to run from the `ruby` command.  Good luck.

### Go language ###

You will also need to have the "go" command set up after installing golang (`apt-get install golang` is not enough).  Follow the instructions here:

http://golang.org/doc/install#environment

### Intercal ###

This one's tricky.  On Linux Mint, `apt-get install` didn't work for me.  Per the instructions here:

http://catb.org/esr/intercal/ick.htm#toc_Installation

I ended up downloading it from here (which I found from searching the newsgroup ... oy):

http://c.intercal.org.uk/download/#n5

Then go to the directory you downloaded it to and run these commands:

    tar xvf intercal-0.29.pax.gz  # or whatever the version is
    cd intercal-0.29
    mkdir build
    cd build
    ../configure
    make
    sudo make install

That should leave you with `ick` on your path and ready to use for that part of it.
