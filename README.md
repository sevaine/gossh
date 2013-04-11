gossh
=====

Simple, and easy SSH connection management utility written in Python

License
-------

gossh is open-source and licensed under the Apache License, Version 2.0

Installation
------------

The master branch of this repo is considered ready for use, new features will go into the 'develop' branch.

git clone git@github.com:sevaine/gossh.git

- PyYaml is required for gossh.  Install it using your OS' package management, or with pip

Installation is simple, once PyYAML is installed, simply copy bin/gossh to ~/bin/gossh and then start using it.

Using gossh
-----------

- Adding a host:    
   gossh -a samplehost -i /path/to/ssh/key -u sample_user -H samplehost.example.com
- Removing a host:  
   gossh -r samplehost
- Updating a host:   
   gossh -m samplehost -i /path/to/ssh/new_key
- Connecting:       
   gossh samplehost

The gossh connections config file
---------------------------------

Gossh stores information about connections in $HOME/.gossh/connections.yaml
At present gossh only supports 1 config file per user.  
