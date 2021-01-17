# Git/GitKraken

## About Git and GitKraken

According to Wikipedia, Git is a distributed version-control system for tracking changes in source code during software development. It is designed for coordinating work among programmers, but it can be used to track changes in any set of files. 

In other words, GitKraken is a GUI (graphical user interface) that provides a visual representation of the repository. Here you can see commits that members of the repository have made as well as their commit messages. GitKraken also has commonly used features such as push, pull, branch, pop, stash, etc.

## Creating a new project (Method A)

Firstly, what we like to do is create a folder for the new project or iteration. Make sure you know how to navigate to it through your computer's file explorer.

![](https://lh4.googleusercontent.com/UZQO1qyI1xjjgxC39tQYXvuXfOKhULM9VTXCH1POzKcG570ZqioVnljctmyougqB6mvtBrG747tpopwriJbYRwEp1gMsGXFcV_BxqEoNN-Jcw3re93tAeYIYWDEag7u0acctlU_B) 

For each project and lab, you will get a repository in GitHub. On the project's main screen (usually the one with the main branch) you will want to click the green button that says "Clone or Download." Then copy the link by either clicking the button (as shown in the picture below) or using Control+C.

![](https://lh3.googleusercontent.com/DNKAdlhIwP9moRURQwOktAK4ntV0_UbKUVsSkfz1tqyzaoqG_yxFeqFahxwceGfIM0fJeN0ogug0tnBwnlRGLMu3QCdyc2_639pj-BnjQ7LaaIhnb-XnRsZtoQPmq6GRkvSbiu5O)

(Screenshot below) Now open GitKraken. Click "File", then "Clone Repo." You should get a screen titled "Repository Management." Under "Clone" and "Clone with URL", you should see the Clone a Repo screen. Where it says "Where to clone to" browse to the folder that you created for the project. This folder will hold all the files for the project. And where it asks for a URL, paste the URL from the repo on GitHub that you copied earlier. Once you've completed that, click "Clone the repo!" and it'll clone the repository and open the project.

![](https://lh3.googleusercontent.com/tkB0IWjyU8gngTX8O90wqVi4OIF-RBuHvIkXF5za4ApoBE2pmNIT_pkDDdAlTY3kvmrOINxU7Ic2idzAG_3EPQieCjx_hX24HQOC5Z49lH6VMjNw4isb98vKv_a8IOlC8nFZ1jCK)

If you need to open the project or another project, go to "File" and click "Open repo", then select the folder that has the project you're looking for. You can do this in BOTH GitKraken and VS Code.

## Creating a new project (Method B)

Make sure you and your group have your repository in GitHub set up. And also have a directory for your project to go to. Now go straight to GitKraken. Choose "File" then "Clone Repo." Select "GitHub.com" and choose your group's repository and the directory where you would like to save the repository to on your machine.

## How to make a new branch

When you make a new branch, what you are doing is making a copy of the branch you're branching off from. You could think about it as parent and child branches. For example, if I want to make a new feature off the parent branch, the new branch (child branch) will be an exact copy of the parent branch. You can make new changes to the child branch and save changes without altering the original parent branch. When you are finished with changes on the child branch, you can then merge the child branch, back into the parent branch or another branch of your choosing. Now the selected branch will contain the approved changes of the child branch along with what it originally had.

![](https://lh3.googleusercontent.com/2XFh9jf4bF21dPx3j2AsihUQRJlGy5NB8gkz9DN8G8KY4gQu7PrfTdZY_aMvhv3pA0Tvz1iV7NA8mYE4n_yJrQciGYjU7_HMJWmPJ5SogbZ6hfXF4mGJiMV04qySDWsA8rR17XQZ)

When you merge a new branch into the original branch, there may be code that overlaps. So you might have different code in the same file (i.e. line 37 of app.component.ts has different code). This is called a merge conflict and is covered in a later section

To make a new branch, go to your project in GitKraken. Find the branch that you want to branch off of (the branch you want to make a copy of). Then click the "branch" button in GitKraken and give the new branch a name.

![](https://lh4.googleusercontent.com/d3cD4a_H3l96JDL1NJuBWqm7yQzBaFzaPbwSnC-0TVBjUEYnbmuhY4Ni7W62vhcBCP289ewJQW_ekTER-BVDAQQgLUY1iZT7aOV3MH0CpM3zdfthwIlq5z1kGpIqYs6mmg4OZQrJ)

After you enter the name of the new branch, you should see a new branch in the GitKraken interface that sticks out of the original branch which illustrates that you are in a different branch. When you open VS Code, you'll now be in that new branch which you can check by looking in the bottom left corner.

![](https://lh5.googleusercontent.com/jQ7UNsNtDX9ieKzzi4VHLorUnWqrIrYlR_bxu0vApfyEsczPPS636gA3PwYVDzdYyZb3hhihQd8L8pBtWU_z551LVdUgGnZTbHFj-45vsJLEAuuVVJombJB4CI7UGMbUjq5-GJ-2)

![](https://lh4.googleusercontent.com/2ONyGKGeb8rKbDG57jJ8sQPFrWel7YTcINXCuB8k7URbz_ApdUW4-JaG3HeoFr8-iFHhgbBBmvaHS-L95Cclg4UJqAwTuGNn0X3APy6PpJG2hfnuhtSKZF68RmTFEtymicBgbXGU)

When naming the branch use standard good naming practices to avoid confusion. An example of a bad name would be: "My_branch#$7" and a good example would be something more descriptive such as "doorBoard-list".

## Committing a Change

When you alter code and want to save the changes, you will have to commit your changes. Make sure that you are committing to the right branch, which you can see on the left hand side. The easiest (and most visual) way to do this, is to use GitKraken

![](https://lh5.googleusercontent.com/dVGJLuGx2yRG9CqdoPeQT62-wZW7wlxNiY6PvgqlCeGTYX_yASMQVFPFiyWTCdpy7dSrNVwYfSByPiTbUkNawUBpf4CVK80kApQVt8Y6jENAFR5ubhLIf2-nQBH6-fUhT3tTxIJh)

As the picture above shows, the file(s) that you want to save changes on will appear in the top right column. You need to hit the button "Stage File" so it appears in the box below.

![](https://lh4.googleusercontent.com/EX_YO1njlqms2ojuuWxIru5B9JlhMBEtKCcsdzHA6Y9R3PTf4d1KXh1Xyz5r3YbbWsbeoCXMTnS00opmb_5kKKqEUwpH_BHApz5SViJ4IjCLOUQF3YHf-7foeXzBo36vUxTY7LtN)

The commit message you attach to your change should be brief, but descriptive. The title for the commit is like the header of an email and should be able to tell someone what the change consists of in as few words as possible. Clicking on a file lets you view the changes that you made.

![](https://lh3.googleusercontent.com/uTrDmtnsP2lB9cAXzLFDcp4C1EAT40TLgyQFJ1gxGJN3nUhLw8xb1A9wwguNOl5PxKA0RCwS-Ytjgcu2x04PMb79Icos5QkEs5rOm4rvMUzHrrI5P0Z8FV_IRCG-CsJWFp3efTQG)

It is a good practice to commit often (especially if you make a lot of changes) to help avoid major bugs. When you make a commit, these changes are only saved locally; only you can see the change, until you push to GitHub, which leads into the next section.

## Pushing

When pushing, you are sending the recent commits to the working repository (which you can see in GitHub). This will allow other members of the repository to view changes in the branch and pull the code to their local environment. 

Multiple people can work on one branch at the same time. When you work on a branch, you are working on a local version of it. That means, the changes you make (before pushing) are only visible to you. So when working with a partner or group remotely it is important to communicate when you solve an issue so it can be pushed and everyone has access to the same working code.

![](https://lh3.googleusercontent.com/nALzV6pKu6nTQdfAmxWGGkwPZltqg7yDl5xf38_JKfHHY88W6Urm9NPLcSv2DJFmwp0K88zwcIMEZr9vqKDuh04omVmNAaO0t4_3nuU8JjHQGaf3avYG9KD11lH8bzvfgDi06RS5)

You must pull all new changes from a branch before pushing your own changes. To push, after making all your commits, hit the "push" button on GitKraken. If it works, you'll get a blue popup that says pushed successfully. If there are changes to pull, there will be a red box that prompts you to pull first. And if a push fails, you'll get a red push failed prompt.

![](https://lh6.googleusercontent.com/P_ZCnN5Jvc9O4FIX76u5hbRFdXpWnJrrS863Ukz7mwaIAfnfqvHB_ZZrhbNYCb9rxCOLUiQvOc1cx4_9zpXo6D9U1S9ILmhh_tznisTekbPYgdFylj8-FTOYdygIqhj3AjlRBAOh)

## Pulling

After pushing the changes other members of the repository will be able to pull the code to their local environment. When you pull changes for a branch, you are grabbing the changes to the branch and pulling it to your local project.

![](https://lh3.googleusercontent.com/VOKH7KNh7-ZJBaU-m61oIZNhfHPnTyrLezBjt19GZEoH-3WLOH7OIu_QCvsqsTvVYWOuxxlTNNmYEWJc3Azask7hQEMMj_MJA49RiD5jjPlKNa4apF4P83BpYW8UIYKLaJH4hFkX)

To summarize, pushing changes makes your changes to a branch available for members of the repository to see (usually your group and professors). Pulling brings those available changes to your local project.

How to Merge Branches

Any changes you make to a branch will need to be merged into either the main branch or a working branch for the changes to be utilized. For deployment all of the approved changes will eventually need to be merged into the main branch itself. 

In order to merge branches the easiest way to approach the problem is through GitKraken. Let's say you want to merge branch B into branch A. Simply click and drag branch B on top of branch A and click the "Merge branch B into branch A" option.

![](https://lh5.googleusercontent.com/9KWGzMtUnjQxkATwEOp7yNE3SsS0FmDVrhPoZCVpr8rLJG-U2UXDEGDPQW4IDdzoM0C0cQa6WG8ozKngpKj-PB0gq42ei0sh7r-TjZIPvl2lFAB1BVjs8yYcTQFQ7QCtKXiLyReM)

![](https://lh3.googleusercontent.com/JqEFgdrbvsiKbrrysKlIlw984edUd9uQbefzpPUkAOxVT8wD_HHU4-NRn65z8ibsX5maUhNI_uI5C_oMBqZWXn9941MTWN8DxCJ5OJmd20OiX-Xzpm8tGKL9xo1TAal0fL7cXl2O)

Now the changes you made on branch B will transfer over to branch A (assuming there are no merge conflicts which is the next topic). 

## Merge Conflicts

When merging 2 branches, you will often run into a merge conflict due to overlapping code, a line of code in one file may have different things on another branch. When you merge, you will often get a yellow prompt notifying there is a merge conflict.

![](https://lh5.googleusercontent.com/mlIfEcK6F2nAW0sx_QChogNzMDHk2XNfT2V7OzfxsLehphuGs4aqYZ3GaS4lnsOv4ZDq5Qxm4PiKOIVFOAsEiDXfADtxzIiShTP-FhWA3acNwB3dQiBGBufxqAktuXeOdCTxnt5D)

When you come across this, you must choose which code to keep, which ones to delete, or if you would like to keep both sets of code. In GitKraken, it will show the files that have merge conflicts on the right. Click on one of these files. You should get an A and B split screen as shown below

![](https://lh6.googleusercontent.com/mbrN-e3MmH8SkEhtqBvWw27y0y54XsTaMa261R_M7AFihzKnaU1Qjsox5JheBc7qIuPvPzw4OR3yh9tbnIAT-om11_QPT0up4Vwg5Z2ZT_dhAj76xHmYIHAY2DUuEbwJyzGdu2qV)

At this point, you can choose which lines or chunks of code you want to keep. It will highlight and show green checkmarks as shown above. You are able to keep both if you choose to (sometimes this is a safe practice because you can just delete the stuff that doesn't end up working) but it will create a close "duplicate" of the same code so be sure to clean it up later.

When you are finished with a file, click the green "save" button in the top right corner and continue with the other files. When you finish resolving all the merge conflicts, you want to click the green commit and merge button on the bottom right which will save all your merge conflicts and merge the two branches.