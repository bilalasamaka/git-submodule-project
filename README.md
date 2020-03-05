# submodule-example-project

# Create Empty New Repository

    The git submodule add is used to add a new submodule to an existing repository. 
    The following is an example that creates an empty repo and explores git submodules.

    $ mkdir git-submodule-demo
    $cd git-submodule-demo
    $git init 

# Add Submodule Repository 

    $ git submodule add https://bitbucket.org/jaredw/awesomelibrary

    This command creates a new file ".gitmodule". 
    This file has own submodule path with submodule repository-url

        [submodule "awesomelibrary"]
        path = awesomelibrary
        url = https://bitbucket.org/jaredw/awesomelibrary
    
    $ git add --all
    $ git commit -m "added submodule."

# Checkout Submodule Changes 

    This command chechout selected branch update own submodule on main repository 

    $ git submodule update 
    