#Important Git Concepts

1.Configure SSH Key. ( For Authentication as password is no longer supported )
    *[**Refer this documantation from git**](https://docs.github.com/en/authentication/connecting-to-github-with-ssh/ generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent)
    *[**Refer video for more understanding**](https://www.google.com/search?sca_esv=601322691&sxsrf=ACQVn0-fTvPFQ0y37jH2YDTdSlrf0nL80w:1706161910201&q=how+to+configure+ssh+key+for+git&tbm=vid&source=lnms&sa=X&ved=2ahUKEwj3vti07PeDAxW_-zgGHUFtAi4Q0pQJegQIDBAB&biw=1850&bih=966&dpr=1#fpstate=ive&vld=cid:d317f611,vid:8X4u9sca3Io,st:0)

2.Learn what is a repository.
    *Repositories in GIT contain a collection of files of various different versions of a Project. These files are imported from the repository into the local server of the user for further updations and modifications in the content of the file. 
    [*refer this tutorial for better understang*](https://www.geeksforgeeks.org/what-is-a-git-repository/)

3.Learn what is the diff between Git & GitHub.
    *Git: Git is a distributed version control system for tracking changes in source code during software development. It is designed for coordinating work among programmers, but it can be used to track changes in any set of files. Its goals include speed, data integrity, and support for distributed, non-linear workflows. 

    *GitHub: GitHub is a web-based Git repository hosting service, which offers all of the distributed revision control and source code management (SCM) functionality of Git as well as adding its own features. 

4.Install Git on your system and learn how to check the version of that.
    * sudo apt install git
    * git --version
    
5.Learn how to initiate empty repo on your local machine.
    * git init <project directory>
    * git clone <repo url>

6.What are different steps involved in Git.
        Step 1: Install Git and Create a GitHub Account.
        Step 2: Create a Local Git Repository.
        Step 3: Create a New Repository on GitHub.
        Step 4: Add a File to the Repository.
        Step 5: Unstage Files on Git.
        Step 6: Create a Commit.
        Step 7: Undo Last Commit.
        Step 8: Create a New Branch.
    * [refer this documentation for better understang](https://opensource.com/article/18/1/step-step-guide-git)

7.What is commit messages? And what is called as proper commit message?
    *Commit messages are a way of communication between team members. Let’s say there’s a bug in the application which was not there before. To find out what caused the problem, reading the commit messages could be handy. The proper commit message can save a great deal of time finding the recent changes related to a bug.
    [refer for more details](https://reflectoring.io/meaningful-commit-messages/#:~:text=Commit%20messages%20are%20a%20way,changes%20related%20to%20a%20bug.)
    
8.Learn how to add remote origin.
    * git remote add origin https://github.com/OWNER/REPOSITORY.git
    * git remote -v
    * [refer for more in git documantation](https://docs.github.com/en/get-started/getting-started-with-git/managing-remote-repositories)
9.Learn how to check for existing remote origin added.
    * git remote -v

10.Learn how to add User Config details ( username & email )
    *git config --global user.name "*username*"
     git config --global user.email"*email*"
     
    *[refer](https://www.google.com/search?q=Learn+how+to+add+User+Config+details&oq=Learn+how+to+add+User+Config+details&gs_lcrp=EgZjaHJvbWUyBggAEEUYOTIKCAEQABiiBBiJBTIKCAIQABiABBiiBNIBCDEwMzZqMGo3qAIAsAIA&sourceid=chrome&ie=UTF-8#fpstate=ive&vld=cid:b750776e,vid:yDntCIs-IJM,st:0)

11.How to check existing user config details.
    *git config --list
12.What is a branch?
    *A branch is a version of the repository that diverges from the main working project.
    *[refer for more..](https://www.javatpoint.com/git-branch)

13.How to create a branch? And how to checkout to a branch?
    *git branch <branch_name>
    *git checkout <other_branch_name>
    *git switch <other_branc_name> #both do same work

14.What is merging?
    *Git marge will help to combine the changes from two or more branches into a single branch. Developers will work on different branches to improve code or to develop the code after completion we can merge them into a single version of the code.
    *[refer for more..](https://www.geeksforgeeks.org/git-merge/)

    
15.What are merge conflicts?
    *Merge conflicts happen when you merge branches that have competing commits, and Git needs your help to decide which changes to incorporate in the final merge.
    *[refer for more..](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/addressing-merge-conflicts/about-merge-conflicts)

    
16.What is stashing?
    *The Git stash command can be used to accomplish this if a developer is working on a project and wants to preserve the changes without committing them. This will allow him to switch branches and work on other projects without affecting the existing modifications. You can roll back modifications whenever necessary, and it stores the current state and rolls back developers to a prior state.
    *[refer for more..](https://www.geeksforgeeks.org/git-working-with-stash/)
    
    
17.What is git pull? What is git push? Diff between them.
    *git pull is one of many commands that claim the responsibility of 'syncing' remote content. The git remote command is used to specify what remote endpoints the syncing commands will operate on.
    *The git push command is used to upload content to a remote repository. The git fetch command can be confused with git pull .
    *[refer for how it works](https://www.google.com/search?sca_esv=601333276&sxsrf=ACQVn08G8YersEwXXVSthu4TzNucyRup9g:1706164760546&q=What+is+git+pull%3F+What+is+git+push%3F+Diff+between+them.&tbm=vid&source=lnms&sa=X&ved=2ahUKEwiu3OuD9_eDAxV_mVYBHeloCJwQ0pQJegQIChAB&biw=1850&bih=966&dpr=1#fpstate=ive&vld=cid:e0b3895b,vid:H63nJJhoiMw,st:0)
    
18.How to create a repo on GitHub?
    *[follow git documentation](https://docs.github.com/en/repositories/creating-and-managing-repositories/creating-a-new-repository)

19.How to check the status of your local Git repo?
    *git status

20.What is the use of git log
    *The git log command displays committed snapshots. It lets you list the project history, filter it, and search for specific changes.
    *[refer how it works](https://www.atlassian.com/git/tutorials/inspecting-a-repository#:~:text=to%20a%20repository.-,git%20log,and%20search%20for%20specific%20changes.)
