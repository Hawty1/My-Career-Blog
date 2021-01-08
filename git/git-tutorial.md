
## Lets get in touch with Git
>
>On my coding adventures I heard "Git" alot. As you can read my blog on GitHub right now, I even
>decided to try it out myself. In my coding course today it really payed off because I already 
>understood the branching system quiet.
>
>This pictures was the perfect explantation for the git system. 
>
> ![](https://guides.github.com/activities/hello-world/branching.png)
>Tutorials from [GitHub](GitHub.com) like the [hello-world](https://guides.github.com/activities/hello-world/)  one helped me alot. <br>
>We can find the most important git-keywords already here.
>1. Master
>2. Branch
>3. Commit 
>4. merge
>5. Pull request
>
##### Apply it to our Linux directory with the *_Git - Distributed Version Control System_*
Of course we doing this by Terminal commands. Since we are already on GitHub we already know the structure how Git looks like. But in our Terminal or in our simple Linux directory, we dont have thit fancy user interface. Even though it still works exactly the same.
<br>
<br>

# Creating a Repository
### *1. Initialize the directory you want use as your _repository_*
We can accomplish this with the command 
       
    git init

Now our current directory is initialized as our repository and will be able to work with I just as we can on our GitHub Website. 
### *2. Create a readme file and push it to our _master branch_* 
For creating a file I will simply use our touch command.

    touch readme.md

The file is now created, but not really pushed. We need to actually add it to the branch we are working on. Since we dont have created a new branch at the moment, we should be still in our master branch by default. So let's push (or add) our file to our current branch (master branch).

    git add readme.md

### *3. _Commit_ the change that we added a file.*


After adding our file we almost finished our first set up.
As we want to be as clear as possible what we changed its always good to write a message 
within every commit we are about to do. The _"flag"_ to accomplish that is _"-m"_.

    git commit -m "readme for my first repository created with terminal"

If you facing an error here, dont worry. Here's the solution:
Git dont knows who you are, so we need to tell it to recognize who the user is which is working 
for. It takes 2 things: name, email. Type those commands with your actual Name and Email adress inside of the quotation marks.

    git config --global user.name "FIRST_NAME LAST_NAME"
    git config --global user.email username@example.com

Now git knows who we are and let us commit our file. So try it again if you faced the error before.  
*_CONGRATS!_ We have just created our first local repository where we can work on with the git system applied.*

<br>
 
# Check Status

At any point during the work process we can always check the current status of the _branch_ we are in. As we just setted up the first repository, there should be only the main branch.  
Check your current working status with: 

    git status

## The output should look like some of those:  
1. Here we see untracked files. this will happen if we don't _add_ our changes to our current repository.   

<img src="img/notaddedstatus.png" style="width:55%;height:25vw;margin-left:3.5em">  

___NOTE: Even if changes are already in the folder, they still have to be added to be tracked by git.___  

2. Next one is the message if we have changes that where added, but not committed yet. 

<img src="img/notcommitedstatus.png" style="width:65%;height:25%;">

___NOTE: Every change we add, also have to be commited afterwards.___

3. As we can see now, because we _added_ any untracked files and _committed_ them to our _repository_, git status will tell us that everything is done.

<img src="img/clearnstatus.png" style="width:65%;height:25%">

___NOTE: every git status message ONLY checks the status for the _Branch_ you are currently working in.___
