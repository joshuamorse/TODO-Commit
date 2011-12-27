TODO-Commit
===========

A PHP-CLI script to append removed lines from a TODO file to a commit message.
This is a revision of the gcmftd script written by [richtaur](http://github.com/richtaur).


Install
-------

Add todoc to your ``$PATH`` in your ``.bash_profile``:

    # todoc path
    export PATH=~/bin/todoc-script:$PATH


Add permissions:

    chmod 777 ~/bin/todoc-script/todoc


Usage
-----

By default, ``todoc`` will look for a ``TODO.markdown`` file in your repository, which will look something like this:

    something to do
    i need to do this
    
As you work, simply remove the items you complete, then run ``todoc`` from the command line. ``todoc`` will automatically
stage changed files, then commit them via removed todo-list items.