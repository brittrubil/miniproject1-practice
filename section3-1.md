1. Forking vs Cloning
> _They are similar, they are related, they are not interchangeable._
- Forking
  - A fork is a copy of a repository that allows you to freely experiment with changes without affecting the original project. A forked repository differs from a clone in that a connection exists between your fork and the original repository itself. In this way, your fork acts as a bridge between the original repository and your personal copy where you can contribute back to the original project using Pull Requests.

  - *Example:* Forking a project is as easy as clicking the Fork button in the header of a repository. Once the process is complete, you'll be taken right to your the forked copy of the project so you can start collaborating!

- Cloning
  - When you create a new repository on GitHub, it exists as a remote location where your project is stored. You can clone your repository to create a local copy on your computer so that you can sync between both the local and remote locations of the project. 
  - Unlike forking, you won't be able to pull down changes from the original repository you cloned from, and if the project is owned by someone else you won't be able to contribute back to it unless you are specifically invited as a collaborator. Cloning is ideal for instances when you need a way to quickly get your own copy of a repository where you may not be contributing to the original project.

  - *Example:* To clone a repository, you need to go to the main page of your project and click the Clone or Download button to get the respository’s HTTPS or SSH url. Then, you need to open your command line or terminal and use the ‘git clone’ command to clone your repository.

2. Pull Request

- Pull requests let you tell others about changes you've pushed to a branch in a repository on GitHub. Once a pull request is opened, you can discuss and review the potential changes with collaborators and add follow up commits before your changes are merged into the base branch.

3. Adding a Collaborator to a Github Repo

- Navigate to the repository on Github you wish to share with your collaborator.
- Click on the "Settings" tab on the right side of the menu at the top of the screen.
- On the new page, click the "Collaborators" menu item on the left side of the page.
- Start typing the new collaborator's GitHub username into the text box.
- Select the GitHub user from the list that appears below the text box.
- Click the "Add" button.

4. Concept of Branching

- Branching is the practice of creating copies of programs or objects in development to work in parallel versions, retaining the original and working on the branch or making different changes to each. Each copy is considered a branch. The branches come from the trunk, also known as the master.

5. How to Use Branching

- Branching is used for version control and software management to maintain stability while isolated changes are made to code, Branching facilitates the development of bug fixes, the addition of new capabilities and the integration of new versions after they have been tested in isolation.

6. What is a Merge Conflict

- Merge conflicts happen when you merge branches that have competing commits, and Git needs your help to decide which changes to incorporate in the final merge.

7. How to Avoid Merge Conflicts
 
- You can compare your branches using the diff tool.

```
git difftool  branch1 branch2
```

- You can do a git fetch. A git fetch gives you the chance to do a git diff between your local branch and the remote branch spotting potential conflicts in the process.

```
git fetch
```
- If you like to merge often you can use git rerere. It means reuse recorded resolution. Basically it records a merge conflict that has been resolved and reuses it again when that merge conflicts happens again. This means that we do not waste time solving recurring merge conflicts.

```
git rerere
```
8. How to Resolve Merge Conflicts

- Open Terminal. 
- Navigate to the local git repository that has the merge conflict. 
- Generate a list of files that are effected by the merge conflict.
- Navigate to the parts of the files with the conflicts. 
- Then determine which changes to keep. 


