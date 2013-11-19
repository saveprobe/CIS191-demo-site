CIS 191 Project 3
-----------------

This is a demo site that is a simplified version of the CIS 191 website. It is
used as a testbed/training ground for Git usage and merge conflict resolution.

1. What does our *git hook* do?
    
What an excellent question. When we push from deploy to cloud, the push completes and then triggers the post-receive hook we have set up in the repository server. Our shell script copies all the files we push into the public directory of our site. The script also restarts the server. 

2. What does the python server do?
    
Our python server publishes from it's current directory, which in our case is www.

3. What is a *bare repository*?
    
A *bare repository* is a repository contains the files and directories traditionally contained inside .git. It does not contain a directory named .git, as it only contains its contents. It also does not contain a "working tree."
