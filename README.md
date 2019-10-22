# BHTO19_StarterProject

This repo is a special offering for BHTO2019 newbies. 

It is designed to be relatively self-contained, self-explanatory, and catering to all ability levels. 


## Using this repo

Here are the things you will need to do to get going with contributions on this project.  

More details on each step are listed below. 


1. If you don't have one, get a github account. 

2. Fork this repo

3. Make a local clone your fork

4. Choose a task to work on from the issues list  

5. Hack!  

6. Contribute your wonderful contributions back to this repo

7. Return to 4. 



***Your first task will be to add your name to the contributors list***

Recommendation: repeat with a few small, unambitious changes (e.g. to documentation files) to get the hang of the contributor workflow. 






## In more detail

### Fork the repo

- Sign in to github
- Navigate to this page
- Click the `fork` button (top right of this page)

### Make a local clone of your fork

#### Install git on your local machine

#### Tell github about your local machine

*Generate an ssh key for your machine*
 
On the git command line type 


```bash
ssh-keygen
```

*Tell github the publich half of your generated ssh key*

```bash
cat ~/.ssh/id_rsa.pub
```

Select + copy the public ssh key

In the browser: 

- Go to github
- ...your github settings (not the repo settings)
- ...ssh and gpg keys
- ...create new ssh key; paste in the locally generated public key


#### Clone your fork

```bash   
git clone git@github.com:yourgithubusername/BHTO19_StarterProject  
```

(Note: this command is different the one you use for repos you don't intend to push changes to, which is just `git clone <repourl>`)


Tell your local clone where the upstream master repo is

```bash
cd BHTO19_StarterProject  
git remote add upstream https://github.com/JohnGriffiths/BHTO19_StarterProject
```

To pull updates (you will need to do this regularly)

```
git fetch upstream
git merge upstream/master
```


### Choose a task

Look at the issues list in the master repo. 

Choose a task you find interesting and you think you can do. 

Questions + discussions can be done on the thread


### Hack

#### Create a new branch

First: create a new branch from the `master` branch. This is where you will make your changes. When you are ready to contribute your updates back to the master repo, you will submit a pull request for the entire branch. 

```bash
cd BHTO19_StarterProject  
git checkout -b newbranchname
```

Check what branch you're on and the status of the branches in your local repo clone:

```bash
git branch -a -l
```

#### Make your changes


#### Record your changes

```bash
git add changedfile
git commit changedfile -m"description of change"
git push origin newbranchname
```

Check your local github fork in the browser. 



#### Check for updates

```bash
git fetch upstream
git merge upstream/master
```





### Contribute back

Once your new contribution is finished and you are ready to have it merged into master: 

#### Submit a pull request







---
---

***Project Organizer Notes***

Plan for this project: 

Basically, we will list a number of new tasks based off the things done in the edu course, which will use 

[this repo](https://github.com/josephmje/scwg2018_python_neuroimaging/blob/master/bin/07_functional-connectivity-analysis_solutions.ipynb)

so check out the repo contents and start listing ideas as issues


To do: 

- get+add the link(s) for the educational project(s) repo(s)
- make decisions re: data availability+access, if important
- build out issues list with lots of handholding
- replace this list with a readme for people
- change the name?


Ideas:
- Fingerprinting on control subjects vs SCZ -- do psychiatric conditions affect how well we can fingerprint
