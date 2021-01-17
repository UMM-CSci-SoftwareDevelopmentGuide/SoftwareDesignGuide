# Project Development

## Agile Development/ZenHub

Zenhub is a project management tool used to organize your project into epics, stories, and milestones. A milestone is essentially a major goal for the project that will include a start and end date. After a milestone will come epics. These are the pieces that will make up the meat of your project; most often these are features in your projects or significant pieces of labs. You could consider these as an umbrella of ideas, most often features that include smaller pieces regarding the functionality of the idea that include numerous smaller parts. Finally is the step of creating stories/issues, these are the smaller pieces mentioned earlier that make up an epic. Issues are what you assign to people in your group. While testing is not worthy of its own issue it is extremely important which will be mentioned later. This style of development will help you organize your project within your team and serve as an advanced checklist. The UI provides a visual representation of your work. This is done by first setting up the project and after some progress, tools like the burndown chart (shown below) can be useful to evaluate your progress towards completing your milestone. 

![](https://lh4.googleusercontent.com/15ys6f8_cm3Q3tRV-_N-_p5mXZk9TYBfcJT5VtC0QuH-ChQX2wdzqFOfnNPAr6-dq5QmeejmkF2diW0F04C3An2Et0C3p1XzSqD2ZFvbzBGQyKLGdWoDgetn2oizFfTiWFcOPNcA)

When you and your group begin a project, you will want to organize the tasks that you want to accomplish; in an iteration these will be features that you sell to your customer. When selling these features to the customer, you and your group need to consider the value of each feature and predict its difficulty. Once your team is on the same page about what tasks need to be accomplished, use Zenhub to create issues and assign these issues to group members. 

![](https://lh5.googleusercontent.com/DkFc7V_blGNUFTu7KFwm5H_fjJyHx5ghhzP4YtwBbZNUNA41iQ5wYaOf-XOu9rDVtLpc0FVpZZ2KzSTmbogQY8Vp-CA10I3li_Dm1iDm24q-NnKhKpOMOh1_s2wLVFuYp8kQGA31)

When looking at ZenHub you will notice each issue has a number associated with it. On your commit messages, you will want to include the issue number in the title of the commit in the format of  "Title #(number here)" for whatever issue you are working on. 

![](https://lh6.googleusercontent.com/StvYAW4juYETDjyDWs8ToDltHATx8226r1A1JJ4XYacKyodgTIdPhrS7WJxyikVYJYiYlmcgXEfeR9ljwcGeC9RKq_dSHxhiXfM_IU99CdvjlF3MTSK_gL2nJG2IFQjlB7rkkJQj)

When you close an issue this will update the burndown chart and other tracking tools on ZenHub showing progress on the project. You can also manually move the projects from in progress to the review or done sections in Zenhub.

![](https://lh3.googleusercontent.com/CFUs7alamdV02w-YOiu5DP3lKg53pc5TY9h2hTXv-vT_YrSEq9FAO8e7bkZL__6pge6iGj3_ep9d6kItXwK9eTisUtFDIM2QmpVN7Q2edUCHlqSeuYe7PYctC7nyao6k0bSnzeXQ)

![](https://lh4.googleusercontent.com/1zqQjrnlnL0m-Mj7HCe6S25HofSw1cPRB0c_iiNSkyt5M0XpaJAZQBaxMHDCOfGcqsd7SLtW-MWSX_j8WFoVwQQt_IsUzOfA4KGLqE2gtfgga34tgHzXzSCHNzzsvw0fCrGZ5Jg9)

This aspect of the class is more important than it may seem, being able to actively organize with your group and visualize your goal and progress is a key to success even beyond this class. This may feel trivial at times, but rest assured it is a good practice which encourages organization, consistency, and healthy communication.

## Continuous Integration

On GitHub, when you do have a red X (especially the main branch), you should focus your attention on fixing that as soon as you can. Your code should be production ready, and when there is broken code, it has to be addressed. Continuous integration is making constant commits, pull requests, pushes, etc. To make sure that when you do merge branches, there isn't an alarming amount of merge conflicts. Committing your changes often and with suitable clarity will help ensure that the small pieces do not break the functionality of the entire project.