# Introduction

Why hello there! This section aims to help you get started with the development process using Next.JS + TypeScript + Tailwind CSS. You will find all the necessary installations as well as quick tutorials for each of the tech stack and development process
used here. If you have questions about how things work and are connected to one another, don't worry! There will be a lot of information here. This project moreorless kills two birds with one stone. First, to help teach you the typical development process 
in software engineering (i.e. creating your own project, working in a team, etc...) that you might really not get from school and of course, building your own personal website (althought this is more for fun and for the business ;D).

## Pre-requisites
There are a few pre-requisites you'll need to have in order to know what's going on and to not be completely lost but I'm sure you already have most, if not, all of these. You should have a solid understanding (maybe not solid but basic) of the following:
- HTML5 (This is like the skeleton of your web pages which generates your structure)
- CSS3 (This language is mostly responsible for applying the styling to your webpage and makes it look aesthetic)
- JavaScript (This will essentially be the logical portion of the app, to make it interactive and respond to certain events such as what happens when you click buttons, etc...)
- Git/GitHub (Git for version control and GitHub as the cloud repo to store all these changes with an intuitive UI for collaboration)
- React.js (I know you probably don't have a clue how to use React which is okay since I'll basically be teaching you in this project)
- Figma (This is optional if we want to use this for prototyping our designs)

