## A modified lynx browser

This repository has a modified lynx browser.
You would need it only for web indexing, because lynx is used in the project Trokam to extract the plain text and title from an HTML page.
The modification makes lynx to save the title of the page in a file under the /tmp directory.
You find the original lynx in its [website](https://lynx.invisible-island.net/current/index.html).

## Build and Install

Build the modified lynx executing

    $ ./configure
    $ make

Do not install it using the make file. Execute this commands,

    $ sudo cp ./lynx /usr/local/bin/lynx_mod
    $ sudo cp ./lynx.cfg /usr/local/etc/lynx_mod.cfg
    
You could copy lynx_mod to any other location as long as the system find it for execution.
Trokam expects that it has the name lynx_mod. And the configuration file name must be lynx_mod.cfg in /usr/local/etc/.
Additionally, following this procedure you wont have any conflict with lynx installed by the package manager of you operating system.
    
