Vagrant Box Factory
===================

The project to create the box manually.

The commands to run in the guest OS:

    # Guest OS
    $ sudo apt-get update -y >>/tmp/provision-script.log 2>&1
    $ sudo apt-get install nodejs -y >>/tmp/provision-script.log 2>&1
    $ sudo apt-get install lynx-cur -y >>/tmp/provision-script.log 2>&1
    $ sudo apt-get install ruby1.9.1-dev -y >>/tmp/provision-script.log 2>&1
    $ sudo gem install jekyll >>/tmp/provision-script.log 2>&1

The commands to produce the box:

    # Host OS
    $ vagrant package --output first-box-jekyll.box

