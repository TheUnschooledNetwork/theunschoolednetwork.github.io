---
title: Contributing to Unschooled
date: 2025-01-17 12:00:00 -500
categories: [Unschooling, Guides]
tags: [unschooled, contributing, how-to]
pin: true
toc: true
image:
  path: /assets/img/Posts/tungsten.jpg 
  alt: the one light in the dark by Patrick Brosset is licensed under CC BY-NC 2.0.
---
 
### **Guide Overview**  

This guide will walk you through the process of adding a post to the Unschooled Network using GitHub and Jekyll. 

By following this guide, you will:  
- Set up the necessary tools (Ruby, Jekyll, Git)  
- Clone the website’s repository from GitHub  
- Create a new post using Markdown  
- Preview your post locally on your computer  
- Submit your changes to GitHub using a Pull Request  

### **Prerequisites**  
Before proceeding, ensure you have the following:  

1. **A GitHub Account** – If you don’t have one, create it at [GitHub.com](https://github.com).  
2. **Git Installed** – You should be comfortable using the command line (Terminal on Mac/Linux, PowerShell on Windows).  
3. **GitHub Authentication** – Make sure you're logged into your GitHub account and have set up authentication (using HTTPS or SSH). If unsure, follow [GitHub’s setup guide](https://docs.github.com/en/get-started/getting-started-with-git).

---

Now that you you are all set up, let's get started 

### **Installing dependencies**
First thing's first, make sure you have the necessary tools installed:  
```bash
sudo apt update
sudo apt install ruby-full build-essential zlib1g-dev git
```

If you are using Bash (the default for most systems), configure Ruby Gems.

```bash
echo '# Install Ruby Gems to ~/gems' >> ~/.bashrc
echo 'export GEM_HOME="$HOME/gems"' >> ~/.bashrc
echo 'export PATH="$HOME/gems/bin:$PATH"' >> ~/.bashrc
source ~/.bashrc
```

Install Jekyll and Bundler

```bash
gem install jekyll bundler
```
### **Cloning The Repository and Creating a New Branch**
Clone TheUnschooledNetwork.github.io Repository and install dependencies.

```bash
git clone https://github.com/TheUnschooledNetwork/theunschoolednetwork.github.io.git
cd theunschoolednetwork.github.io
bundle install 
```

Before adding a new post, create a new branch:

```bash
git checkout -b my-new-post
```

This will create a new branch and switch to that branch. This will ensure that your changes do not apply to the main branch until they have been reviewed by the project maintainers. 

### **Adding A New Post**

Navigate to the `_posts/` directory and create a new Markdown file following the naming convention

```bash
cd _posts
nano YYYY-MM-DD-title-of-your-post.md
```

> You can also open the file with [Visual Studio Code](https://code.visualstudio.com/docs/setup/setup-overview) by using the command 
```
code YYYY-MM-DD-title-of-your-post.md
```
{: .prompt-tip }

Use the following front matter template at the top of your file 

```yml
---
title: "Your Post Title"
date: YYYY-MM-DD HH:MM:SS -500
categories: [your-category]
tags: [your-tags]
---
```

Write your content following [markdown formatting conventions](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet) and [_Writing a New Post_ on Chirpy](https://chirpy.cotes.page/posts/write-a-new-post/). Then, preview your changes locally.

Additionally, you may wish to make use of our working document with [Resources for Content Creation](https://theunschoolednetwork.github.io/posts/Useful-Content-Creation-Resources/)

```bash
bundle exec jekyll serve
```

then open `http://localhost:4000` in your browser to check your changes.

### **Commit and Push Changes to GitHub**
Once satisfied with your edits, you will push (submit) these to our GitHub repository. But before doing that, check the status to see which files have been modified

```bash
git status
```

You should see your new post listed as an untracked or modified file. Stage it for commit. 

```bash
git add _posts/YYYY-MM-DD-title-of-your-post.md
```

Now, commit your changes with a descriptive message before pushing them.

```bash
git commit -m "Draft: Initial version of 'My Post Title'"
```

Push your changes.

```bash 
git push origin my-new-post
```
### **Submit/Update Your Pull Request (PR)** 
Now that your changes have been uploaded to GitHub you can submit a Pull Request (PR). This is the process by which you can propose changes to TheUnschooledNetwork main repository. 

Open a browser and navigate to [TheUnschooledNetwork.github.io](https://github.com/TheUnschooledNetwork/theunschoolednetwork.github.io) repository

You should see a notification that your recently pushed branch is available to create a PR. Click the "Compare & pull request" button.

Fill out the PR details, adding a title and brief description. Lastly, make sure you are merging your branch into `main`. 

Submit and await review by clicking "Create pull request." Wait for feedback from us. If changes are requested, make the edits locally, commit them and push again using 

```bash
git push origin my-new-post
```
After submitting the PR, check back on GitHub for any feedback or requested changes. You can respond to comments directly in the PR discussion and continue updating your branch until it is approved.

The PR should update automatically. Once approved, your post will be merged into the main repository and become part of The Unschooled Network. 

> For info about creating an account on our BTC Pay server to accept payments non-custodially, please contact theunschooled@proton.me
{: .prompt-info }