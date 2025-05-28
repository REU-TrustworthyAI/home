[<img width=900 src="../img/logo_rit.png?raw=yes">](../README.md)   
[Home](../README.md) |
[Schedule](../schedule.md) |

## Github Basics

### 0. Install [Git](https://git-scm.com/downloads) and create your [Github](https://github.com/) account.
 - Skip this step if you already have one.

### 0.5 Accept the invite to be added to this organization [REU-TrustworthyAI](https://github.com/REU-TrustworthyAI).
 - Add your GitHub username to [Google sheet](https://docs.google.com/spreadsheets/d/1w6aNToF7cyjsaXNpmJNCxZmzXrB5BWu0F6thpt_bnKk/edit?usp=sharing).

### 1. Create a new PRIVATE repository under this organization [REU-TrustworthyAI](https://github.com/REU-TrustworthyAI).
 - (1) Click on the **new** button:
 
 - (2) Initiate the new private repo:
 

### 2. Clone the created repo to your local machine.
 ```
 git clone THE-REPO-URL
 ```

### 3. Save username and token in git.
 - Create your personal access token on [this page](https://github.com/settings/tokens)
 - Copy the generated token.
 - In terminal:
 ```
 git config --global credential.helper manager
 ```
 - When running this command, the first time you pull or push from the remote repository, you'll get asked about the username and your token (NOT Password!). Afterwards, for consequent communications with the remote repository you don't have to provide the username and password.

### 4. Working with a github repo.
 - (1) Go to the local directory of the repo.
 - (2) Pull from Github so that the content on your local machine is updated with the remote server of Github:
 ```
 Your-Repo> git pull
 ```
 - (3) Work on your local machine (add/remove/edit files under the local directory of the repo).
 - (4) Commit to the remote server of Github (upload local changes).
 ```
 Your-Repo> git add .
 Your-Repo> git commit -m "YOUR COMMIT MESSAGE"
 Your-Repo> git push
 ```
 
 ### 5. Add your information to [Google sheet](https://docs.google.com/spreadsheets/d/1w6aNToF7cyjsaXNpmJNCxZmzXrB5BWu0F6thpt_bnKk/edit?usp=sharing)
 - Add your github repo url (along with your RIT identifier and Github ID) to the Google sheet.

## Initialize your repo

- Clone this repo **home** to your local machine
- Copy everything under the _lab/_ directory from this repo to your private repo on your local machine **(Don't forget the .gitignore)**
- Push the changes of your private repo to GitHub server.

