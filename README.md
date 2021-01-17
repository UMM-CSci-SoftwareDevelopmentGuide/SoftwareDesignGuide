# SoftwareDesignGuide

## University of Minnesota Morris - Software Development Guide

## Created by: Chineng Vang and Jack Perala

Here is a (hopefully) helpful guide for what we have learned in our time in the Software Development course at the University of Minnesota Morris.

### DISCLAIMER:

Everything in this guide is to our knowledge. They are all ideas and concepts we have worked with and would like to give guidance on. There are certainly more areas to explore and it is encouraged that you expand your knowledge beyond this document. 

It is always advisable to ask a professor, a TA, a trusted peer, or another classmate about confusions or other approaches to a problem. As you work with the code and your projects, you will develop a better understanding of the material but it is important to ask questions to better supplement your learning.

In no way is this a substitute for lecture. A non-trivial portion of your education will come from not only attending lectures but also working alongside your classmates. Communication and sharing ideas will be key to not only problem solving but expanding your knowledge as a whole.

Remember to ask your professor if any confusions arise. It is a healthy practice to seek solutions from a variety of sources, when your peers (or even professor(s)) are unable to assist with your inquiries. Be proactive, be the pursuer of your own solutions, but seek advice if you encounter a roadblock. 

Again, this is simply a guide to understand the common topics of the course and an introduction to the programming challenges you will encounter.

### Introduction

At the beginning of the course, it is common to feel like you are overwhelmed whether it is because a lot of new ideas are being thrown at you, or your classmates may seem more educated in the subject. Do not be discouraged, we all felt that way at some point. Keep an open mind and make sure to pay attention. While you may not be proficient at everything in the beginning, building on what you do understand and actively learning about what you don't will be valuable for you in this course. It is important to realize that nobody will know everything, especially in the beginning or even towards the end, never be afraid to ask questions. As you go further into the class, you and your classmates will be more familiar with whatever project you are working on, so be willing to consult your classmates.

### Table of Contents

|

