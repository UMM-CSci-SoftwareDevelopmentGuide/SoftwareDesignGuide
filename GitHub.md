# GitHub

## The Main Branch

Every project has a main branch, this is what you should be submitting for labs and deploying for iterations. You should not be committing incomplete code to the main branch, whether it is a feature in a project or a lab. It is better to have solid code and comprehensive testing (even if it's not that much) rather than submitting partial code that is subpar and untested. On GitHub, you can view all previous changes on the main branch, as well as all other branches. You will most likely be using GitKraken, a tool used to make the process of commits, pushes, and merges more easily readable. After you push changes on GitKraken, you will be able to see the changes update on GitHub. When making a commit you should have all of the tests passing which will be annotated by a green check mark.

![](https://lh5.googleusercontent.com/ANqg8RlTwtMKql--Qf3RFpG0P2fkALOviS7XpIz1klaehvfkg2x8MO2yu3UXwXnLkiix0M4s3aU1WjYnLsoE7218imsW5_4JU-2RsHweylvjgl0KeoBAPOUdVOaJsCOsfXj__Ivs)

## Viewing Changes

Like the main branch, you can choose to view the changes that are on a different branch by toggling the branch button. 

![](https://lh5.googleusercontent.com/-lF2xGiFwdJqI-qHDTDVPR-a44kx3mHK-amdDxMBXCr4Y2Y3r1xUh5rndk5BO5Tbmu3eo3mhhW3yOhBKHcRGlZWPMv2VshoO0fPfpaVidwv2aYiIm17yJ5Vc4ptktQ8ODgSoiZaA)

The files on GitHub reflect the same files that are being committed to the branch, so you can see the code that a file has. This is especially helpful if you want to view the code base that another team has.

![](https://lh6.googleusercontent.com/sENdwk8YIFFkAWk8KLhLUkc_hGl8wWssRjU_FxqKSjVhzwxnrb5IRMD_kiTxjxV6UsGAbLBEmE4HaJteIWZ5-2_CkMJlY7eclGlYKeEzdGjXBCx9Nb6XalPYCJrn9ClR6Dw7duUq)

## Git Blame

In relation to the last point, Git Blame can be another useful tool at your disposal. This allows you to see who has made commits in relation to changes in the code. This can be particularly useful when joining a new team and repo, allowing you to track down who wrote a particular piece of code in order to ask any clarifying questions.

This is not a tool to copy and paste another group's code during a lab or project. It is important to understand the code you are writing and how it functions. If another group has solved an issue you are stuck on, it is recommended you communicate with that person to understand how their logic can fit into your code. Similar to researching solutions online (Stackoverflow, etc.), a block of code that works for someone else does not necessarily mean it will work for you; but the idea could be tweaked in a way that would benefit you.

The easiest way to view the git blame record is through GitKraken. After selecting a commit you will see the changed files on the bottom right panel. Click the file you would like to view the changes of and you will get the differential view displaying new changes highlighted in green and the old code in red. Above this you will see a button labeled "blame". Here you will be able to examine the file line-by-line, see when modifications were made as well who the author is.

![](https://lh6.googleusercontent.com/Jz9wa822v2ypoo6fY_MhY7vxHGG0fe1r5y91dNIGqNhOUHN0RArt7v6fUlGUOCfVgkKtmDin4VmR3_1FUeTf_aNW9JQtjjA6vfof4SREJeE91iXf6YZTu4NQLwWSpUDSvIvO3c5b)

![](https://lh6.googleusercontent.com/QXz681_196YezEcSEGK_yW1qpAddBgMjQhh345mhVlzcAGq29J3XMhYGaWUutuoVKWLSO55A8dkzhzrwlscZldsiAyQfOb28OXPkY3I6ILHJyRC5ynfP0uvqRVvl7pZfLbWIF_XP)

## The Green Check and the Red X

On GitHub, you can see a green check or a red X on whatever branch you have selected in the upper right corner of the files. If there is a red "X" that means at least one test in your code does not pass. This could be an E2E test, a spec test, or a server test. Occasionally, GitHub can experience issues and say you have a failing test when you know you don't have any! If this happens, simply re-run the tests through GitHub by clicking the red X and selecting to re-run the workload.

![](https://lh4.googleusercontent.com/VMnIW6ixp-WZOk6XRzsmIL1x2ER280m9671cf5kIf3Y2pLRqMqwqBgWi7SmkA7PZW8YL2TSkY5S_eueToJMkWZfCZn1jW6xBp0dS6RZiDG-QxeLC86v_-cMp5GATE2vzSIKH1B6F)

A green check mark signals that all your tests are passing. 

![](https://lh3.googleusercontent.com/1CTR52VjKuH93yG3mjdACRhKZTLi7tz88RKrv2rXQgapaFTV2V_xwSV_ZTOG7vTrVWZlO7kDiPxg50BvUw6XFMhRl3zTR05iW6cHh4QR34Dj4idVT7ci6AyvQX463H8DRyu44acV)

Tests should reflect what you want the code to do. It is important to write code in a test driven development (TDD) sense for this reason. We have found that when a test fails, it is most often not the test itself that is incorrect but the logic of the code. This means your logic or how your code speaks to each other is incorrect somewhere. Failing tests will also suggest lines in your code where potential errors occur. 

Another possibility is a yellow circle, which would appear instead of the green check or the red X. Don't panic! This just means GitHub is in the middle of checking to see if your tests pass or not. Within about five minutes it will turn to either a red x or a green checkmark.
