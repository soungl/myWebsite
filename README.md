I struggled to build my first website and to connect it to github (for version control and sharing code) and netlify (for site deployment). I had a working local repository but couldn't push it to the remote repository. So I copied the local respository under a new name, "myWebsite", and tried to connect it to a new remote respository. The following is how I did this. This will serve as a reminder if I have to do it again.

1. I already had an existing local repository in my laptop, called myWebsite.
2. I opened a new remote repository at GitHub. I needed to open one without README file to avoid an error when pusing the local repository.
3. I ran in the command line, git remote set-url origin https://github.com/soungl/myWebsite.git. This was to reset remote origin because I already had one (it was a messy process: I repeated creating and deleting). This command reset the remote origin. If I had done fresh, the usual command, git remote add origin https://github.com/soungl/myWebsite.git, would have worked.
4. I verified remote origin with command, git remote -v.
5. I pushed the local repository with command, git push origin master.