## Post-requisites
By the end of this project, you'll have learned a lot which may (or may not) help you when it comes to working in a co-op/internship or even securing one!
- React.js (In my honest opinion, arguably the most useful and intuitive frontend framework and makes frontend development very seamless)
- Next.js (You may be wondering what is Next.js, and thought that we were making this project in React.js but I'll explain a little later down in the document)
- TypeScript (Another language woohoo! I've already mentioned this but if you know JavaScript, you already know TypeScript)
- Tailwind CSS (Our utility CSS library. I'll explain more on this in another section as well)
- Vercel (This will be our deployment service where we can host our website. Next.js is actually made by Vercel so they're basically a package deal - another reason why we're using Next.js)
- Utilizing Git Actions/Issues and Software Development Process/Workflow

# Tech Stack
I've already mentioned the tech stack we're going to be using but you still may have a lot of questions like "Why this tech stack?", "What's the difference between different tech stacks?", "Why does it matter?" and a bunch of other questions. In this section
I'll aim to cover the reasoning behind this and why it'll matter. In short, it's to streamline the development process. We want to make developing as easy as possible for us while still remaining inside the realm of feasability. We want to use things that
have already been developed instead of re-inventing the wheel (Why re-invent the wheel when we can just use it?).

## Next.js
This is going to be what our entire project is built using. So you may be wondering? What is Next.js and what's the difference between Next.js and React.js? In short, Next is a framework that's build on top of React, just like how React is a framework
built on top of JavaScript. This means you need to learn how to write and code in JavaScript before developing in React and that you should know how to develop in React before Next. You may feel overwhelemed by skipping React but don't worry, it'll be a fun
journey :D. Next basically is a React-App that provides a lot of useful features such as server-side rendering (SSR), easy out of the box routing and many other features. For the most part, if you want to build a frontend project, React is the way to go.
However, when it comes to e-commerce websites, Next.js just shines brightly and is like the golden ticket for developers.

If you want to learn more about Next.js I recommend reading this [tutorial/documentation.](https://nextjs.org/)

## TypeScript
Next on our list is our best friend TypeScript. Honestly, this have became such a widespread and popular language and I can definitely see why. Like I've said multiple times, if you know JavaScript, you already know TypeScript. Like you learned in discrete math
set theory. TypeScript is essentially a "superset" of JavaScript. That means everything you have in JavaScript, you also have in TypeScript. All JavaScript code is valid TypeScript code. As the name implies, TypeScript is literally "JavaScript with Types". (Even the 
logo is basically the same! Minus the color scheme and letter). 

Learning TypeScript is not as difficult as learning JavaScript initially. You know with statically typed languages like Java and C, you have types such as "int", "double", "String", where as for dynmaically typed languages like JavaScript and Python you don't need 
to define types (i.e. myList = [] in Python, let myList = [] in JavaScript). The problem with this is that we don't perform any error checking until run-time, which can be bad since we don't know when an error or fault occurs until we encounter them. It's like 
the same as launching a rocket and finding the fault there vs running a simulation of the rocket before launch and finding the error in the simulation. Obviously, we'd rather find when the error occurs in the simulation than when we actually launch it. 

TypeScript enforces us to declare types so we know what type of data we are working with and if they are compatible or not. This gives us a way to see any potential errors that could arise before we actually deploy or run our code. When you launch your webpage though, 
the only thing you'll really see are HTML, CSS and JavaScript files. You will never see a TypeScript file. This is because all TypeScript files gets "transpiled" down into JavaScript files. TypeScript is essentially just a tool to help the developer in debugging 
their JavaScript code. 

I do suggest reading the [docs](https://www.typescriptlang.org/docs/handbook/typescript-from-scratch.html) for TypeScript to gain a little more familiarity. If you are a visual learner instead of a reader, there's plenty of tutorials on
YouTube that should not take more than 1-2 hours to learn TypeSCript. Here is one example [video](https://www.youtube.com/watch?v=d56mG7DezGs).

## Tailwind CSS
Our next tech stack is going to be my favourite CSS utility library, Tailwind. Honestly this just makes writing CSS a lot easier. Instead of creating .css files and then importing them and giving each DOM element a specific class name, we can just use some
built-in keywords to define what style we want to apply. This reduces the need to create .css files which helps reduce the load time and also makes it pretty clear which styles are applied to which elements instead of having to navigate back and forth
between files. 

There are other utility libraries out there like BootStrap, MaterialUI, and others but Tailwind has been my favourite amongst them. The aesthetics match mine and it just seems more modern. A lot of companies out there also use Tailwind so it's quite
a plus to know this. Something to keep in mind is that a lot of companies do not use vanilla CSS, they'll more than likely use some sort of utility library but you should still know vanilla CSS since the more you know of it, the easier it is to use Tailwind.

You can read more in their [docs](https://tailwindcss.com/docs/installation) or watch a tutorial on [YouTube](https://www.youtube.com/watch?v=ft30zcMlFao). This is a long video so don't feel as if you need to watch this in one sitting. You may even learn more
as we do it and if you ever have questions just let me know! Though the best way to learn is to struggle through it and play around with it. CSS is arguably one of the harder languages to master but once you've mastered it, you can plow through developing frontend
designs very easily.

# Software Development Process
This section will aim to teach you the generals of using Git and GitHub in a team environment. We'll also be using a lot of Git and GitHub. Git is the version control software whereas GitHub is a medium to store all those projects/repos (Don't get these mixed up). Git works with many other cloud repository such as GitHub, GitLab, etc... GitHub just tends to be more popular (and is also my choice too looool).

## Git
When it comes to Git, some of the most useful commands I use on a daily basis are:
- **git fetch** (this basically tells us that there are new changes in the remote repo that we should pull from but does not copy it into our working repo)
- **git pull** (this basically runs git fetch and then git merge so that you get all the changes from the remote repo into your working directory)
- **git branch** (lists all your branches in your working directory)
- **git checkout -b \<branch-name>** (this creates a new branch off of the current branch you are on)
- **git checkout \<branch>** (allows you to switch between branches)
- **git branch -r** (Lists all the remote branches. If you do git checkout \<branch> with \<branch> being one of the red highlighted branches, you basically pull down a copy of that remote branch to yours. This is useful if you want to checkout someone else's branch)
- **git branch -D \<branch>** (deletes a branch. if you want to delete the current branch you're in, you have to first checkout to a different branch)
- **git branch -m \<old> \<new>** (renames an old branch into a new branch)
- **git status** (checks how many commits behind/ahead you are of the current branch that is in the remote repo)
- **git add .** (adds all unstaged files to your staging area. You can replace "." with a specific file path if you only want to add one or specific files into your staging area)
- **git commit** (useful for multi-line commits; personally what I use)
- **git commit -m \<message>** (commits what you have in your staging area with the commit messaged declared in \<message>)
- **git commit --amend** (useful if you've already committed a change but you made a new change that you think fits in with the previous commit. Thought not intended to, can also be used to rename or retouch the previous commit)
- **git stash** (adds all non committed changes to a stack; useful if you found like you've been working in the wrong branch but have not committed your changes and you try to checkout into a diff branch but terminal is complaining about having uncommitted changes and that you need to abort or stash, then use this. also helpful if you want to temporarily stash away what you have to temporarily get the original state of the branch back)
- **git stash pop** (pops off the top most changes in your stack into your current branch)
- **git restore .** (basically restores the modified file back to its original state in the latest commit. imagine you made some terrible mistakes in the current file and you want the originally copy. In that case, just run git restore \<file> for the file you want to restore or use a "." to restore all files. Careful when using this operation since you will discard your changes. I only use this when I know I messed up and want to start clean again)
- **git restore --staged .** (unstage all currently staged files. Replace "." with a file path if you want to unstage certain files)
- **git reset --\<soft | mixed | hard>** \<commit tag ID> (a little more tricky to explain so I suggest searching this up if you want to redo a commit)
- **git rebase** (this gets situational but for the most part, you won't need to do this unless you want to pull in changes that I've pushed up)
- **git rebase -i** (interactive rebasing, provides lots of option for squashing, merging, fixing, renaming, deleting previous commits, this is situational as well)
- **git merge** (I honestly don't do this much since I follow a typical branch workflow and work independently from other branches. I prefer to use a rebase over a merge since a rebase provides a cleaner tree history)
- **git push** (pushed your branch to the remote repo and updates it)
- **git push -f** (force push your changes to the remote repo; useful if you ammended a commit and want to override what's currently in the remote repo)

## GitHub
This section will aim to teach you how we actually use GitHub collaboratively. We mostly make use of 2-3 things within GitHub. The "Issues" section and the "Pull Requests" section (maybe the "Actions" section if we want some sort of Ci/CD testing). The "Issues" is where
we're going to keep track of all the tasks that needs to be done and their current progress. This allows us to see who's in charge of specific tasks, and any pull requests linked to it. In the "pull requests" tab, we'll see a list of all open and closed pull requests. This is essentially any features, fixes or code changes you want to merge in from one branch to another. Ths reason it's called a "pull request" or PR for short is that you should think of in terms of the main repo and that the person making the PR is trying to get you
to pull in their new changes. Typically we need some sort of reviewer for these PR to make sure the new code changes, once merged, does not break our main/"clean" branch since all other branches will eventually be derived from this and we don't want to propagate
errors down to every branch.

## Creating and Utilizing Feature Branches
Whenever you want to work on a new feature or fix something, make sure you are working in your own branch. This just makes development cleaner since you'll be working on a "side copy" instead of the main copy and if you ever screw something up, then you can just
discard your branch and create a new clean copy off the main branch. The general workflow for creating your own branch is as follows:

- git checkout main
- git pull
- git checkout -b \<feature-branch-name>
- git push -u origin \<branch>
  - or you can alteratively just do: git push and then copy and paste the line they suggest (if your branch is not already up in the remote repo)
  - you can also do this after you've made changes to your remote branch so you don't push an empty branch up
- code changes, add to staging and commit
- git push (while in your feature branch)
  - this will push the current changes in your working directory to the remote repo and update it
- go to GitHub and create a PR to merge feature branch into main branch
- resolve merge conflicts (if any) and request a review
- if approved, then merge the PR
- repeat

## Commit Message Conventions
Typically the convention for commit messages depends on who/which company/team you're working with. Sometimes they're not too strict but I always like a clean and descriptive commit history so I know what each commit is doing and what's going on. I usually follow a standardized convention for naming my commits and I think it's a good practice to follow it. Here are some examples commit messages and specific keywords to prepend to your message for better context:

- chore (if the commit pertains to anything chore related like updating package version or dependencies)
  - chore: updated tailwind dependency version
  - chore: added eslint as a dev dependency
- fix (if the commit fixes a bug or any development issues)
  - fix: removed redundant white spaces in navbar title
  - fix: resolved persisting UI bug on modal dismiss
- feat (a new feature or implementation)
  - feat: implemented a carousel for list of services
  - feat: added submission buttons to end of form
- enhan (an enhancement - I typically use this when I just needed to populate certain data)
  - enhan: added more resume points into resume-points.json
  - enhan: changed cancel button color from red to blue
- deprecate (when we want to deprecate a feature or service or dependency)
  - deprecate: marked doneButtonV1 as deprecated and replaced with doneButtonV2

This is much more description than having a commit message like "updated buttons" since we can see the starting phrase to identify what type of commit it'll be and the following message to describe the new change. We can also add comments to
commits if we use **git commit** instead of **git commit -m \<message>**.

# Installations and Running the Development Server
In order to work with this project, you'll need to have a working version of node and npm. You can download [Node](https://nodejs.org/en) here and download npm via node (run `npm install -g npm` within the terminal). To check if you have a running version
of node and npm, you can run this in the terminal (`node -v` and `npm -v`).

Once those two have been installed, you can clone this repo (there's a Code > Local button within the Code tab to give you the https/ssh link). We will use HTTPS so we do not need to configure an SSH key. Run `git clone https://github.com/chene40/zen-nails-web.git` within your terminal of a working directory of your choice (I ran this in my Desktop directory).

Once you have cloned the repo, you can open VSCode (if you haven't already) and open up the cloned repo/folder.

Make sure you are at the folder's root directory (e.g. Desktop/zen-nails-web) and run `npm i` to install all the node dependencies for the project.

Run `npm run dev` to start the development process and open up the link that's listed in your terminal (should be something like `http://localhost:3333`).

Congrats you've got everything you need! In this project, we have hot module replacement, which means that any changes you make to the code will update the page in real time. So you do not have to run any scripts to build the project and then
re-run the development process or refresh the page. 
