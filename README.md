# Git 'er Done 🤠

## About
I wrote this during my 2023 summer internship with SkySpecs. It is a command line utility 
that allows you to easily customize your own git subcommand and comes with some handy features 
that streamline the agile process straight away.

* It combines multiple git commands into one where appropriate

* It allows you to link a commit to the ticket you're working on with an optional flag

* It copies relevant information to your clipboard when it comes time to write the merge request so you don't have to dig for it

* It clears your desktop of any screenshots or screen recordings once the merge request has been accepted and you're done with the branch

* It does it all while adding a fun Western theme to your workflow, which can be customized to anything you want!

## Installation
To install, simply run the following commands in the desired location on your machine.

    $ git clone https://github.com/ahmedxyz/git-erdone.git
    $ cd git-erdone && echo "export PATH=$PWD:\$PATH" >> ~/.zshrc && source ~/.zshrc

## Usage
To begin, provide a branch name and a new branch with that name will be checked out.

    $ git erdone <branch name starting with ticket id>

Next, provide a commit message whenever you want to commit. Use the optional flag to link the commit to the ticket.

    $ git erdone [-l/--link] "Commit message"

Pushing is easy. Use the optional flag to copy a link to the ticket in Shortcut to your clipboard (convenient for writing the MR).

    $ git erdone push [-mr/--mr]

And finally, when you're done working on the branch

    $ git erdone done

That's it!
