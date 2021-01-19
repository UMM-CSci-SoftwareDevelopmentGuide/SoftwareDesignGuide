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

# <a name="FAQ">FAQ's/Miscellaneous</a>

*   How is this class similar to Data Structures?

   Software Design builds off of concepts in Data Structures. You should have used Java/IntelliJ in Data Structures, and writing code for the server is also written in the same language. JUnit testing is also another thing you should have have at least been introduced to in Data Structures which you will practice more in this class

*   How much time do I need to dedicate to this class?

   Well, to put it bluntly, a lot. Every group put in dozens of sleepless nights into this class. It takes awhile to understand what each part does, and then putting it altogether in a short period of time is not easy for anyone. This will certainly be a class that will test your character, patience, and work ethic.

*   Yikes, everyone seems like they know what they're doing and I'm stuck. What should I do?

   The best thing you can do for yourself is to ask questions. Ask the professor, the TA, or other classmates. This is a learning experience. No book or text can help you more than actually playing with the code, thinking about how the moving parts work, and asking questions about what you don't know. There is not always a solid answer, but there could be insight into possible approaches. When you reach your second or third iteration, you will have become more of an expert about the code than the professor(s), because you have undoubtedly tangled with it more, and understand how it functions. We can assure you, your classmates are equally and or more confused as you are, so learn together and help each other. Remember everybody is stronger in some areas than others so while some classmates may seem ahead of the game there is almost certainly something unique you can bring to the team.

*   I accidentally forgot to do Ctrl+C in the terminal before I closed VS Code and now it says the session is locked

   We did this way too many times. Here is a potential fix that worked for us: <https://stackoverflow.com/questions/39091735/port-4200-is-already-in-use-when-running-the-ng-serve-command>

*   I can't find the error where my code is breaking

   This is the thing that will keep you up at night. Debugging is frustrating and annoying because the error could be as small as a missing a comma, a mis-named variable, or other minute overlooked pieces. 

   If the error responds with a line of code that is potentially the problem, it's worth going to that line and tracing backwards. This means going back through the chain of interactions that let you create that line of code. So if the line has a variable, go to that variable and see if it's defined. If the line uses a method, go to the method and see if it's written correctly. Hopefully, you can find and correct your error. If something appears to be incorrect with a method but you can not pin down what it is write a test! This will help you find the error as well as reinforce good habits for writing tested code.

   If you don't think you made a mistake by tracing backwards, maybe stop and ask, does the approach I'm using make sense or am I missing something? Is there an error or mistake in logic? If you're unsure, ask your professor or a classmate about your approach and see what their opinion of it is. (It is a strangely relieving feeling to hear, "Oh, your approach is on the right track, you just forgot to include these things").

   Oftentimes, it might just come down to having another pair of eyes looking at the code. This happens a lot more than you can imagine, so don't be frustrated because believe us when we say it happens to everyone.

*   How much CSS is enough?

   From our experience, CSS is important, but not crucial. What we mean is that CSS is necessary to make a professional looking web application. It can really compliment the user experience, but do not overdo it or spend great lengths of time on it. Try to find a suitable balance so it makes sense and presents a professional atmosphere, but not so much that it distracts the user from the application itself.

*   I feel overwhelmed right now and I don't know what to do

   First and foremost, know that it is ok. It's a common feeling. A good first step is to start with the small things. Take the time to really understand one or two ideas/concepts and how they work. Ask questions about what you don't understand. Once you start to see how the details function you can put together the bigger picture.

   We should also say, this is not a walk in the park kind of class. You will have to put time, and genuine effort into this class if you want to do ok, even more if you want to excel. Don't sit back and rely on your team, that is the worst thing you can do for your learning. Even if you just do a couple things, do them well, and seek to do more. Being proactive about accepting tasks and problems is a great way to learn the material and even if you do not succeed right away you can set up the framework in order for your team to assist you.

*   How Many Questions is Too Many Questions?

   If you are confused about a concept or a bug it is best to ask questions early and often. Don't be ashamed or scared, your question may benefit everyone. Banging your head against the wall until the situation is solved can be very time consuming and may not lead to the best solution. Asking questions early can save you time and allow you to move on to other tasks.

#### Remote programming

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

#### Conclusion

We do hope you found this guide helpful in some way, and that you continue to seek guidance if you have any questions.

Link to setting up dev environment on Windows:

<https://gist.github.com/floogulinc/2d9f80b278332b0df731e777c43b206c>

