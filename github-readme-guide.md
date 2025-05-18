### How to add a simple `README.md` file to your GitHub profile

  
#### Audience

This guide is aimed at people with general PC proficiency, basic Git and GitHub knowledge.

  

#### Prerequisites

* PC/Laptop with Windows

* Internet Connection

* GitHub account

* GitHub repository named after your username

* Git application

  

#### Intro

If the repository name matches your GitHub username, GitHub will display its `README.md` on your profile page. 
This guide explains how to connect to that repository using Git and how to add a `README.md` file with some basic Markdown to it.  

**Note:** This guide doesn't cover the Git installation process, please refer to [official Git install manual](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git).   
For a GitHub repository creation, please see [their official manual](https://docs.github.com/en/repositories/creating-and-managing-repositories/creating-a-new-repository).

  

#### Verifying Git installation and setup

1. Open command line and verify that you have Git installed:

```console

git --version

```

Output example:

```console

git version 2.49.0.windows.1

```

2. As per GitHub's Git Setup manual, you should setup your username and commit email address in Git.

To verify it has been set up, run the following commands:

```console

git config --global user.name

```

```console

git config --global user.email

```

The output should display your name and email. If not, refer to the [documentation](https://docs.github.com/en/get-started/git-basics/set-up-git).

  

#### Cloning a repository

3. Cloning the repository to your local machine:

```console

git clone <REMOTE_URL>

```

`REMOTE_URL` is the link to your repository, for example, `https://github.com/oleh2601/oleh2601`.

After cloning, Git will create a new directory named after your repository.

4. Open the cloned repository:

```console

cd repository-name

```

#### Creating a `README.md` file

5. Create a new `README.md` file:

```console

notepad README.md

```

6. Next, add your own text or copy this sample Markdown text inside Notepad:

Sample:

```Markdown
### **_Success!_**

I now know how to create simple Markdown files...

> _“I am still learning.”_ —Michelangelo

```

Save the file and close Notepad.

#### Adding a file to a repository

To add the new file to your repository, you need to:
	1. Stage the file(tell Git that we want to include the file in the next update)
	2. Commit (confirm the created/changed file and add a message about the changes)
	3. Push to GitHub (send the updated files to our repository)

7. Stage the file:

```console

git add README.md

```

8. Commit the change:

```console

git commit -m "Adding README.md"

```

`-m` adds a commit message

9. Push to GitHub:

```console

git push origin main

```

You will be prompted to complete authorization.

10. Now if you open your profile in the browser, you will see the newly created README.md file at the very top.

  

#### Summary

  

In this guide, you learned how to:

1. Verify your Git setup
    
2. Clone a GitHub repository
    
3. Create and edit a `README.md` file
    
4. Stage, commit, and push changes
    
5. Display your README on your GitHub profile


If you are interested in learning more about Markdown:
*  checkout its [Wikipedia page](https://en.wikipedia.org/wiki/Markdown)
* learn useful Markdown basics at [Markdown Tutorial website](https://www.markdowntutorial.com/).