[GitHub](#github-anchor)

-   The Main Branch

-   Viewing Changes

-   Git Blame

-   The Green Check and the Red X

-   About Pull Requests

-   Setting up Reviews for Pull Requests

-   Creating Pull Requests

-   Testing

-   Agile Development/ZenHub

-   Continuous Integration

 |

[Angular/VS Code](https://docs.google.com/document/d/1-tO3_0tYb5kTzgTHj-ZXLNdYdJXD9q1SHvVX2zJupdM/edit#bookmark=id.wlutxe36xvfl)

-   How to Open a Project

-   How Angular Works

-   The Client-Server-Database Model

-   App.module

-   Running the Server and Running the Client

-   All About Components

-   Component.html

-   Component.ts

-   Component.spec.ts

-   Mock Testing

-   Component.scss

-   Creating an Object

-   Services

-   Server Side Files

-   Controller

-   Controller specs

-   Database

-   About Databases

-   Seeding the Database

-   E2E Testing

-   VS Live Share

 |
|

[Git/GitKraken](https://docs.google.com/document/d/1-tO3_0tYb5kTzgTHj-ZXLNdYdJXD9q1SHvVX2zJupdM/edit#bookmark=id.pywuj576v6c1)

-   About Git and GitKraken

-   Creating a New Project

-   How to Make a New Branch

-   Committing a Change

-   Pushing

-   Pulling

-   How to Merge Branches

-   Merge Conflicts

 |

[FAQ's/Miscellaneous](https://docs.google.com/document/d/1-tO3_0tYb5kTzgTHj-ZXLNdYdJXD9q1SHvVX2zJupdM/edit#bookmark=kix.3n9vwdmzh1vk)

-   FAQ's

-   Remote programming

-   A list of common terminal commands

Github(#github-anchor)

The Main Branch

Every project has a main branch, this is what you should be submitting for labs and deploying for iterations. You should not be committing incomplete code to the main branch, whether it is a feature in a project or a lab. It is better to have solid code and comprehensive testing (even if it's not that much) rather than submitting partial code that is subpar and untested. On GitHub, you can view all previous changes on the main branch, as well as all other branches. You will most likely be using GitKraken, a tool used to make the process of commits, pushes, and merges more easily readable. After you push changes on GitKraken, you will be able to see the changes update on GitHub. When making a commit you should have all of the tests passing which will be annotated by a green check mark.

![](https://lh6.googleusercontent.com/Uh5WwgtoEBT9ALbP1aY82xG0M0uXF39KFqBz8HSxOWhN8tC90R5-IVN24HKp31bVue60a9nq0tQbBrjnjluXIVIm4U3J9VlfvpinGZrtjHfVUV2Tu5W0R8UEjOgry_eu_GhuVtR5)

Viewing Changes

Like the main branch, you can choose to view the changes that are on a different branch by toggling the branch button. 

![](https://lh6.googleusercontent.com/LDyjBEGBC-aUcy6-kO3s2h0LjWnTGWDWexFHpZ2gqgENd4Sj426i85gxQXBoPOBKYql7WeBsjRu0i_6ZNLrUBWoeqbiHRK9TunNnK_EA2bHEpsrS-ez7GhP9K7jGt-W491pgSdfC)

The files on GitHub reflect the same files that are being committed to the branch, so you can see the code that a file has. This is especially helpful if you want to view the code base that another team has.

![](https://lh5.googleusercontent.com/0SVXZAAfAvnyQh5A5EkLl8dQlM8csJkuSFvqAwUuYpm6FjceakNU7vgy3w-nNdUR09feXEENTOfLZPToICQrldfT0_Y7_wqrlCLJbUXMfOea7Ca0HslpMc5egGFry2veF8akH9bb)

Git Blame

In relation to the last point, Git Blame can be another useful tool at your disposal. This allows you to see who has made commits in relation to changes in the code. It is particularly useful if another group has found a solution to a problem or found a more efficient/accurate way of implementing a feature or idea. 

This is not a tool to copy and paste another group's code during a lab or project. It is important to understand the code you are writing and how it functions. If another group has solved an issue you are stuck on, it is recommended you communicate with that person to understand how their logic can fit into your code. Similar to researching solutions online (Stackoverflow, etc.), a block of code that works for someone does not mean it will work for you; but the idea could be tweaked in a way that would benefit you.

The easiest way to view the git blame record is through GitKraken. After selecting a commit you will see the changed files on the bottom right panel. Click the file you would like to view the changes of and you will get the differential view displaying new changes highlighted in green and the old code in red. Above this you will see a button labeled "blame". Here you will be able to examine the file line-by-line, see when modifications were made as well who the author is.

![](https://lh3.googleusercontent.com/myGrDzQ78i5ClRuhbIdEtvKSiysB4i1-n26nxQmuXEyXoVDpVIaOU_d8ZQ8IlceUB5Zx-bu7ohSuoJc55OZRfVI6V_H1inGzASQgizaALvIXkUQErQWJ0_aR1yBWotUNSsI6BhNy)

![](https://lh3.googleusercontent.com/SvgYjIxJFN4nmjPsGQvRekQDJj99FVA5PubWZMfOtnFxSW2l0as5RswGBmRT6esZgalAjqA3astfUtXP7l_x7YqT92IFvZrm1vyGxpty49awA1BcupWhP7ILCfrWwIIZFHkplryT)

The Green Check and the Red X

On GitHub, you can see a green check or a red X on whatever branch you have selected in the upper right corner of the files. If there is a red "X" that means at least one test in your code does not pass. This could be an E2E test, a spec test, or a server test. Occasionally, GitHub can experience issues and say you have a failing test when you know you don't have any! If this happens, simply re-run the tests through GitHub by clicking the red X and selecting to re-run the workload.

![](https://lh3.googleusercontent.com/6bamSK9WKcQl_k0Fb8LJI5QYzlJJd1UqKUnk1je4tt_YCFERwXntq8Mij1aC22tsERTChF9PqVDLRU92jwOTDxXFo-RkerPsODYV0ikaxeoWgQbwbUUltrr7xG5aklfpwGpVnctR)

A green check mark signals that all your tests are passing. 

![](https://lh4.googleusercontent.com/_W89CJJJu4OA_8m6s2SQ_yk9urziRbrCgp3DV2z2A7eBlxvYbFbGG0EDOHLYJm8d9zkkOo6PQBbn9ziOXTHKj8QZb7XEOyuClbpsoyMd-MXeoNFxvOMBsLqtFJp76Wt2nIVtIiUd)

Tests should reflect what you want the code to do. It is important to write code in a test driven development (TDD) sense for this reason. We have found that when a test fails, it is most often not the test itself that is incorrect but the logic of the code. This means your logic or how your code speaks to each other is incorrect somewhere. Failing tests will also suggest lines in your code where potential errors occur. 

Another possibility is a yellow circle, which would appear instead of the

green check and red X. Don't panic! This just means GitHub is in the middle of checking to see if your tests pass or not. Within about five minutes it will turn to either a red x or a green checkmark.

About Pull Requests

<https://www.youtube.com/watch?v=e3bjQX9jIBk>

When creating a project, especially once your experience with a customer begins, you will be encouraged to personalize some settings on Github that will be discussed by your team. Pull requests are a useful method of making sure nothing unacceptable is being implemented. In your team settings you can set up a parameter for requiring a certain number of approvals in order to merge in a branch. Here is a link to a video with a quick explanation of pull requests: <https://www.youtube.com/watch?v=e3bjQX9jIBk>.

Pull requests are basically someone in your group merging one branch into another branch on GitHub. Here the person merging the branches can leave comments about what they changed or ask questions to the other people in the group through the comments section. Then someone else in the group can confirm the merge or add more comments to the request (sort of like discussing if it is ok to merge or not and ask clarifying questions). 

![](https://lh3.googleusercontent.com/Ew8FWr4avbPKxHdohldW0YvTl0Ir3Dl-FilUKt7JLKIB0eTHcwOxLvU98zJJr_Fn9pNEV8XDaAR1mr4ina7UbigfQXnOs6L-YP6dhMtSLYegJ2loSvuDAQZqBFwqcCDXs58aBjML)

In the above picture, it is highlighted where you can access pull requests in GitHub. 

In our experience, we have upheld strong communication and if not one but two, or three, other group members were fully up to date before ever reading the pull request. While it is not required, it is strongly recommended to leave a comment on why a pull request was rejected. Communication is key, and with a small group it is certainly achievable.

Setting Up Reviews for Pull Requests

![](https://lh3.googleusercontent.com/3u7YlN-dlk2CTZWkdKGPAdZFPltNgxvkIkQCQJUjGISlbslxggAk19r-qI5up7mhJL4uZVodoKpViR05h7spzZJb-RB6JJPfNsWBFuqc0834iLDPHy0m3-8s_lnQYUoxUvEjEt-L)

To set up pull requests for your groups first navigate to the desired repository on GitHub and locate the settings button on the far right side of the top bar, once you are in the settings screen you will want to click on the branches button located in the sidebar on the left side. From here you will want to click "add rule" which will bring you to the branch protection rule page.

![](https://lh6.googleusercontent.com/PnirT_1xRnSI5hGW0ZWJ497RyHVBlR9BFEcGwp9puzgguPyeiSBeXoWj33xU9hjgdNPsAdFZB88bl_4ZVi3PkplcQehJL-qdiKAi-7sKZMgRWd4AD21mNfvXYW7FKZt6OepDszu1)

Now that you have reached the branch protection rule page you will want to name the branch pattern and select the "Require pull request reviews before merging" checkbox. Typically we have set the required approvals to one or two people because there will be times when the whole group is not able to meet at the same time. There are a handful of other options that could prove useful but setting up reviews for merge requests is what we found to be the most useful.

Creating a Pull Request

   To create a pull request, navigate to the pull requests section in the top bar on your GitHub repository and click the green "New pull request" button located on the right side of the page.

![](https://lh3.googleusercontent.com/xcdzMw6inNWf67-RWvNrTen70gXishbSCsTYiiec5MnE_VmZP3GkITuIZV__2TVipnwOFnimAi70scILc50B89zV7Oz518g5WwUqN_4pBoGZnLxREtolu6ItXb5PPpa4wCeo00p5)

After accessing the pull request page, you will need to select the branch that will be merged into another branch, you will most likely be merging into the main branch (previously known as the master branch). Then click the green "Create pull request" button. 

![](https://lh3.googleusercontent.com/9u4p_N8rFNZAM0xbtjUqYJg7kWpZfczCTSaqLItxwiJ84iAn6wA3a0XVU2ekPRh_E0GSmPALjYQyGPwtKzBRKGERe9RxAMAsUiPZlS7cxTjjI33_8jPk-abV7OZ_SjKoAoOvzJ-q)

On the lower sections of the page you will be able to view commits that have been made to the branch as well as what code has been changed, this is denoted by a green highlighted section in the code. Once the pull request is created group members of your repository will be able to view the request and leave comments or approve the merge. 

![](https://lh5.googleusercontent.com/Hj-vh6JjzTApPeZQvyTg5sY1GkJOTRuK2JhTiYNGbeYAwNgVihig6a9jw9vUNM10rP_nTzplGO8O34ZV-s4iGt_3OrLl_Brgrw8LZrxFL6Nlz_hiycLnTCf_kq0oRqel7lsbYORe)

![](https://lh6.googleusercontent.com/KFIV6_JoBojNMHlInFzc4u1ieFgpApiPsZXPbeJ_VhqX1it9_O0oKMt_X3M1iAbWZNsVtW5ZKooEtr_3K0TVjBOEbXeNNOiXLcOZW5MtQj47f6iNmBoJARBDmc9JMnyCShhmcZ5w)

Testing

We've previously mentioned tests and testing, but here we'll go more in depth about what it is and how it works. When you write a block of code, you want to make sure it functions how you want it to. Writing a test for that code is a way to check that. We go into this with more in detail in the Angular section, this is just a brief overview.

There are different types of testing such as end to end (E2E), JUnit tests in Java, Angular testing, etc (for testing on a specific file, you'll want to reference the All About Components section). In general, a block of code will need some data to process. When you write a test for that code, you will be providing that input data along with a conditional statement about what the outcome of the test should be.

![](https://lh5.googleusercontent.com/C5tYkkLrwwzCaJoNuO6ylTzsP8qNKhhwgYlV1YtBCkjD9O_6aMqqmWME4vpQ8oIAAzyKLmeraNnKrE30otiMdlq3ztJ8yft05gkiqfFVajz1dk4h8DC6h21KElp2-5drZDn5q7Ex)

Agile Development/ZenHub

Zenhub is a project management tool used to organize your project into epics, stories, and milestones. A milestone is essentially a major goal for the project that will include a start and end date. After a milestone will come epics. These are the pieces that will make up the meat of your project; most often these are features in your projects or significant pieces of labs. You could consider these as an umbrella of ideas, most often features that include smaller pieces regarding the functionality of the idea that include numerous smaller parts. Finally is the step of creating stories/issues, these are the smaller pieces mentioned earlier that make up an epic. Issues are what you assign to people in your group. While testing is not worthy of its own issue it is extremely important which will be mentioned later. This style of development will help you organize your project within your team and serve as an advanced checklist. The UI provides a visual representation of your work. This is done by first setting up the project and after some progress, tools like the burndown chart (shown below) can be useful to evaluate your progress towards completing your milestone. 

![](https://lh5.googleusercontent.com/UYsYwMEeGlXEjHiPEtsgOMZrYv2So90EjHYYVibC4hCGWXy8Efbxah7zrFsmBfBqdMFpb5eyP_kE_l0OoHJqM1MMExzmNWqRuoMrdPndXgbYxrVAAe4p7pIyDn6l9Id6tk4I41DG)

When you and your group begin a project, you will want to organize the tasks that you want to accomplish; in an iteration these will be features that you sell to your customer. When selling these features to the customer, you and your group need to consider the value of each feature and predict its difficulty. Once your team is on the same page about what tasks need to be accomplished, use Zenhub to create issues and assign these issues to group members. 

![](https://lh4.googleusercontent.com/51SuTzjbejSzWFVzI-ectUZLZHrdgerphYq3j7xzh5Jnl58XXYDr8aVwLFDt4CEOSAVcbkQd27MzsO3AsYd4V4qkfQEeEa1CgWZ2xXUYt2lzXLp_SVG2HUzAY2VzKmQ8SYWMqAzm)

When looking at ZenHub you will notice each issue has a number associated with it. On your commit messages, you will want to include the issue number in the title of the commit in the format of  "Title #(number here)" for whatever issue you are working on. 

![](https://lh3.googleusercontent.com/UNpHeURdhb3zINdlvaJ6WBvpxMhUhqrhWCgUI8Dw1S6a9PAFZKKrW0vRWIKI73gyBRxcQLo0UAlG-qrP5-b_3n89oWmLfVVkyCQb4TExyTmPtmcS34yYDx_3f0KXLbyHBHe3ONw8)

When you close an issue this will update the burndown chart and other tracking tools on ZenHub showing progress on the project. You can also manually move the projects from in progress to the review or done sections in Zenhub.

![](https://lh4.googleusercontent.com/Fv_EMuR3t-wS9ZS-blyJ2zPUKZK7h7AeQxNxryvX1AB1Ap2ngyMpsiLuOkVBomfkfrpq3X0_fdhYysMB97nfQG-OqzJ_4ry9YY2wZogBWMlk-8wKONggnYzvDxMpEGOu5olmVqdn)

![](https://lh4.googleusercontent.com/rmO8NfLazK2tO3GMVm2AmquTYlm8ycA6a-hwJBicr-krm4j-4RFgPwRZwrv74tFV1kI9Yh9JoONO0D8Y2nAoeThclcIW7q3EmlF4qwqW6g8wpGa8LaFV4TcVAQeZQ5n4cwX1DYdF)

This aspect of the class is more important than it may seem, being able to actively organize with your group and visualize your goal and progress is a key to success even beyond this class. This may feel trivial at times, but rest assured it is a good practice which encourages organization, consistency, and healthy communication.

Continuous Integration

On GitHub, when you do have a red X (especially the main branch), you should focus your attention on fixing that as soon as you can. Your code should be production ready, and when there is broken code, it has to be addressed. Continuous integration is making constant commits, pull requests, pushes, etc. To make sure that when you do merge branches, there isn't an alarming amount of merge conflicts. You're basically ensuring that the small pieces do not break the functionality of the entire project.

Git/GitKraken

About Git and GitKraken

According to Wikipedia, Git is a distributed version-control system for tracking changes in source code during software development. It is designed for coordinating work among programmers, but it can be used to track changes in any set of files. 

GitKraken is a GUI (graphical user interface) that provides a visual representation of the repository. Here you can see commits that members of the repository have made as well as their commit messages. GitKraken also has commonly used features such as push, pull, branch, pop, stash, etc.

Creating a new project (Method A)

Firstly, what we like to do is create a folder for the new project or iteration. Make sure you know how to navigate to it through your computer's file explorer.

![](https://lh5.googleusercontent.com/nEAUw9BC9jBvINp9zzMCWYdeOSR2zbR_UWjbHldty1vY8EeD_qDXCC14KUys1VkB8x9S6skVo21z5ZZaE5AvN9-ap0oih0_3TW0C4HgZK-XYY-_ZcURCiLISyuEM0fdXCX58mHWs) 

For each project and lab, you will get a repository in GitHub. On the project's main screen (usually the one with the main branch) you will want to click the green button that says "Clone or Download." Then copy the link by either clicking the button (as shown in the picture below) or using Control+C.

![](https://lh3.googleusercontent.com/TRWoMWxPRI3MYSL7Cxlok4dUqA24D0cojGIKPtkLvZIDfuK2v-xKWR_BcgFP-9gZ5rSxIXNJl_7FAVfp1caFtPiWel6AhtCxqw7LZY1Hb1BslvFjYAWF6HOHePuOxupG1n1DCxHB)

(Screenshot below) Now open GitKraken. Click "File", then "Clone Repo." You should get a screen titled "Repository Management." Under "Clone" and "Clone with URL", you should see the Clone a Repo screen. Where it says "Where to clone to" browse to the folder that you created for the project. This folder will hold all the files for the project. And where it asks for a URL, paste the URL from the repo on GitHub that you copied earlier. Once you've completed that, click "Clone the repo!" and it'll clone the repository and open the project.

![](https://lh4.googleusercontent.com/oRBCOo8BbskwZee7p3vxEk32NYDJCqTLloNKv3x8GkUfSps01Dxei9tm7GC9W5JtSuTCCfc9UxIJHRcmpP-uDI2IsGMQ7sZGXki9qvNa1pADWM91FnOYEnlvYk4pPyhY4QQgHL90)

If you need to open the project or another project, go to "File" and click "Open repo", then select the folder that has the project you're looking for. You can do this in BOTH GitKraken and VS Code.

Creating a new project (Method B)

Make sure you and your group have your repository in GitHub set up. And also have a directory for your project to go to. Now go straight to GitKraken. Choose "File" then "Clone Repo." Select "GitHub.com" and choose your group's repository and the directory where you would like to save the repository to on your machine.

How to make a new branch

When you make a new branch, what you are doing is making a copy of the branch you're branching off from. You could think about it as parent and child branches. For example, if I want to make a new feature off the parent branch, the new branch (child branch) will be an exact copy of the parent branch. You can make new changes to the child branch and save changes without altering the original parent branch. When you are finished with changes on the child branch, you can then merge the child branch, back into the parent branch or another branch of your choosing. Now the selected branch will contain the approved changes of the child branch along with what it originally had.

![](https://lh6.googleusercontent.com/y3VqhYDrYDs782g-u_F-jp1WMSXNK4tWsG8b_Y8eSv6GRp1yaa3G7n41dICv3ypdoePS_0Md7AdFClLxRLRsjbPN_yBqq13caZ8P3rJpMESDFqofr-dWjpOgGOykxRHBvaKopBEe)

When you merge a new branch into the original branch, there may be code that overlaps. So you might have different code in the same file (i.e. line 37 of app.component.ts has different code). This is called a merge conflict and is covered in a later section

To make a new branch, go to your project in GitKraken. Find the branch that you want to branch off of (the branch you want to make a copy of). Then click the "branch" button in GitKraken and give the new branch a name.

![](https://lh3.googleusercontent.com/KEA3WunxYJcAJ6qPRt0-LbJ5ux_gqyt3sY3lMUwRRgYQNp18-0WqphLkjCVNhHzoJwWTkZSGppiAjwpj-_mzd54qzj1ojh_VfwPvG1t8F03jxEYxlLeWoq2cL5eExrxT2vJSSW7N)

After you enter the name of the new branch, you should see a new branch in the GitKraken interface that sticks out of the original branch which illustrates that you are in a different branch. When you open VS Code, you'll now be in that new branch which you can check by looking in the bottom left corner.

![](https://lh3.googleusercontent.com/M6H1p7MRt8eQg_I7FNeqSI2zqFj8NkDEe4kMdOxR8TYQDUZJlcTTIp74qgXr45Q6qj2VqpigbgX2aBawK_RVLuct7-QXx_phFOpIHlp6tadLfctNmB7c2ro071wn9UX_c059dMVe)

![](https://lh4.googleusercontent.com/1nw0b54yxgLsL0f3IEd8IKChGnWf838Lxe_fzNwIymp7Mh5dHhVR4t-bxEIo5mqduj2kE8c3hzlc_FGmAJ6SvHeGrC8KY3JyMndWeqf65R9tx7XtFI-gCgCvY5HqJAF5oPPF0ded)

When naming the branch use standard good naming practices to avoid confusion. An example of a bad name would be: "My_branch#$7" and a good example would be something more descriptive such as "doorBoard-list".

Committing a Change

When you alter code and want to save the changes, you will have to commit your changes. Make sure that you are committing to the right branch, which you can see on the left hand side. The easiest (and most visual) way to do this, is to use GitKraken

![](https://lh6.googleusercontent.com/jjidqqmrsuEkQQ0VDJg_owGOqvk9W3rScpj9lEdDiwKElfdYdrIiUyxd5V23UR87HrLIemcd_igrjWeynMxXNc7SGbvaTODTKDiOn5A7NDOmNW-QUlMpNANjW-DLwOnlzoKr-Sk7)

As the picture above shows, the file(s) that you want to save changes on will appear in the top right column. You need to hit the button "Stage File" so it appears in the box below.

![](https://lh5.googleusercontent.com/GaFUVJUVlfqEOx1FlwknnQ1TWx-6gPv4JXo6n-IFXBCK94ajy6w-yYgysoqDI_f8V7pMd8mUirmNJbfLIRVS8ApGwI0G6rjzyDxhf4E9rpX8MqaEy6G947TEYBAwwwYQkmN4JoWo)

The commit message you attach to your change should be brief, but descriptive. The title for the commit is like the header of an email and should be able to tell someone what the change consists of in as few words as possible. Clicking on a file lets you view the changes that you made.

![](https://lh3.googleusercontent.com/hHTps--RKNc_QaM3IJH0rgysXka6_phQkwVX-3ZJC2AgEsKXaeyrXoAAwaKj0vK241luDwd7wDJSXHBD8abDJnlrv7jK6bW7juxQcvMrhv2o91vIghz98gzX6C5h1YoDhlcVgu_y)

It is a good practice to commit often (especially if you make a lot of changes) to help avoid major bugs. When you make a commit, these changes are only saved locally; only you can see the change, until you push to GitHub, which leads into the next section.

Pushing

When pushing, you are sending the recent commits to the working repository (which you can see in GitHub). This will allow other members of the repository to view changes in the branch and pull the code to their local environment. 

Multiple people can work on one branch at the same time. When you work on a branch, you are working on a local version of it. That means, the changes you make (before pushing) are only visible to you. So when working with a partner or group remotely it is important to communicate when you solve an issue so it can be pushed and everyone has access to the same working code.

![](https://lh3.googleusercontent.com/OLaDE8vAKOa2h3SDEzyyBQyYEeyM-LmmpHY9adscKOxyN3GCVys8k-ExroywZeeSMdNIlu9d25OJ4juMItH3yjgS8GX1Bt9XWBJ69bSwm1lYgdR08V47QwvWn_9JpJs4v5Blc7VT)

You must pull all new changes from a branch before pushing your own changes. To push, after making all your commits, hit the "push" button on GitKraken. If it works, you'll get a blue popup that says pushed successfully. If there are changes to pull, there will be a red box that prompts you to pull first. And if a push fails, you'll get a red push failed prompt.

![](https://lh3.googleusercontent.com/qDiYO7Vj0XkA6rG2wzQOLvK13zG-C2S8NJ6ZOQp3780S_mVCdqDScdY8ZbfAJeULVGchk346Wo5KD0ZpE9IIVp5sEblCnU82DTld6cH-6MB5AVzdZaXa9hunmQ2O3Ho_tgbWa0CZ)

Pulling

After pushing the changes other members of the repository will be able to pull the code to their local environment. When you pull changes for a branch, you are grabbing the changes to the branch and pulling it to your local project.

![](https://lh6.googleusercontent.com/_wVX92j7YBL6b_L4b-_ZKR1ea1DpXzZsUgtuAzsDGXoPMhlM4MXsp58l2LZB4VT5MKBPtzk4TL3IQzZp1lyv3LNgeKECpjssL-9xSlqcx4o1v2cByLAfyPPQIW7jPKCIZcaBYEn1)

To summarize, pushing changes makes your changes to a branch available for members of the repository to see (usually your group and professors). Pulling brings those available changes to your local project.

How to Merge Branches

Any changes you make to a branch will need to be merged into either the main branch or a working branch for the changes to be utilized. For deployment all of the approved changes will eventually need to be merged into the main branch itself. 

In order to merge branches the easiest way to approach the problem is through GitKraken. Let's say you want to merge branch B into branch A. Simply click and drag branch B on top of branch A and click the "Merge branch B into branch A" option.

![](https://lh5.googleusercontent.com/sCo5h4Gz-Pgfh_hs7zEEE6crHFJfC90ffEn4BYrJHr89Br3W97eFCg_FWg5KraIsvAOXs5oosmBbif5IJZEeZbWoBwuOqmjdWD-8CLZIrN9uXuM1XDcLr2oYN0TLBmxPnfQSbfdN)

![](https://lh5.googleusercontent.com/NCpYrjjidFHxugAsTQEtIa2uF31JoKKB6NPaSS_yKCk7VqeDVQYlcGw1ZwFYbjrwiYPizeA2pltqruIAMP_MphWLGjChOfeDDWQG04j1DGWPPsrzYYbfaTFfFovG_3EtnYctrC_0)

Now the changes you made on branch B will transfer over to branch A (assuming there are no merge conflicts which is the next topic). 

Merge Conflicts

When merging 2 branches, you will often run into a merge conflict due to overlapping code, a line of code in one file may have different things on another branch. When you merge, you will often get a yellow prompt notifying there is a merge conflict.

![](https://lh4.googleusercontent.com/EITZOtqS6IrKvqXLO6sNdymLMSc3A8WZ3Ygq9FYlQZw1uvBXj0LImV_8vQcHvqt751RW92kf8dV1UiolALd8tjk1lBINr9UbY9KNtMjW_STlckiRRAfPUHQQNZVFzZ8WjSFTqKuz)

When you come across this, you must choose which code to keep, which ones to delete, or if you would like to keep both sets of code. In GitKraken, it will show the files that have merge conflicts on the right. Click on one of these files. You should get an A and B split screen as shown below

![](https://lh6.googleusercontent.com/33OLMU_UGaSs4iAU38yzRdyV7l8MBr2wtn3BlqC_okF2SS3n-FS5BLbJ80Fah6aKAZknSvyWtv0X4cNvT7YIg_mbBY5jaiMAEg8dZhTZN2GpwVv7ya8WQPksr_XD83FAtYXPZ0zx)

At this point, you can choose which lines or chunks of code you want to keep. It will highlight and show green checkmarks as shown above. You are able to keep both if you choose to (sometimes this is a safe practice because you can just delete the stuff that doesn't end up working) but it will create a close "duplicate" of the same code so be sure to clean it up later.

When you are finished with a file, click the green "save" button in the top right corner and continue with the other files. When you finish resolving all the merge conflicts, you want to click the green commit and merge button on the bottom right which will save all your merge conflicts and merge the two branches.

Angular/VS Code

How to Open a Project

When you open VS Code, it automatically opens the most recent project you were working on, which is convenient most of the time. Other times you will want to open a different project or start a new one. In VS Code, you will want to go to "File" and click on "Open Folder." Then you can choose the project that you want open in VS Code. 

![](https://lh4.googleusercontent.com/ayWFvABWEYAv2PaLJSz2mVEavvAROmjn1gnxgSMvT7JGaSPbJByn-jU3GOFgT8lP9TwWt6TweGoalCtJh1fmvl2RsPUpszjd_73kIU1ZOnaCSowAtKh2pTsZhNF9nefcZUsz20H7)

After you've worked on more projects, going to "Open Recent" will let you choose a previous project that you've worked on instead of manually clicking through "Open Folder."

How Angular Works

Angular is a command line interface used to work with Angular applications and develop web applications.

To begin, when you first start working on your web application, anything that first appears is part of your app.module. We explain in a later section, but the app.module is like the foundation of your project and you can alter the app.module files to immediately see any changes (you should see this in your Angular lab). 

![](https://lh3.googleusercontent.com/qFekQ6PxDDek1X1_GLUpajXCPhP9k1V1VTVZm0yujAtL1R_tK_cQcPdhxxhAh2jBecw09-uXvwDyYmGFU2ZkhcnQxsErUeyXSCLUY0YieKnLMW1JRtdWCbNie6kxjqbQiZ-J_a6F)

![](https://lh5.googleusercontent.com/RhpCA-b2UtNKLKY474ukFDlzY1WZw2AlJ0LQnTbI96dznVPntZgRE_0D30CREG-rGzHseeTe3uG9l8qEVd2uOWJyW7_mRhWvMmfacmR_gffeAQDtJPtkQsgY8dpiEUi6eH2BXk54)

If you want to add a feature to your application like a button or a search bar, you will add a component. Components, like the app.module, add information to your web application. 

The Client-Server-Database Model

This is a topic that is emphasized in lecture and we would recommend asking the professor(s) more about it if you have questions. 

A good explanation can be made using a bank analogy. Let's say someone walks up to a bank teller and wants to take out money. The customer gives the teller their information and the teller retrieves the money from the vault. In this scenario, the customer is like the client, the teller is like the server and the bank vault is like the database. When the client is accessing a webpage, it gives the server information about what it wants to access. The server then goes to the database to request that it returns the desired information/data. The server uses the information provided to filter the database search and returns the desired information to the client.

-   To recap: 

-   Client - User clicking around on a webpage

-   Server - Webpage taking information, making requests to the server and returning the information requested by the user

-   Database - Housing of information/data which is accessed by the server

![](https://lh4.googleusercontent.com/Q2id9wUfX4hQVJzntIMYwO4FBCoYdmJBIFS5RLRxEZ1dW6CZdrj_SmDqXfj6VPhhhLQBg7qpvjzjg-uWrwo1Nc1GfNQ4lUhTtMGhF-zYYnVDnQqmYrmX-qnWg4-V9nNFEYWObeoo)

App.module

App.module is like the foundation of a web application, think of it as the brain of the project. What you are able to do in Angular is create components. A component is like a feature on a web page, an example would be the search bar on YouTube. Components are extra things that can be added to a web page to make it more useful. When we go over the app.module.ts file, you will see that each component you make must be imported and declared.

![](https://lh3.googleusercontent.com/z7tPlip3ggXDNRZI1cYN7nsgwBIbJEDyoUHelbKo6fmnqf8o8B5ZSYcWqhoDiZjGFmBcSu2M5cvpLk_dYl2F11uFF2IJruWjl4zD7nSHeGwbTKT_zM6Z7eu3_NVTWqhmPd8FhV-q)

App.module consists of 6 files:

-   App-routing.module.ts

-   If you are adding a component that requires the user to access another page other than the main application page (which you will eventually have to do) you need to define that path here. The home page itself has a url, so a new page will need a new url/path, which you define here (It's more useful if you create the component first in the component.ts file to avoid naming errors).

![](https://lh3.googleusercontent.com/DsYDIHYWZQ6Wlh2dEhaL2IbHuc71U2HTLpyQ_iqUd0QNnOYz1teHQr6MkyRxBxUc_AfIhP1_K5YT3W8KeLz7ozX7YXnFHOjn7Zayfesly7Gu8X0bX6M2_UYC7cD0LdeEMUW-PTek)

-   App.component.html

-   This is the file that controls what text and images, go on the specified page of your web application. It also has a variety of other features that you can explore such as adding a toggle button.

-   HTML is a markup language used to create web pages for display in web browsers. It is the code for creating web pages, using tags and other commands that a browser reads and converts into the readable web pages that people see.

![](https://lh6.googleusercontent.com/PZFHyhnh1BbnZe9uFm564rd8ST9h0QYttqbqBW2hxJ3A-lfZPAM5lC24K98Ksk2wNHDISbI5NJeciQZ7Fnpn-23Ka3E8xYQrKVClLLd5TjJPoDENL97lsdnJkNRwrmIVU92-y7Im)

-   App.component.scss

-   This file controls the CSS for the html which allows visual customization for certain aspects of the web page, such as changing the color of buttons.

-   App.component.spec.ts

-   This file tests the methods in the app.component.ts file.

-   The file utilizes the methods like toBeTrue(), toBeFalse(), toBeTruthy() and toBeFalsy(). They are what they seem, they are methods used to check if the provided input is true or false.

![](https://lh4.googleusercontent.com/L0-0NbUeWpvLnKPChUg_vmswl0SzFGUL5maI9_yBcVHiyVazOmrz6vngvQhrIC-zx9Q8ovOB1tDHJTKTiZCTmyOEQzrr-3PKEG0Hb1kzAqfUlDLWiv_Hx9Cs7NP_-ON9BU4iDgWt)

-   App.component.ts

-   This file (along with all other component.ts files) are very important. Here, you can create methods that move data/information, which essentially controls the functionality of the component. Each file on the client side is written in TypeScript which is a language with its own syntax. The files for the server are written in Java which you should have some familiarity with and will be noted by ".java" in the file name.

![](https://lh4.googleusercontent.com/ZTZLKobk9hLMomijKM7ZtzREaB9V4Fx_Ixs9r3C-RAulxIt50EM77n4-XQdSw7Bxuj9g3teQQNLGt66Z_zDbr1f28INDUcbswOHHb4ZHwgY8vt5JF2WqbIgQCT-mAbUetK8OX8-w)

-   App.module.ts

-   In this file, you must import and declare each component or it will not work. It is small, but it is necessary for the files to communicate and function.

![](https://lh3.googleusercontent.com/0bdyKvPu6je6AINewfMfvPv5AnJIhrHno2AYwIdguqNRUN9Qwi5rBA1xt5EiGMZ8sHLdQpWXhpWj9EPgq7wl2hF2Oe40F6XhUtZR0v3iv9vHU9KDXOGGVAQa7mmyhvYNoi8kOyKU)

![](https://lh6.googleusercontent.com/YUKCD4zLnaJQkGGFLLXBhvHdFJAONkluure--kKs0h5UWba_ZXVwvdPR74b0MR8TasAftLKBBxDTr7SS5eqXgKZC336nfs6qhB0ziYfr9-Ir-NEyiSX9eqm5uyZv1ElMNPHX2DE9)

Running the Server and Running the Client

You are going to want to see what your application looks like while you work on it so you can view any changes being made.

-   To run the server: 

-   cd server (If the server is already running this command will not work and say the local host is already running, this also applies if you have the server running in another terminal window).

-   ./gradlew run

-   To run the client:

-   cd client (This only applies if you aren't in the client)

-   ng serve

![](https://lh4.googleusercontent.com/LBGwSbDbbW6vh-lzTF_Ax-9CMHbN8VvgWjLonqjy-W7ezorZ4PnyuitP4e4xGmEYkO2PaQuXDMzxbzSOpL6V2tc9ofgZLiMcnII9-ec_v14mbeBHjS7uSnUvfxKR88EufUAutAZz)

Then go to localhost:4200 (your application may experience bugs when using different web browsers, typically Google Chrome has worked the best at first) and it will show you your web application in a new web page.

IMPORTANT:  When you want to close VS Code and you have run the client and server, you must hit Control+C in the terminal for both the client and server. This shuts down the client and server so it doesn't lock you out the next time you try to access it. There are fixes for this issue if you do forget to use Control+C, but hopefully you can avoid that.

All about Components

-   Component.html

Files that end with component.html provide the text for a component, such as what words will go on a button (log-in, etc.). It is possible to change the characteristics of the text like making a word bold or choosing a font but this is usually best handled with CSS.

If a user is providing an email, you can make something like "User's email: (insert here)." Different users will have different emails, but the first part will remain the same. This isn't restricted to just email, any information that the users provide can be displayed if you write the right methods.

![](https://lh3.googleusercontent.com/V3ip2MI5w1C_FCJ0FpuY8tNZeWJ2o5R_i8B72TgwQOa3pd8PgRvbLZnZut97MRb5ykxitCgYWCM_EAZklM9-7JWpBW-i-9diZDH8ssCXZccfI31bnkH7FSOCWkpR8U0rhkjzm9pz)

-   This file is also where you can add buttons on a webpage. What happens with these buttons are defined in the component.ts file. These buttons (when clicked) can bring the user to another page, so you're able to add a link to this file as a button.

![](https://lh3.googleusercontent.com/QqN5rTbHMmZj_59Muev4VotOSuJeKC7nsQVx-37VNEkw8Q9RZdJJKmq98rJXumXnJndl9xoL6yu1XZQcFd2JXzm5IWEj902tfGB2sAefB5RlNFapKCu-RIujrNWKuOEC5ZjPdFLN)

-   Component.ts

-   This is the TypeScript file for a component and where the methods for a component are written. As mentioned before, this is where you also define variables which are crucial, because a lot of bugs will most likely result from a variable not being defined or being utilized incorrectly.

-   This TypeScript file is similar to a class, where it's methods are defined, and you can utilize them in other places with the defined variables. This is also where variables are initialized in the ngOnInit method. Those variables could be undefined with ngOnDestroy.

-   Here's what you usually find in this file:

-   Importing the necessary routes, services, etc.

-   A constructor (usually declaring the imports)

-   An @Component and export class (Component)

-   Variables (defined as string, boolean, etc.)

-   ngOnInit and ngOnDestroy

-   submitForm (optional)

![](https://lh5.googleusercontent.com/vgIkMT8GKl8NIGspwqwLc0jz7J6GGUgRQw8HsGsWxN_RAEsjQydkPgyGhwtW-knbjkxH1dr2y1DvwD8uunVQSAtSzv1xzwt-N09fG1EKUZkxVBvsX8ycY4Q_UqpAkOP1GHZ3ib-u)

![](https://lh6.googleusercontent.com/XYHsItuxINcmdizLlao29bqADjceyWchdMFw9JhGtDJbCA4RJ_85xY6fw3Nk1iv5-OXmS1Tj2o3l-A41RHf6vCeh045RPLx1brK-imH4QKMa4M-JgvF0OvOHSjibZexd2LyeHa4r)

![](https://lh4.googleusercontent.com/F6eh88ktrESglz0osjCehyspfbYpXn-drWYoJqluX5FlezbLFRHkaMIekuKDKj3zSXe9j0E5i5Ui1pIDXZofmPfx0Qq-mGPzR_24KagMQjLinWRuqzgrcC26GSfS2Z5WNCe2Hizq)

![](https://lh3.googleusercontent.com/oqFFLPrq1jACKVp0i8JfSxUw4oTylCNlSQ04dxPo1eDKkXBuL1_WXi0exPHcXPWDhQzhVfy6H_SVxK6k76DhimXfuSNwJzeD1Xra0ob2F3INSSaXu7Oc-2wx0Sw-olg30kZQjwTY)

-   Component.spec.ts

-   This file is used to test the methods that are written in the component.ts file. It checks to make sure that the methods are behaving how you want them to. Because the tests are local (within VS Code) they can't actually reflect your web application. So we utilize mock testing to test our methods with "fake" data that we create. 

-   Mock Testing

-   Testing a component is an important part of this class and the functionality of the project (it also helps with debugging). Mock testing data is in the (nameHere).service.mock.ts file. In the component.spec.ts file, after all the imports, there is a describe method that defines the imports.

-   There is also a beforeEach method that does something before testing a method. If a beforeEach method has "async" then whatever is defined in the beforeEach will happen asynchronously from the other tests.

-   The tests start with an "it" statement telling what the method should do or what it should output. Commonly seen are toBeTruthy() and toBeFalsy() which say if something should be true or false. equals() is also another common statement in a test. 

-   As mentioned before, each test looks at the file (name).service.mock.ts. This is where all the "fake" data is defined and what the tests refer to. This file is like a "fake" database of information that you are testing.

![](https://lh3.googleusercontent.com/j-DP0j7KPMDI05aoDDdruDtpCWol_iww5fqUcRVK7eYPTiJxhJ64HxDKGu-ENPGbq1cPN69ZuQNQEZwVHeNLzLhVjm_v2QtEWGW7j9GMLNJ6rsJMA-x3q5EnT5ut7tHtU7PtRo61)

![](https://lh4.googleusercontent.com/65RTJfv-1_H0efJENh5xOxAsrVqpRBKMSde1bcKMnJyveoXSZaU6NQHd7Iof3i6lAHDdKvWG_IwX6Ovjvf1XfyH4C1yz_1uiRx9TJ--g3_mzFGcJBZm8EZ_uDOmf83j5JQWiqtYg)

-   Component.scss

-   This is the CSS file for a component. It styles the text along with the pieces of the component itself. You can add color, borders, background images, dropdown menus, etc. This website has a lot of CSS stuff that you can quickly apply: <https://www.w3schools.com/css/css_border.asp>. 

-   CSS is an overlooked facet of a web application. (This will allow you to give your application a professional setting and look for the user). If something looks clean and professional, it's bound to do well, and it gives a sense of confidence. Avoid going over the top with it and ending up with a cluttered UI, but there are enough options to make your web application stand out.

-   Creating an Object

-   A TypeScript file (not attached to a single component) can be used to define an object. So if you want to create an object that resembled an email, you would declare that the object "email" has a date, body/message, subject line, sent from, and sent to fields. The name for this file would then be "email.ts" So any component that utilizes this object (by importing it) can access any of the fields. 

-   Each field has a type. Some common ones are string, boolean, etc. You also have the ability to make user defined types.

-   Try to think of this file as multiple people agreeing to speak in the same language. 

![](https://lh6.googleusercontent.com/uDx6I4Ectt5WT_UpD9p1MVyA5Sj879FY2ZNxkXzJxIcyN41UCntwmRO2UQvjyXxAE_2h47qgVI64pLT30aWYoMvXt3MDzq-9je5qg7ciIakDFIVeRAgFA-XgehSYT3NaryBsBCRZ)

-   Services

-   Services will be an important part of your web application. A service file has a bunch of methods that can be utilized by any component. Unlike a service file, TypeScript files for a component are specifically for that component. 

-   Components that use services, have to share the same information. For example, if two different component files utilize a service, and that service has the variable "note", then "note" is defined the same in both files. To declare that a component is using a service, you need to import it. 

![](https://lh3.googleusercontent.com/lKrRKI_mwL9hhCs0WIUnOWe_pb6GiNnIVPj35n3EabbbdhkZo5OTTN2wPIA9zvCUq_dyYPPen15DPmuFSPX2avXBmCV0X5ogVu8McH3baMlCOYWZZA4lZI77w5tgZ5_N1DJTe63s)

-   Spec files for components also need to import services so it can be tested for a component.

-   Services also have spec files to test the methods. NOTE: Inside of these spec files, you create the data that you want the service to test.

![](https://lh3.googleusercontent.com/mgdqrIzyvgfZ7_EgocHmAO0rJA700RTbGIeSH5WbIiqm9ZGhJbsfCDNjgTLPNyvqzRILThGEVS9egy8dJpQek8OrauNiUUZ8hWTTqBoYuaQfj8bcAQuGiODmnuE5PxuQCb-BadRx)

Server Side Files

-   Controller

-   Remember that the server is a way for a user to access specific information from a database. So this controller file has methods that access and change information in a database.

-   The controller also has a .java file which is similar to an object file like "email.ts" on the client side. It's where an object/variable is defined and it can be utilized in the methods. 

![](https://lh5.googleusercontent.com/jcoGLiUu06fZ_lsjPeBepysUj7_KlQQKlsw-BL4WBPPqUzngEOoWXav1jdfhPeO7FK96MI0B-ZqCmh-fJde5MDXKWMGcqhyBCETcYTJlxn27-z2ySqzZIDOIfLAOfAPi-SAAWmV5)

-   After the .java file comes the Controller file, which is written in Java. As mentioned earlier, this file has methods that work within the parameters you set in the .java file. It "talks" to the database and can retrieve or change information in the database.

-   If you have taken Data Structures, you will notice the syntax is a little more complicated, but is still familiar enough that it's understandable.

![](https://lh4.googleusercontent.com/Nmk5XKogqwpiseUId43y7YN6sbVsJqAVlI2X5JdPnvGyzXrrp82YNaZ-aPrliEnYIVyjkrNoowZpSAa_OCUEOfyMU17LlJQ8-W3L411YerZVAifZ3gqyAm_cZVuPqxmI4Nwgz1oM)

-   Controller specs

-   The Controller also needs to be tested so you know the server is doing what you want it to. You will configure these tests by writing JUnit tests. 

-   Like in the client, this test file also has @BeforeEach to declare what is instantiated before each test.

-   The data that you test is also something you define at the beginning of this file. You're essentially creating a mock database.When you add an object to a database, it must have the same fields as it does in the .java file. So our email object would require the fields body/message, subject, etc.

![](https://lh4.googleusercontent.com/aYfTprPaNJGVW3hVYQGAtjLrApozzwt8hhZCnuJu2MgflnGGqz2cmBOZuO498JseRl_oUi3MU00apZKmEko1y39wWLx7Pfyezb9a2l0acCCsYuko5573SRPE3DqvftQFCYCVoAJo)

-   Each test should have an @Test to declare it's a test. It will also provide a "Run Test | Debug Test" option. Clicking Run Test will either give you a check mark or an X (failure). NOTE: Just because a test passes, does not always mean it does what you want.

-   At times a failing test can be the result of how the test itself is written but most likely it is an issue with the method. Being able to read why a test is failing, and possibly which line is causing the error, is a necessary skill in order to debug your code.

![](https://lh3.googleusercontent.com/ba8yngm7cujAG2R48rRVvsgyGbDiqrK2STphth_HzfS6e9DYs5Mv-jbrA6eqOhV6vsXTAqPvFHOatnv545qevUQUuz3fFtMe37jq1VqvAmJtHM3M3WnwaWeM9tviUxDLdgmmLUQJ)

-   JUnit testing can be tricky and the syntax can cause headaches at times, so this is a topic we would suggest you ask your professor(s) about if you need further clarification.

Databases 

-   About Databases

-   Remember that a database works as a bank of information/data. You are able to add, remove, or alter these entries in the database.

-   For this class we used Mongo as our database. When you are working on your iterations/labs, you are able to add sample information to your database with a JSON file. To add sufficient amounts of sample data easily, you can use a JSON generator which can be found online. We have found [Mockaroo.com](https://www.mockaroo.com/) to be the easiest to work with as the fields are easily customizable and there is a straightforward link to download the document.

-   To view a database in VS Code, you need to download the Azure extension. From there you should click "Attached Database Accounts." From here you can see what is in a database.

![](https://lh5.googleusercontent.com/KLcWU5vCfHO_fkak2llYWslBNotYjMyTxfsJz_gzn8C8wYumNCOvrMa0pKGY3GlQHu36pypiNxV4bgKL1PxGGaXWU77-gwctf49_94OnFIUXhamuwcl38a14jm_YhHXgdKT16bLQ)

![](https://lh3.googleusercontent.com/45f4XwGw9koJCECIGdnu89-vRaf_eHoPu7s8GDtAdFr05BLXNjTF4hjmggxBw1E9Cc1ejMgKPryo4VA3fxuYQXGYB6DdCLnP_6WmoeQHhUVmoyhvyQEQmSPDNG0bSqEvNqM_A6Qy)

-   Seeding the database

-   Seeding the database takes an existing JSON file and adds that to a database. Seeding the database will grab all of the current JSON data in VS Code and add it into the database.

-   To seed a database, you need to first cd into the database file. So open a new terminal and the command is cd database. Then ./mongoseed.bat seeds the database.

E2E testing

E2E (End to End) testing tests the connection between the client and the server. It tests whether or not your client to server interaction works and does what you want it to do such as adding an entry to a field or deleting an object.

The E2E files are in their own folder called e2e. 

![](https://lh6.googleusercontent.com/gKZQUdW1LQKOpiHAX8eQqLl9D0I3nPD_QMdZHoM4vvaUoWhPNfi5PzPN4OjRKV3k17mNbXkLIwkgeulZwfmLDsBoQakED7Ea5o_LWgDJiqp503VzQZQ2uy-BIf_f9Vz7NvyqpFKi)

Like the components in the client, there is a .ts file and spec.ts file. You're basically writing more spec tests (like you did for components) but it doesn't test a certain component, but rather the entire application's functionality, the goal is to write tests that will replicate user scenarios.

![](https://lh5.googleusercontent.com/bZFrIvh6lZouLSoXixRtE0JjcKgWbjB7b_7OOEctPFztpJVMwszpZbFqYc0dBYAdAjU6y-DRYNXRJe5E2-HPV8QvfYQKqvJOIstvFb0MBDt1GEpmAd3LpLtSRcGm5JMz-IDnjXdK)

![](https://lh5.googleusercontent.com/a3lGtWWQg3aV7NUDcWwae-nfG7x3DjyxMLe8tv4xYvZod7RBDgHUiWKKPJhtp0i3K_nWbhmEercmIlLbDrdxfBn4ddweDE5WJvMNzfhFJyIrPXgYEDORIRr79ulz0J87wjroJQY-)

VS Live Share

VS Live Share is an extension on VS Code that allows you to pair program with other people. It is similar to Google Drive where multiple people can work on the same code at the same time but in this case one person is hosting the session so they will be responsible for running the client, server, and tests as well as handling commits and pushes.

This is an ideal tool if you have to work remotely, because you and your group can see in real time what is being changed. This also allows you to have an extra set of eyes to look over code which can be very helpful for finding small bugs.

To use it, you first need to download the extension along with the Live Share Whiteboard extension. When you first start or join a collaboration session, you will have to login into GitHub. Then you should have code to share with other people who can join the session

![](https://lh5.googleusercontent.com/h2GXVl4-i5Rp1bq0PKGQlycv3mRZtbJoFqcafMyF0beZ6cKd6WI7LUbnpe53zMC5-rMQam8QjcoPbdnk0X6S8-TNN_hGU0OHw9golB34jfV9DucsK4_BdLbF6UT2wPB1lFHAGQSl)

FAQ's/Miscellaneous

-   How is this class similar to Data Structures?

-   Software Design builds off of concepts in Data Structures. You should have used Java/IntelliJ in Data Structures, and writing code for the server is also written in the same language. JUnit testing is also another thing you should have have at least been introduced to in Data Structures which you will practice more in this class

-   How much time do I need to dedicate to this class?

-   Well, to put it bluntly, a lot. Every group put in dozens of sleepless nights into this class. It takes awhile to understand what each part does, and then putting it altogether in a short period of time is not easy for anyone. This will certainly be a class that will test your character, patience, and work ethic.

-   Yikes, everyone seems like they know what they're doing and I'm stuck. What should I do?

-   The best thing you can do for yourself is to ask questions. Ask the professor, the TA, or other classmates. This is a learning experience. No book or text can help you more than actually playing with the code, thinking about how the moving parts work, and asking questions about what you don't know. There is not always a solid answer, but there could be insight into possible approaches. When you reach your second or third iteration, you will have become more of an expert about the code than the professor(s), because you have undoubtedly tangled with it more, and understand how it functions. We can assure you, your classmates are equally and or more confused as you are, so learn together and help each other. Remember everybody is stronger in some areas than others so while some classmates may seem ahead of the game there is almost certainly something unique you can bring to the team.

-   I accidentally forgot to do Ctrl+C in the terminal before I closed VS Code and now it says the session is locked

-   We did this way too many times. Here is a potential fix that worked for us: <https://stackoverflow.com/questions/39091735/port-4200-is-already-in-use-when-running-the-ng-serve-command>

-   I can't find the error where my code is breaking

-   This is the thing that will keep you up at night. Debugging is frustrating and annoying because the error could be as small as a missing a comma, a mis-named variable, or other minute overlooked pieces. 

-   If the error responds with a line of code that is potentially the problem, it's worth going to that line and tracing backwards. This means going back through the chain of interactions that let you create that line of code. So if the line has a variable, go to that variable and see if it's defined. If the line uses a method, go to the method and see if it's written correctly. Hopefully, you can find and correct your error. If something appears to be incorrect with a method but you can not pin down what it is write a test! This will help you find the error as well as reinforce good habits for writing tested code.

-   If you don't think you made a mistake by tracing backwards, maybe stop and ask, does the approach I'm using make sense or am I missing something? Is there an error or mistake in logic? If you're unsure, ask your professor or a classmate about your approach and see what their opinion of it is. (It is a strangely relieving feeling to hear, "Oh, your approach is on the right track, you just forgot to include these things").

-   Oftentimes, it might just come down to having another pair of eyes looking at the code. This happens a lot more than you can imagine, so don't be frustrated because believe us when we say it happens to everyone.

-   How much CSS is enough?

-   From our experience, CSS is important, but not crucial. What we mean is that CSS is necessary to make a professional looking web application. It can really compliment the user experience, but do not overdo it or spend great lengths of time on it. Find a balance, do enough to where it makes sense, but not too much that it distracts the user from your actual web application.

-   I feel overwhelmed right now and I don't know what to do

-   First and foremost, know that it is ok. It's a common feeling. A good first step is to start with the small things. Take the time to really understand one or two ideas/concepts and how they work. Ask questions about what you don't understand. Once you start to see how the details function you can put together the bigger picture.

-   We should also say, this is not a walk in the park kind of class. You will have to put time, and genuine effort into this class if you want to do ok, even more if you want to excel. Don't sit back and rely on your team, that is the worst thing you can do for your learning. Even if you just do a couple things, do them well, and seek to do more. Being proactive about accepting tasks and problems is a great way to learn the material and even if you do not succeed right away you can set up the framework in order for your team to assist you.

-   How Many Questions is Too Many Questions?

-   If you are confused about a concept or a bug it is best to ask questions early and often. Don't be ashamed or scared, your question may benefit everyone. Banging your head against the wall until the situation is solved can be very time consuming and may not lead to the best solution. Asking questions early can save you time and allow you to move on to other tasks.

Remote programming

Unfortunately, we took this class during the COVID-19 pandemic, and the entire class had to program remotely. Although it was tough at first, we managed to adapt and still put together a solid project. If you also find yourself in a position where you program remotely (which is a realistic expectation after college), the CSCI faculty have guides to download the software necessary to program like you do in the lab (of course each guide is specific to the laptop/computer you have).

Here are the tools we utilized to program remotely:

-   Zoom - For online face to face meetings and programming sessions.

-   Zoom Whiteboard - Zoom has a whiteboard feature that we used constantly to draw out our ideas.

-   VS Live Share - To interact with the code synchronously.

-   Slack - To communicate with your team, classmates, and professors.

-   GitKraken - Provides a visual environment for repository.

-   GitHub - A repository hosting service used for pull requests, and eventually ZenHub.

-   ZenHub - An Agile project management tool which can be implemented into GitHub. This gives a visual workspace for your project allowing for planning and tools such as burndown charts.

It is almost always better to program in person when you can, but it is not out of the picture to program remotely and has its place in working effectively.

A List of Common Terminal Commands (note that "→" stands for followed by, an example being firstCommand → secondCommand)

-   cd (used to change current directory)

-   ls (lists files and directories)

-   cd client → npm install (need to do at beginning of every project)

-   cd client → ng serve (runs the client)

-   cd client → npm run e2e (runs an e2e test)

-   cd client → ng test (runs all the client spec tests)

-   cd server → ./gradlew run (runs the server)

-   cd server → ./gradlew test (runs all the server tests)

-   cd database → ./mongoseed.bat (seeds the database)

-   CTRL+C (shuts down the client or server depending on which one you're in)

-   git clone (insert repo link here) (clones a GitHub repo to your local machine)

-   git pull (pulls the latest changes of the main branch to your local machine, will require login information)

-   git push (allows you to choose and push your changes to a branch on GitHub, will require login information

Conclusion

We do hope you found this guide helpful in some way, and that you continue to seek guidance if you have any questions.

Link to setting up dev environment on Windows:

<https://gist.github.com/floogulinc/2d9f80b278332b0df731e777c43b206c>

