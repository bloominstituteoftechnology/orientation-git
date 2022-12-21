# Git Configuration Walkthrough

This github repository will walk you through setting up your Git and GitHub accounts. The intention of this project is to ensure your computer's environment is set up correctly and to give a preview of the Git work flow.  A deeper-dive into Git with additional functionality and explanations of each command will be part of your continued learning at BloomTech.

---

## Checklist

- [x] View this README  
- [x] Create a GitHub Account  
- [x] Open your Command Line Interface  
- [x] Setting up your Username and Email  
- [x] Setting up your Authentication  
- [x] Forking a Repository  
- [x] Cloning a Repository  
- [x] Making Changes to the Repository  
- [x] Commiting Changes Locally  
- [x] Moving Changes to GitHub   
- [x] Standard Work Flow

---

## View this README
First step complete! Welcome and good luck over the next steps!  
If you run into issues please visit the Hub's discussion forums or submit a ticket for assistance.

---

## Create a GitHub Account
*One time only.*

If you have not already created a GitHub account, follow this [GitHub](https://github.com/) link.
> Click Sign Up and follow the instructions.
> During setup you will need to verify your email, which is likely the final step.

---

## Open your Command Line Interface
*Become familiar with this step as you will use it often in your career.*

MacOS
> Open the Terminal: `Command Key + Spacebar` then type `terminal` in the search.

Windows
> Install [GitBash](https://git-scm.com/downloads) for Windows if you have not already done so.  
> Open GitBash: `Windows Key` then type `git bash` in the search.

---

## Setting up your Username and Email
*This step will need to be completed once per different computer you will use.*

1. On your Command Line Interface, type:  
    ```
    git config --global user.name "Put your Name in Here"
    ```
    ```
    git config --global user.email your@email.here
    ```

2. Check to see if that worked! Type:  
    ```
    git config --list
    ```
    
    You should see two lines in this list matching your values! Other lines are likely in the list as well.
    ```
    user.name=Radhika Zaur
    user.email=radhika.zaur@bloomtech.com
    ```

---

## Setting up Authentication
*This step will need to be completed per different computer and may need to be re-completed after a set amount of time.*
1. On GitHub: Click your profile icon on the top right.
2. Choose `Settings`.
3. Scroll down on the left menu and choose `<> Developer Settings`.
4. On the left menu choose `Personal access tokens`.
5. Choose `Generate new token`.
6. You will be prompted for your GitHub password here, type it in.
7. In the `Note` section, type a note for this personal access token. Something like: `BloomTech`.
8. In the `Expiration` section, choose the amount of time you wish this personl access token to remain valid.
9. Select the first check box next to `repo`. This should select the entire group.
10. Scroll to the bottom and click `Generate token`.
11. Leave this page open. You will need this token during the `Pushing Changes to GitHub` step.

---

## Forking the Repository
*This step will need to be completed once per repository you wish to have your own copy of on GitHub*
1. On the GitHub page this README is located, near the top right select `Fork`.
2. Under `Owner`, select your account.
3. Under `Repository name`, you may adjust the name of the repository if you like.
4. On the bottom of the page select `Create fork`.
5. You should be redirected to a new repository associated with your user account on GitHub.  
  
**Note:** Backend Developers - Forking will automatically occur with your subsequent repositories. You will likely fork repos for personal or later career uses though.

---

## Cloning the Repository
*This step will need to be once per repository you wish to place on your local computer.*

1. Look for the green `Code` button on GitHub and select it.
2. Select `HTTPS` if it is not currently selected.
3. Select the `copy` icon next to the displayed `https://github.com/...` link.
4. On your Command Line Interface, begin by moving to the directory you will store this repository.  
    Example: `cd ~/Bloom-Repos/`  
    If you need to build a new directory, follow these steps:  
    ``` 
    cd ~
    mkdir Bloom-Repos
    cd Bloom-Repos
    ```
5. Type: `git clone` then right click and paste the text you copied.  
    > Example: `git clone https://github.com/yourusername/orientation-git.git`
6. Type `ls` to view the newly cloned repository on your local computer.

---

## Making Changes to the Repository
*This step will typically involve you working on your project with integrated development environments.*
1. Move into the repository you cloned in your CLI by typing: `cd bd-orientation`. Your directory name may be slightly different.
2. Type `ls`. You should see a file called README.md. 
3. Your next goal is to open that file and edit it. Instructions below will use a basic text editor, but you may open the file any way you wish to modify the text inside.  
    > MacOS: type `open -e README.md`  
    > Windows: type `notepad README.md`
4. Place an `x` in each step you completed of the Checklist. This is simulating you modifying files while working on a project.  
    You should not place an `x` in the Committing Changes Locally or Moving Changes to GitHub yet.
4. Save your changes/
    > MacOS: press `Command S`  
    > Windows: press `CTRL S`
6. Close your editor and return to your command line interface. You should still be in the same directory as before.

---

## Commiting Changes Locally
*This step will typically be done one or more times on a project. Larger projects may require you to complete this step many times.*
1. On your Command Line, type: 
    ```
    git add .
    ```  
    Attention: the `.` above is intentional. The `.` identifies to Git to add all changed files.
2. Type:
    ```
    git commit -m "Checked off my finished tasks"
    ```
    Attention: Be careful with the `"`quotes`"` in the message above. Make sure to start and end the quotes.

---

## Pushing Changes to GitHub
*This step will typically be done one or more times on a project. If connected to Codegrade, this will cause your project to be scored again.*
1. Type:
    ```
    git push
    ```
2. If you are prompted for a `username`, type in your GitHub username.
3. If you are prompted for a `password`, copy and paste the personal access token you generated earlier.
4. Return to your GitHub repository page. Refresh if needed.
5. Check that the README.md file has been recently updated.
6. Scroll down to see the Xs you finished.

---

## Standard Work Flow ##
1. On your local computer, edit the README.md file again to add `x`s to your now finished tasks.  
   > Technically you have not finished the Standard Work Flow task, leave it without an `x`.
2. Practice adding, committing, and pushing. Check if your updates appear on GitHub.  
   > Adjust the message accordingly, ie: `Checked off additional finished tasks`
3. Repeat this process one final time for your final `x`. You want to become familiar with the process.

---

## Congratulations! ##
Git will be a tool you likely use daily throughout your career. 

This was a minimal dive into Git to make certain your computer's environment is set correctly. A deeper-dive into Git with additional functionality and explanations will be part of your continued learning at BloomTech.


