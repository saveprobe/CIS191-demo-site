CIS 191 Project 3
-----------------

This is a demo site that is a simplified version of the CIS 191 website. It is
used as a testbed/training ground for Git usage and merge conflict resolution.

1. What does our **git hook** do?
    
	When we push from our *deploy* branch to the cloud remote, as soon as the push completes, our *post-receive* hook is triggered that we have set up in the remote *deploy* repository. Our shell script copies all the files that we pushed into the bare repository into the directory *www,* which we designated as the public directory for our site. The shell script also restarts the server.

2. What does the python server do?
    
	Our python server publishes the files from its own directory, which in our case is *www*.

3. What is a **bare repository**?
    
	A **bare repository** is a repository that contains only the files and directories traditionally contained inside the *.git* directory. It does not contain a "working tree," so in that sense it is *bare*.
