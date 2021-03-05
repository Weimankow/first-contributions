
Hi there! If you are unfamiliar with Github, but have a passionate desire to update any of the practices on the practices site, this readme aims to simplify and guide the way to making your first contribution. 

If you are looking to make your first contribution, follow the steps below.


# Workflow overview

It takes many small steps to make a contribution, but conceptually these are the 5 major things you have to do.

1. Prepare: Type up your suggested edits 
2. Fork: Forking just means creating a copy of the practices site code for your GitHub account
3. Edit: Copy and paste suggested edits into the code in your copy of the practices site through the GitHub UI and save it in a branch
4. Pull Request: Pull Request is the technical term for submitting the suggested edits to be reviewed, approved by someone else and updated on the site
5. Delete: When the change is approved, delete your copy of the practices site.

Repeat steps when you want to add new changes to the site.

# Step by Step Instructions 

## Prepare
1. Type up the changes you want to make for the Practices site.
2. Create a Github account, if you don’t have one. Login to your Github account, if you do.
3. If you’re doing this for the first time, set aside up to 30 minutes.

## Fork (Create a copy of Practices site)
1. Go to the [VMware practices repository on Github](https://github.com/vmware-tanzu/tanzu-dev-portal/tree/main/content/practices) - this is where all the code for the site sits. It is also open to the public for contribution. 
2.  Click on fork
3. Fork it to your own Github account
4. Click on Content
5. Click on Practices. You’ll see a list of all the practices currently on the site.
6. Click on the practice you want to add to. For this example, I clicked on design-studio.
7. Click on index.md. You can now see what the page looks like in plain text
8. Click on the pencil edit icon. You can now see what the page looks like in markdown language. Don’t worry, markdown is a simplified HTML/CSS script. 

## Edit (Make Edits and save as branch)

1. Paste your edits into the right section. Just note that if you’re adding a ‘header’, ‘callout’ or any form of special formatted text, take a look to see how headers have been written, so you can copy the syntax. 

For example, I added a tip here. A tip is written like this:
 {{%callout%}}
My tip
 {{/%callout%}}

Try to keep to the indentation format so that the text looks neat and readable.

2. Scroll down to the Commit Changes section, and fill in the title. It defaults to ‘Update index.md’, but give it a short summary of what you did in less that 50 words
3. Fill up the extended description with the reason why the update was needed, or the context around the update.
4. Select ‘Create a new branch for this commit’
5. Create a name for the new branch that explains what it is 
6. Click Propose Changes. Do NOT click the ‘Create Pull Request’ button that appears in the next screen. 

## Pull Request (Submit edits for review)

1. Go to the Pull Requests tab
2. Click ‘New Pull Request’
3. Change the dropdown for your “compare: main” to the name of the branch you have created. Scroll down to check that text highlighted in green is the change you want to make. 
4. Click Create Pull Request
5. Click Create Pull Request again. This will send the edits through some automated checks. 
6. At this stage, you’re done! 
7. If you want to, you can keep the screen running until all the tests have passed, and click on the netlify row to preview how it will look on the site!
8. Otherwise. feel free to close GitHub and continue with your life. The checks will continue running even if you leave the page. Once the change passes through all the checks, it will land on the reviewers’s plate, and all you have to do is wait for it to be reviewed, approved and merged. 


> #### How will I know if the changes have passed the checks, been rejected, approved or merged?
> If there’s a change to the status of your pull request, Github will alert you via the email linked to your Github account. 
> A change in status of your pull request will also appear if you click on the notifications icon of your Github account. 
>
> #### How can I make a change to the pull request if it doesn’t pass a test, or there’s a request for edits from the reviewers?
> Go to your copy of the Tanzu Practices site, making sure that you are in the right branch to make the edits.
> Go back to the file to edit it.
> Under Commit Changes, fill in the title and description for the change.
> This time, commit directly to the branch. Do NOT create a new branch. This updates your pull request with your latest edits. 
> That’s it!

## Delete (delete repo)

Once you’re sure your edits have been merged, go to settings, and delete your copy of the repository. 











# First Contributions

This project aims to simplify and guide the way beginners make their first contribution. If you are looking to make your first contribution, follow the steps below.

<img align="right" width="300" src="https://firstcontributions.github.io/assets/Readme/fork.png" alt="fork this repository" />

## Fork this repository

Fork this repository by clicking on the fork button on the top of this page.
This will create a copy of this repository in your account.

## Clone the repository

<img align="right" width="300" src="https://github.com/Weimankow/first-contributions/blob/master/Screenshot%202021-03-05%20at%2012.57.55%20PM.png" alt="clone this repository" />

Now clone the forked repository to your machine. Go to your GitHub account, open the forked repository, click on the code button and then click the _copy to clipboard_ icon.

Open a terminal and run the following git command:

```
git clone "url you just copied"
```

where "url you just copied" (without the quotation marks) is the url to this repository (your fork of this project). See the previous steps to obtain the url.

<img align="right" width="300" src="https://firstcontributions.github.io/assets/Readme/copy-to-clipboard.png" alt="copy URL to clipboard" />

For example:

```
git clone https://github.com/this-is-you/first-contributions.git
```

where `this-is-you` is your GitHub username. Here you're copying the contents of the first-contributions repository on GitHub to your computer.

## Create a branch

Change to the repository directory on your computer (if you are not already there):

```
cd first-contributions
```

Now create a branch using the `git checkout` command:

```
git checkout -b your-new-branch-name
```

For example:

```
git checkout -b add-alonzo-church
```

(The name of the branch does not need to have the word _add_ in it, but it's a reasonable thing to include because the purpose of this branch is to add your name to a list.)

## Make necessary changes and commit those changes

Now open `Contributors.md` file in a text editor, add your name to it. Don't add it at the beginning or end of the file. Put it anywhere in between. Now, save the file.

<img align="right" width="450" src="https://firstcontributions.github.io/assets/Readme/git-status.png" alt="git status" />

If you go to the project directory and execute the command `git status`, you'll see there are changes.

Add those changes to the branch you just created using the `git add` command:

```
git add Contributors.md
```

Now commit those changes using the `git commit` command:

```
git commit -m "Add <your-name> to Contributors list"
```

replacing `<your-name>` with your name.

## Push changes to GitHub

Push your changes using the command `git push`:

```
git push origin <add-your-branch-name>
```

replacing `<add-your-branch-name>` with the name of the branch you created earlier.

## Submit your changes for review

If you go to your repository on GitHub, you'll see a `Compare & pull request` button. Click on that button.

<img style="float: right;" src="https://firstcontributions.github.io/assets/Readme/compare-and-pull.png" alt="create a pull request" />

Now submit the pull request.

<img style="float: right;" src="https://firstcontributions.github.io/assets/Readme/submit-pull-request.png" alt="submit pull request" />

Soon I'll be merging all your changes into the master branch of this project. You will get a notification email once the changes have been merged.

## Where to go from here?

Congrats! You just completed the standard _fork -> clone -> edit -> pull request_ workflow that you'll encounter often as a contributor!

Celebrate your contribution and share it with your friends and followers by going to [web app](https://firstcontributions.github.io/#social-share).

You could join our slack team in case you need any help or have any questions. [Join slack team](https://join.slack.com/t/firstcontributors/shared_invite/zt-kpbyrmkk-JDkRtchcvRvQ0qK4iPmyvA).

Now let's get you started with contributing to other projects. We've compiled a list of projects with easy issues you can get started on. Check out [the list of projects in the web app](https://firstcontributions.github.io/#project-list).

### [Additional material](additional-material/git_workflow_scenarios/additional-material.md)
