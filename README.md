# Welcome to GitHub!

You probably haven't encountered GitHub yet, but that's okay. In this guide, we'll explain how **Git** works and focus on important concepts like **Commit** or **Pull Request**.

## Navigation

* [Basic Concepts](#basic_concepts)
* [Creating a Repository](#creating_repository)
* [Setup / Committing from Visual Studio](#commit_vs)
* [Setup / Committing from GitHub Desktop](#github_desktop)
* [Setup / Committing from JetBrains Rider](#commit_rider)
* [Setup / Committing from Terminal](#commit_cmd)
* [Collaboration between Classmates](#collaboration)
* [GitHub Student Developer Pack](#student_pack)
* [Resources](#resources)

## Basic Concepts <a id=basic_concepts>

**Git** - Git is an open source tool that allows you to **track changes** in files. It's the fundamental technology that GitHub uses.

**Repository** (**Repo**) - A repository is the basic element of GitHub. You can say it's a **folder** where your project is located. This folder contains all the files of your project and stores the **history of all changes** for each file. You don't have to be the only one with access to the repository, as a repository can have multiple collaborators. A repository can be **public** or **private**.

**Commit** - A commit is a **grouping of changes** in a project. When you commit, Git creates a **unique ID** that allows you to keep records of these changes and also **who** and **when** made the change.

**Organization** - A GitHub Organization is like a profile that **multiple** users have access to. In this organization, you can create repositories.

**Fork** - A fork is a copy of another user's repository that gets saved among your repositories. Forks allow you to freely make changes to a project **without affecting the original repository**. However, you can open a **Pull Request** in the original repository.

**Pull Request** - Pull Requests are changes in a repository that a user has proposed and that you as the **owner** (or **collaborator**) of the original repository can **accept** or **reject**.

**Push** - Uploading local changes (not yet on GitHub) that are contained in **commits** to **GitHub**.

**Pull** - Downloading the **current version** of a repository from GitHub. If you've modified some files, a conflict (**Merge Conflict**) may occur, which needs to be resolved.

**Branch** - A branch is a **project branch** that you can add if you want to fix a bug or experiment with something, but don't want it to affect your project. Every repository has a **default branch**, but can contain others as well.

**Merge** - Merge is the **combining** of one branch into another by executing a **Pull Request**.

**Merge Conflict** - This is a state where multiple **newer** versions of a file exist in the code and it's unclear which version should be used.

**License** - A license is an important file that **allows** or **prohibits** you from using other users' code. A license may contain **conditions** and you can legally use code under this license only if you meet them.

**IDE** - *Integrated Development Environment* - is a **development environment** in which you'll work.

**readme.md** - This is a text file containing information about the repository. Since it's automatically displayed **under the repository**, it's usually the first file that a visitor to your repository will see. It's written in **Markdown**.

**.gitignore** - gitignore is a file that specifies which parts shouldn't be uploaded along with changes in a commit. It's used to **filter out unnecessary files**, for example those created by the IDE, or **files with sensitive data**.

*Note: These are just basic concepts. We recommend reading the glossary from GitHub's official documentation: https://docs.github.com/en/get-started/quickstart/github-glossary*

## Creating a Repository <a id=creating_repository>

1. In the upper right corner, click **+** and click **New Repository**.

![img1](https://github.com/SPSKNM-cvicenia/Github-Introduction/blob/main/uploads/newrepo1.png "New repo")

2. Name your repository, you can also add a description, **readme** file, **.gitignore**, **license** or change the repository to **private**. Then click **Create Repository**.

![img2](https://github.com/SPSKNM-cvicenia/Github-Introduction/blob/main/uploads/newrepo2.png "New repo")

## Setup / Committing from Visual Studio <a id=commit_vs>

### Repository Setup

After installing Visual Studio, you must synchronize your GitHub repository so you can create commits from it.

1. After opening Visual Studio, choose **Clone a repository**, which is located in the right part of the window.

![imgvs1](https://github.com/SPSKNM-cvicenia/Github-Introduction/blob/main/uploads/vs/1.png "vs")

2. Here choose **GitHub**.

![imgvs2](https://github.com/SPSKNM-cvicenia/Github-Introduction/blob/main/uploads/vs/2.png "vs")

3. A window will pop up where you can log in by clicking **Sign in...** in the upper right part.

![imgvs3](https://github.com/SPSKNM-cvicenia/Github-Introduction/blob/main/uploads/vs/3.png "vs")

![imgvs4](https://github.com/SPSKNM-cvicenia/Github-Introduction/blob/main/uploads/vs/4.png "vs")

4. After successful login, Visual Studio will make your repositories available.

![imgvs5](https://github.com/SPSKNM-cvicenia/Github-Introduction/blob/main/uploads/vs/5.png "vs")

After selecting one of the repositories, it will download and you can edit it or use it otherwise.

### Committing

After editing files, you must commit the changes.

1. After editing the project, Visual Studio will show how many changes were made. Click on the pencil in the lower right corner with a number (the number symbolizes how many files were changed), and the **GIT panel** will open.

![imgvs6](https://github.com/SPSKNM-cvicenia/Github-Introduction/blob/main/uploads/vs/6.png "vs")

2. Write a description of the commit and press **Commit All**.

![imgvs7](https://github.com/SPSKNM-cvicenia/Github-Introduction/blob/main/uploads/vs/7.png "vs")

![imgvs8](https://github.com/SPSKNM-cvicenia/Github-Introduction/blob/main/uploads/vs/8.png "vs")

3. Notice that Visual Studio says the commit was created locally - this means it's not yet in your repository on GitHub, but only on your computer. If you want to put it on GitHub, click **Push**, and Visual Studio will push it to GitHub.

![imgvs9](https://github.com/SPSKNM-cvicenia/Github-Introduction/blob/main/uploads/vs/9.png "vs")

![imgvs10](https://github.com/SPSKNM-cvicenia/Github-Introduction/blob/main/uploads/vs/10.png "vs")

### Downloading Changes from GitHub / Fetch

Changes that were made in the repository by someone else won't download automatically, you must first **fetch** them and then **pull** them.

1. In the Git panel, click **Fetch**.

![imgvs11](https://github.com/SPSKNM-cvicenia/Github-Introduction/blob/main/uploads/vs/11.png "vs")

2. Visual Studio will then show you how many commits need to be downloaded so you have the most current version of the repository:

![imgvs12](https://github.com/SPSKNM-cvicenia/Github-Introduction/blob/main/uploads/vs/12.png "vs")

3. Click on the **number of changes** and then on **Pull**.

![imgvs13](https://github.com/SPSKNM-cvicenia/Github-Introduction/blob/main/uploads/vs/13.png "vs")

## Setup / Committing from GitHub Desktop <a id=github_desktop>

Unlike other **IDEs**, GitHub Desktop is a stand-alone GIT client, which means it doesn't have IDE elements (Compiler, code editor, ...) but is intended only for committing and other GIT operations.

### Repository Setup
After installing GitHub Desktop, you must synchronize your GitHub repository so you can commit from it.

1. On the left, click **Clone a repository from the Internet**
2. Then choose **GitHub.com** and click **Sign In**. Then in the security warning window, click **Continue with browser**.

![img_gh1](https://github.com/SPSKNM-cvicenia/Github-Introduction/blob/main/uploads/ghd/1.png "ghd")

![img_gh2](https://github.com/SPSKNM-cvicenia/Github-Introduction/blob/main/uploads/ghd/2.png "ghd")

![img_gh3](https://github.com/SPSKNM-cvicenia/Github-Introduction/blob/main/uploads/ghd/3.png "ghd")

4. In the browser, log into GitHub (if you're not already) and click **Authorize desktop**.

![img_gh4](https://github.com/SPSKNM-cvicenia/Github-Introduction/blob/main/uploads/ghd/4.png "ghd")

6. Your repositories will be displayed on the right. Choose the correct one and click **Clone [repository name]**. Choose where you want to save it and click **Clone**.

![img_gh5](https://github.com/SPSKNM-cvicenia/Github-Introduction/blob/main/uploads/ghd/5.png "ghd")

![img_gh6](https://github.com/SPSKNM-cvicenia/Github-Introduction/blob/main/uploads/ghd/6.png "ghd")

![img_gh7](https://github.com/SPSKNM-cvicenia/Github-Introduction/blob/main/uploads/ghd/7.png "ghd")

8. Your repository has just been cloned and you can start working.

![img_gh8](https://github.com/SPSKNM-cvicenia/Github-Introduction/blob/main/uploads/ghd/8.png "ghd")

### Committing
After editing files, you need to make a **commit**. GitHub Desktop automatically tracks changes in files and displays them on the panel in the left part with each change.

1. In the lower left corner, write the commit name and optionally description, then click **Commit to master**.

![img_gh9](https://github.com/SPSKNM-cvicenia/Github-Introduction/blob/main/uploads/ghd/9.png "ghd")

2. Notice that your commit is not yet on GitHub, and GitHub Desktop says that one (or more) commits are available that haven't been **pushed** to GitHub yet - this means these commits are not yet in your repository on GitHub, but only on your computer. If you want to put them on GitHub, click **Push origin**, and GitHub Desktop will automatically push them to GitHub.

![img_gh10](https://github.com/SPSKNM-cvicenia/Github-Introduction/blob/main/uploads/ghd/10.png "ghd")

### Downloading Changes from GitHub / Fetch
Changes that were made in the repository by someone else won't download automatically, you must first **fetch** them and then **pull** them.

1. On the top panel, click **Fetch Origin**. This will check the state of the repository and whether a newer commit is available.

![img_gh11](https://github.com/SPSKNM-cvicenia/Github-Introduction/blob/main/uploads/ghd/11.png "ghd")

2. If a newer commit is available, you'll see the option to **pull** changes. Pull them by clicking **Pull origin**.

![img_gh12](https://github.com/SPSKNM-cvicenia/Github-Introduction/blob/main/uploads/ghd/12.png "ghd")

## Setup / Committing from JetBrains Rider <a id=commit_rider>

### Repository Setup

After installing JetBrains Rider, you must synchronize your GitHub repository so you can commit from it.

1. After opening JetBrains Rider, choose **Get from VCS**.

![imgrd1](https://github.com/SPSKNM-cvicenia/Github-Introduction/blob/main/uploads/rider/1.png "rider")

2. After opening a new window, check if Rider recognizes Git in the system. If you see **Git is not installed**, click **Download and install** and wait for the process to finish (it may take a few minutes).

![imgrd2](https://github.com/SPSKNM-cvicenia/Github-Introduction/blob/main/uploads/rider/2.png "rider")

3. On the left in the menu, click **GitHub** and then **Log in via GitHub...**, which will open a web browser. Click the **Authorize in GitHub** button, log in, and after successful login, you'll see that you've successfully logged into GitHub and can close the tab.

![imgrd3](https://github.com/SPSKNM-cvicenia/Github-Introduction/blob/main/uploads/rider/3.png "rider")

![imgrd4](https://github.com/SPSKNM-cvicenia/Github-Introduction/blob/main/uploads/rider/4.png "rider")

![imgrd5](https://github.com/SPSKNM-cvicenia/Github-Introduction/blob/main/uploads/rider/5.png "rider")

![imgrd6](https://github.com/SPSKNM-cvicenia/Github-Introduction/blob/main/uploads/rider/6.png "rider")

4. After successful login, Rider will offer your repositories for download:

![imgrd7](https://github.com/SPSKNM-cvicenia/Github-Introduction/blob/main/uploads/rider/7.png "rider")

5. Click the **Clone** button - The repository will automatically download and you can use it.

### Committing

After editing files, you need to make a **commit**.

1. In the upper right corner, you see **GIT** menu icons. For committing, click the green checkmark.

![imgrd7](https://github.com/SPSKNM-cvicenia/Github-Introduction/blob/main/uploads/rider/11.png "rider")

2. A menu will open on the left showing changed files. Write a commit description at the bottom and click **Commit and Push**.

![imgrd7](https://github.com/SPSKNM-cvicenia/Github-Introduction/blob/main/uploads/rider/12.png "rider")

3. This step is only necessary after the **first commit** from a new **IDE**: Git needs your information for the first run. Enter the information and then click **Set and commit**.

![imgrd7](https://github.com/SPSKNM-cvicenia/Github-Introduction/blob/main/uploads/rider/13.png "rider")

4. A window will appear summarizing what changes you're about to make. Click the **Push** button and Rider will upload the changes directly to GitHub.

![imgrd7](https://github.com/SPSKNM-cvicenia/Github-Introduction/blob/main/uploads/rider/14.png "rider")

### Downloading Changes from GitHub / Fetch

Changes that were made in the repository by someone else won't download automatically, you must first **fetch** them and then **pull** them.

1. In the GIT panel, click the blue arrow pointing down.

![imgrd7](https://github.com/SPSKNM-cvicenia/Github-Introduction/blob/main/uploads/rider/16.png "rider")

2. After clicking, choose **Merge incoming changes into current branch**.

![imgrd7](https://github.com/SPSKNM-cvicenia/Github-Introduction/blob/main/uploads/rider/17.png "rider")

## Setup / Committing from Terminal <a id=commit_cmd>

### Setup
1. Download **GIT** (installation guide is available on [their website](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git)).
2. Configure your **name** and **email**.
```
$ git config --global user.name "Your Github Login"
$ git config --global user.email "your_email@something.something"
```
3. **Initialize** a Git repository in the folder. This command creates a new so-called local repository. Local repositories store changes only on your computer.
```
$ git init
```

If you want to use GitHub, you must add it as a remote origin. Remote origin is a repository that will be synchronized with your local one. This means you'll be able to pull changes made on GitHub (as remote), and push changes made in the local repository. However, this process is automated, so you just need to execute commands from the Committing and Downloading changes from GitHub sections. If you want to add your repo as remote, execute the following command, just change the URL address:
```
$ git remote add origin "https://github.com/github_login/repository_name.git"
```

3. Set the **branch** you want to work in (usually `main` or `master`).
```
$ git branch -M main
```
### Committing
1. Select all **changes** you want to **upload**.
```
$ git add <changed_file>
```
or, if you want to upload **all files**:
```
$ git add .
```
2. **Commit** changes with an appropriate **description** of changes.
```
$ git commit -m "this is a commit description"
```
3. **Push** committed changes to GitHub.
```
$ git push
```
### Downloading Changes from GitHub / Fetch
1. If you want to **only get information** about the **current version** of the remote repository, execute:
```
$ git fetch
```
2. If you want to **download them afterwards**, use:
```
$ git pull
```

## Collaboration between Classmates <a id=collaboration>

You're in a team with a classmate and you need to work on a project together, but you don't want each of you to have your own repository, you want to work on one. In that case, you can add your classmate as a collaborator to your repository.

1. Go to **repository settings**.

![img3](https://github.com/SPSKNM-cvicenia/Github-Introduction/blob/main/uploads/privrep1.png "settings")

2. Click **Manage Access** (May require re-login).

![img4](https://github.com/SPSKNM-cvicenia/Github-Introduction/blob/main/uploads/privrep2.png "settings")

3. Click **Invite a collaborator**.

![img5](https://github.com/SPSKNM-cvicenia/Github-Introduction/blob/main/uploads/privrep4.png "settings")

4. Search for your classmate and add them.

![img6](https://github.com/SPSKNM-cvicenia/Github-Introduction/blob/main/uploads/privrep5.png "settings")

![img7](https://github.com/SPSKNM-cvicenia/Github-Introduction/blob/main/uploads/privrep6.png "settings")

![img8](https://github.com/SPSKNM-cvicenia/Github-Introduction/blob/main/uploads/privrep7.png "settings")

![img9](https://github.com/SPSKNM-cvicenia/Github-Introduction/blob/main/uploads/privrep8.png "settings")

5. Your classmate will then receive an invitation to their email address, which they will accept.

![img10](https://github.com/SPSKNM-cvicenia/Github-Introduction/blob/main/uploads/privrepo8.png "settings")

![img11](https://github.com/SPSKNM-cvicenia/Github-Introduction/blob/main/uploads/privrepo9.png "settings")

## GitHub Student Developer Pack <a id=student_pack>

GitHub provides a set of tools and benefits **for free** to students. Examples include **JetBrains IDE** or **GitHub Copilot**. Our school is registered with GitHub and therefore as a student you have the opportunity to use these benefits.

For the pack you need:

1. **GitHub** Account

2. Proof of school attendance from **EduPage** or **ISIC**

3. **School** email address (@spsknm.onmicrosoft.com)

Start by adding your school email address as **secondary** in settings:

![img12](https://github.com/SPSKNM-cvicenia/Github-Introduction/blob/main/uploads/email1.png "settings")

Then go to https://education.github.com , where you log in and request a **discount**. Choose your **school** email address and write how you plan to use the **GitHub Student Pack**:

![img13](https://github.com/SPSKNM-cvicenia/Github-Introduction/blob/main/uploads/imgGEdu.png "settings")

Then click **continue** and upload your scanned **ISIC** / screenshot from **EduPage**:

![img13](https://github.com/SPSKNM-cvicenia/Github-Introduction/blob/main/uploads/eduimg3.png "settings")

For **Proof type** put:

* if you sent **ISIC** - **Dated School ID**.

* if you sent a screenshot from **EduPage** - **Other (Example: Screenshot of school portal)**.

And submit the request. GitHub should respond within **30 days**.

*Note: You need to ask your programming teacher for the school email address (@spsknm.onmicrosoft.com)*

*Note: We recommend reading the official GitHub Education documentation: https://docs.github.com/en/education. We also recommend reading the GitHub Education FAQ if you don't have ISIC: https://github.blog/2019-07-30-how-to-get-the-github-student-developer-pack-without-a-student-id/*

*Note: GitHub often changes these requirements, so this section may be out-of-date. If it is, we welcome pull-requests with corrected procedures.*

## Resources <a id=resources>

GitHub Docs - https://github.com/github/docs/ under <a href="https://github.com/github/docs/blob/main/LICENSE">CC-BY 4.0</a> license
