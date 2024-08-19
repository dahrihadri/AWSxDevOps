# AWSxDevOps Series II - Setting Up A Git Repository with AWS CodeCommit
Now onto Project TWO of the series, where I will share how to store my web application's source code in a repository. Now that I have some Java source code locally, let's store the source code in a Git repository.

![s1-architecture](assets/screenshots/s1-architecture.png)

## Introducing AWS CodeCommit!

### What it does & how it’s useful
AWS Cloud9 is a cloud-based IDE that lets you write, run, and debug code with just a browser. 
Developers and teams use AWS CodeCommit because It integrates seamlessly with other AWS services, supports collaboration, and ensures code security and version control. 

### How I’m using it in today’s project
I’m using AWS CodeCommit to store, manage, and track changes to my project's source code. It helps ensure version control, allows for collaboration, and integrates seamlessly with other AWS services for a smooth CI/CD pipeline. 

### This project took me
This project took me about 20 minutes to complete, including setup, coding, and testing. Documentation took me around 30 minutes to write, ensuring detailed and clear instructions for each step. 

**Difficulty**: Easy peasy  
**Time**: 50 mins  
**Cost**: $0  
**Tools Needed**:
- An AWS account - [Create one here!](https://aws.amazon.com/free/)

## AWS Services Used

- AWS Cloud9
- AWS IAM
- AWS EC2
- AWS CodeCommit

## What I'll share in this second project series:

   - ⚙️ `Set up a CodeCommit Repository`: I created a new repository in AWS CodeCommit to securely store and manage the source code for my Java web app.
   - ☁️ `Configure Git in Cloud9`: I established my Git identity with my username and email, so my changes to the repository are properly attributed to me.
   - 📂 `Initialize and Configure Your Local Repository`: In the Cloud9 environment, I initialized a new Git repository. I set up your CodeCommit repository as the remote origin, preparing the path to    synchronize my local and remote repositories.
   - 🫸 `Make Your First Commit and Push`: I added all my files to the staging area, committed them with a message marking the "Initial commit", and pushed these changes to the main branch of my CodeCommit repository, making my code available in the cloud.
   - 🗂️ `Understand and Organize Your Project Structure`: I've learned about the essential files in my repository, such as the src directory for my source code, and the pom.xml file for managing my Maven project's dependencies and settings. 

## Table of Contents

- [Prerequisites](#prerequisites)
- [Steps](#steps)
  - [Step 1: Create a Git repository](#step-1-create-a-git-repository)
  - [Step 2: My first commit](#step-2-my-first-commit)
  - [Step 3: Git Action](#step-3-git-action)
- [My key learning](#my-key-learning)
- [License](#license)

## Prerequisites

- An [AWS account](https://aws.amazon.com/free/) (Free Tier eligible)
- Basic knowledge of HTML

## Steps

### Step 1: Create a Git repository

- Git is a distributed version control system that tracks changes in source code during software development.
- A Git repository is a storage space where your project's source code and its revision history are kept, enabling version control and collaboration among developers.
- To create a Git repository in the cloud, I used AWS CodeCommit, a secure and scalable source control service.

<p align="center">My setup page for a CodeCommit repo</p>

![set up for my AWS Account](assets/screenshots/set-up-for-my-AWS-Account.png)


### Step 2: My first commit

- I initialized a Git repo in my web application by running the command git init -b main in my Cloud9 IDE.
- To commit and push my code, I will have to run three different commands in order:
   - `git add .` - This adds all changed files to the staging area.
   - `git commit -m "Initial commit"` - This commits the changes with a message.
   - `git push -u origin main` - This pushes the commits to the remote repository.

<p align="center">File I committed showing up in my CodeCommit repo!</p> 

   ![My Cloud9 IDE](assets/screenshots/My-Cloud9-IDE.png)

### Step 3: Git Action

- I wanted to see Git working in action, so I changed the index.jsp file in Cloud9 by adding a new line of text.
- Then I tried seeing these changes in my CodeCommit repository, but this didn’t work because I hadn't pushed my changes from my local Git repository in Cloud9 to the remote CodeCommit repository.
- I finally saw the changes in my CodeCommit repository after running git push in my Cloud9 terminal to push my committed changes to the remote origin (CodeCommit repository).

<p align="center">My updated index.jsp file showing up in CodeCommit!</p> 

   ![My Cloud9 IDE](assets/screenshots/Maven-and-Java.png)


### My key learning

1. Git is a DevOps tool used for source code management. It's a free and open-source version control system designed to handle projects of all sizes efficiently. Git tracks changes in source code, facilitating collaboration among multiple developers.
2. A local repository refers to a copy of a Git repository that resides on your computer. It allows you to work on your project locally, making changes and staging them before pushing them to a remote repository like AWS CodeCommit.
3. To commit your code in Git, you typically run these three key commands
     - `git add .` - This command stages all changes in your working directory for the next commit.
     - `git commit -m "Your commit message"` - This command records the changes staged in the previous step to your local repository.
     - `git push` - This command uploads the changes from your local repository to the remote repository
4. One thing I didn’t expect was the seamless integration between AWS CodeCommit and Cloud9, which simplified my workflow for version control and development. 

## Great! 
### We are done with series II

   ![s1-architecture](assets/screenshots/s1-architecture.png)

## Find this helpful?
Let's Connect and Feel free to reach out or follow me in [LinkedIn](https://www.linkedin.com/in/dahrihadri) for more updates on my journey through AWS and DevOps!

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

# Lets continue our AWSXDevOps project in [Series III](https://github.com/dahrihadri/AWSxDevOps/tree/main/Series-III) ! 🌟
