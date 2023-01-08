---
layout: home
title: "Setup Staff Pages" 
parent: References
nav_order: 3
---

# {{page.title}}

We have found it helpful to set up webpages with staff bios with
a picture and brief bio of each staff member.  

Purpose:

* to help the course staff (instructor, TAs, LAs) get to know each other.
* to help students feel comfortable attending labs and office.

See these example sites for the example bios and the info that you can include: 

| As Web Page | As GitHub Markdown Source |
|-------------|---------------------------|
| <https://ucsb-teaching-cs.github.io/s21/staff> | https://github.com/ucsb-teaching-cs/s21/tree/main/_staffers |
| <https:///ucsb-csw8.github.io/s22/staff> | <https://github.com/ucsb-csw8/s22/tree/main/_staffers> |
| <https://ucsb-csw8.github.io/w23c/staff/> | <https://github.com/ucsb-csw8/w23c/tree/main/_staffers> |
| <https://ucsb-csw8.github.io/w23k/staff/> | <https://github.com/ucsb-csw8/s22/tree/main/_staffers> |


You can use these as an inspiration to write your bio and select a picture that you'd like to share with students.

# Technical Steps

1. You will need a GitHub account; you can sign up for one at <https://github.com> on the free plan.  (You may also like to get the GitHub Student Developer Pack at <https://education.github.com/pack> but you won't need that to create your bio.)

https://ucsb-teaching-cs.github.io/s21/hw/adding_bio/

In the instructions, a PROJECT_REPOrefers to our GitHub repository (repo) that hosts our course website: https://github.com/ucsb-csw8/s22

For the naming convention, you can just use FirstName-LastInitial.png. (or whatever is your image extension; please don't use .tiff or .bmp)
==> I also included a templated bio file in the _staffers folder (it's called _example.md): feel free to copy its contents and create a new .md file with your NetID in which you can paste/update the info in the example.

If something is unclear in the instructions, please don't hesitate to reply to this email, directly to me (ykk), and ask for clarification! It helps make sure that those without any git/GitHub experience can follow the steps and get experience. :-)

## Step 1: Log into your GitHub account.

<details>
<summary>
If you need basic background on git/GitHub click the ▶ character at left
</summary>
## Version Control

First, a bit of background.

git and GitHub are two of the currently popular tools to keep track of the changes in text-based files.

### What's the difference between git and GitHub?
A lot of times you'll hear people use these terms interchangeably but that's not entirely correct.

**git** runs locally on your computer and keeps track of the changes that you make to the files on your machine.
You won't be able to share these changes with your teammates using git alone, and that's where GitHub comes in.

**GitHub** is a web service, a "cloud" platform that hosts your projects in repositories and allows you to share your repos with the world.
There are alternative solutions to GitHub, such as GitLab and BitBucket, but they are all designed to let you `push` your local changes to the cloud to enable backup, sharing, and collaboration.

### Basic git/GitHub references and tutorials

Here's a **GitHub Basics Tutorial - How to Use GitHub** <https://youtube.com/watch?v=x0EYpi38Yp4> to get you started.

You might also find it useful to look over the [Git Tutorial: Get Started with Version Control](https://www.taniarascia.com/getting-started-with-git) 
and [Command Line Tutorial: Usage in Linux and macOS](https://www.taniarascia.com/how-to-use-the-command-line-for-apple-macos-and-linux/) by Tania Rascia.

These visual guides might also be helpful in exposing what's going on behind each `git` command you run:
* A Grip On Git (A Simple, Visual Git Tutorial) <https://agripongit.vincenttunru.com>
* Version Control with Git <https://zuckermanbrain.github.io/git-novice>
* A Visual Git Reference <https://marklodato.github.io/visual-git-guide/index-en.html>


</details>


## Step 2: Locate the repo for your course's website


The repo for your course's website will be under the `ucsb-csw8` github organization, and probably has a name that follows the naming conventions shown here:

| Quarter                         | Repo Name  | Link                               |
|---------------------------------|------------|------------------------------------|
| Winter 2022                     | w22        | <https://github.com/ucsb-csw8/w22> |
| Spring 2022                     | s22        | <https://github.com/ucsb-csw8/s22> |
| Summer 2022 <br />(Kharitonova) | m22-ykk    | <https://ucsb-csw8.github.io/m22-ykk/> |
| Summer 2022 <br />(Elsayed)     | m22-shereen| <https://ucsb-csw8.github.io/m22-shereen/> |
| Winter 2023 <br />(Conrad)      | w22c       | <https://github.com/ucsb-csw8/w22c> |
| Winter 2023 <br />(Kharitonova) | w22k       | <https://github.com/ucsb-csw8/w22k> |

## Step 3: Fork the course website

<details>
<summary>
If aren't familiar with how to 'fork a repo' click the ▶ character at left to open this section and learn more.
</summary>

Navigate to the course repo. In the instrucitons below, I'm showing the interface for
the `w23k` repo:




We will use this course's repository in order for you to practice the open-source model of collaborating on a `PROJECT_REPO`. 

In the open-source model, there is one or more owner and maintainer of the project repository.

Typically, you as a contributor do not have a direct access to making changes to the repo -- the way you contribute is by submitting your suggestions/modifications via **Pull Requests**.

In this example, we will be referring to this course's website as the `PROJECT_REPO`.

### Fork the repo

**Fork** the `PROJECT_REPO` using the GitHub interface. 

You can get the `PROJECT_REPO` URL/address by clicking on the green "Code" button on the GitHub's website.

Note that **the _forked_ repo will produce a different URL** (i.e., web address) for each person who forked this repo. We will refer to it as a `PROJECT_REPO_FORK`.

You'll be making changes in your forked copy.

</details>





------
------
------


---

At this point, you have two alternative routes that you can take (each is described in its respective section below):
* you can continue adding the files using the GitHub web interface
* you can continue adding the files using `git` and the command line

You will need to make the changes to **your fork** using _one_ of the above options. 
Then, when you have your picture and bio uploaded, you will need to **submit a Pull Request** (PR) via the GitHub web interface.

---

### Add your files using the GitHub interface

In this assignment we ask you submit a recent photo and bio to share with our students. The idea is to help them get to know you better.
If you really don't want your photo on the website, use the image that's listed in the `_example.md` file.

#### Step 1: Navigate to your fork
 In the browser, open up the `PROJECT_REPO_FORK`. (_Note that you need to open **your fork**_, not the original course repo.)

#### Step 2: Upload your picture
* Navigate to the `assets/images` folder and select "Upload files" from the "Add file" dropdown. 
	* Use an image that shows your face and helps students recognize you.
	* Use a **square** PNG image (300x300 px max resolution).
	* Use the naming convention `XX-QQQ-FirstName-LastInitial.png`, where `XX` is the course number that you are tutoring for (e.g., `CS08`, `CS09`,  `CS16`, `CS24`, `CS90DA`,  `CS130`, `CS130B`, `CS148`, `CS156`) and `QQQ` is this quarter (e.g., `W21`, `S21`)

* After uploading your image, remember to "Commit changes".
	* Save the filename for the image that you uploaded.

#### Step 3: Upload your bio
Now, navigate to the `_staffers` folder in the `PROJECT_REPO_FORK` GitHub repo. 

* Select "Create new file" from the "Add file" dropdown. 
* Name your file `NETID.md` making sure to substitute _your_ `NETID` (all **lowercase**) before the `.md` part (`NETID` is the part that comes before your `@ucsb.edu`).
* Copy the following template and update the fields accordingly.
	* Leave the opening and closing dashes intact.
	* Update your `name`
	* Update the `pronouns` to only include yours
	* Leave the `role` as the `Undergraduate Learning Assistant` (_don't change it or add anything to it_)
	* Use the base filename (not the path) for the `photo` that you uploaded (_make sure that you added it to the correct folder_)
	* Add your bio - please, **do not** list your contact information as part of your bio.

```
---
name: Your Name
pronouns: She/her Him/his They/their
role: Undergraduate Learning Assistant
ula_for: CS X
photo: image.png
---

Write your bio and a welcome message for the students in your course (300 to 400 words). 
```

* Remember to "Commit changes".

---




### Add your files using the command line


#### Clone the (forked) repo

Now that you have your own fork `PROJECT_REPO_FORK` (i.e., copy of the `PROJECT_REPO`), which is connected to the main `PROJECT_REPO`, it's time to **clone** the fork to your local computer.

You can get the `PROJECT_REPO_FORK` URL/address by clicking on the green "Code" button on the GitHub's website. 

> To quickly check that you are cloning the correct repo (i.e., the fork, not the main project), look at the name of the repo in the top left portion of the website: it should show `YOUR_GITHUB_USERNAME / PROJECT_REPO` and underneath it should say **"forked from"** and link to the main `PROJECT_REPO` address.

To clone  `PROJECT_REPO_FORK` to your computer, open a Terminal window and type:
```
git clone PROJECT_REPO_FORK
```

**Note**: if you type `pwd` (i.e., _print working directory_) it will produce a path to the folder on your computer which now contains a cloned version of your forked repo (`PROJECT_REPO_FORK`). 

You can verify that the new repo is there by running `ls -l` (Note: _these are not ones (1) but "ells" (lowercase Ls)_). Once you run the `ls` command you should see your `PROJECT_REPO_FORK` folder on the list.

Congrats! You can now switch to that folder by typing
```
cd PROJECT_REPO_FORK
```

If you run `ls` you should see the README.md and other files in this repo.

Woohooo! We are done with the setup and are ready to start working with the files.

---

Follow the instructions and requirements above for uploading your picture and the bio. 

Since you are working on the command line you'll need to add
* your picture to the `assets/images` folder
* your bio to the `_staffers` folder


#### Add the files to your fork

* Verify that your changes are detected by running `git status`. It tells you which files you have modified. 
* If the file that you created is "red" in the "Untracked files" category, make git aware that it needs to keep track of it: Add the changes by running `git add`, followed by the path/name of your files.
* See the difference by running `git status` and make sure that only the files you intended to change are “green”.
* Commit your changes by running this on the command line: `git commit -m "Added a profile picture and the bio."`
* Make your change show up on your fork's github repo website by pushing this commit to the repo using `git push` (note: not including `origin <branchname>` after `git push` defaults to `origin master`).

**This commit and the correspending files now live in _your fork_ and not in the main `PROJECT_REPO`.**

When you are ready for your changes/files to show up on the main website, **submit a Pull Request (PR)**.

### Submit a Pull Request (PR)

In order for your changes to be added to the main `PROJECT_REPO`, you need to issue a **Pull Request** (usually abbreviated as PR).

Pull Requests (PRs) are typically issued through the GitHub web interface. 

To submit a PR go to the `PROJECT_FORK_REPO` page on GitHub. Click on the "Pull Requests" **tab** and click on the green "New Pull Request" button.

**Important**: make sure to select the "`compare across forks`" link and then set the `base` and `head` repositories and branches accordingly.

Fill out the necessary information and then to finalize your PR, click on the green "Create Pull Request".

---------

# Acknowledgement / Contact Me

If you have any questions or suggestions, don't hesitate to reach out to me via ykk@ucsb edu (remember to replace a space with a `.` between the `ucsb` and `edu`).

For attribution, please keep the reference to the author:

> Content developed and released under the CC BY 4.0 by Yekaterina Kharitonova.

------

If you would like us to add or correct anything, feel free to use the `edit this page on GitHub` link below and then submit a Pull Request from your forked repo.

**Acknowledgement**

Developed by Yekaterina Kharitonova and edited by Phill Conrad
{: .fs-2 }

