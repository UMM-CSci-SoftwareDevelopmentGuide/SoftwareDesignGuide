# Angular/VS Code

## How to Open a Project

When you open VS Code, it automatically opens the most recent project you were working on, which is convenient most of the time. Other times you will want to open a different project or start a new one. In VS Code, you will want to go to "File" and click on "Open Folder." Then you can choose the project that you want open in VS Code. 

![](https://lh3.googleusercontent.com/LrLPXsI5-_BpwWdads7qUaUWjt3NHh9clXYuKNbqERI3OgonCDPaO9HmY6YiRAd0lc9XFZET_UkcbIjCzvgzuQn-YOYXBXv_8fDlbQBh-un5MNbepdps_MciY_BWzxrtg2TFKsLh)

After you've worked on more projects, going to "Open Recent" will let you choose a previous project that you've worked on instead of manually clicking through "Open Folder."

## How Angular Works

Angular is a command line interface used to work with Angular applications and develop web applications.

To begin, when you first start working on your web application, anything that first appears is part of your app.module. We explain in a later section, but the app.module is like the foundation of your project and you can alter the app.module files to immediately see any changes (you should see this in your Angular lab). 

![](https://lh5.googleusercontent.com/X8kchv5ZM8a9kZyn8XAIV-5-4qO_5TSKwfjQTVwDaCEVxtDlw7LMEC9FVn0Eh5U5t3l1mGhOUja1M0_dGIG0Jpef71GW9iBfd7Pt9pqFeBT8-ftnnDX-slMPWhF_hCgzDg-U3Y1H)

![](https://lh4.googleusercontent.com/H2BypGIxPFXrsKZoQeYiipa9oMwbnXKXpqzYYtuRYWkeyomDUSOijk-vWk0PfyT4raAvXhwqtVNycgUWEg6mAIt9-VYPq5L70pg_-NULF8OEByvaznMmrIkfXx2XN3UuhyZbgxXG)

If you want to add a feature to your application like a button or a search bar, you will add a component. Components, like the app.module, add information to your web application. 

## The Client-Server-Database Model

This is a topic that is emphasized in lecture and we would recommend asking the professor(s) more about it if you have questions. 

A good explanation can be made using a bank analogy. Let's say someone walks up to a bank teller and wants to take out money. The customer gives the teller their information and the teller retrieves the money from the vault. In this scenario, the customer is like the client, the teller is like the server and the bank vault is like the database. When the client is accessing a webpage, it gives the server information about what it wants to access. The server then goes to the database to request that it returns the desired information/data. The server uses the information provided to filter the database search and returns the desired information to the client.

-   To recap: 

-   Client - User clicking around on a webpage

-   Server - Webpage taking information, making requests to the server and returning the information requested by the user

-   Database - Housing of information/data which is accessed by the server

![](https://lh6.googleusercontent.com/RL9ko2Vfx5VBMY-S7GA4ciJY68p6nIsD_2NPC3nNxJ1GP1o2o_UESZlGUXwEXsASUYzzgUFRwiCCfzr69c51y_t8ws4upNdqM1RCDUcf1CBAT_ez6ewRI8kqlfNCYLTri3jc6lxa)

App.module

App.module is like the foundation of a web application, think of it as the brain of the project. What you are able to do in Angular is create components. A component is like a feature on a web page, an example would be the search bar on YouTube. Components are extra things that can be added to a web page to make it more useful. When we go over the app.module.ts file, you will see that each component you make must be imported and declared.

![](https://lh3.googleusercontent.com/9yTKGujyXgNG_K2e28kCcIdJ5kkBfqTq1x34qDJ9Bl8j-8bnGRQTicPFvH7K0s57oEEXwZYN1Ydq2jWfS3C2rpwmfAz_UBOl55jKeKQ_MJyfkSZ8Z9tSbHwLXuRD6PLl5JW-zdSb)

App.module consists of 6 files:

* App-routing.module.ts

  If you are adding a component that requires the user to access another page other than the main application page (which you will eventually have to do) you need to define that path here. The home page itself has a url, so a new page will need a new url/path, which you define here (It's more useful if you create the component first in the component.ts file to avoid naming errors).

![](https://lh3.googleusercontent.com/7ANOTWFz44NhBqGwZpr7hDWH7MCPyshcw9DmpctmYhL7MUonaco2CibRYrR3ACwPkncX-AnlAmC-5dODCJZOmNm172KkJytvpplbhx8J7FSs5BatZQc190k9Oe3069kQKxLWGnoU)

* App.component.html

  This is the file that controls what text and images, go on the specified page of your web application. It also has a variety of other features that you can explore such as adding a toggle button.

  HTML is a markup language used to create web pages for display in web browsers. It is the code for creating web pages, using tags and other commands that a browser reads and converts into the readable web pages that people see.

![](https://lh3.googleusercontent.com/d1QSg56rPXx6yXoq_SAAznrMecF8IgQZVFwifcApq_7fyDdlaApv7Qsjg93oLGMxGuJPHb-n7LuGd9htcjnKQHGUu31DnS59PHlnyHPRTt6_o2Sk2YgZuPRoZt1U3gpzsL8tQAbP)

* App.component.scss

  This file controls the CSS for the html which allows visual customization for certain aspects of the web page, such as changing the color of buttons.

* App.component.spec.ts

  This file tests the methods in the app.component.ts file.

  The file utilizes the methods like toBeTrue(), toBeFalse(), toBeTruthy() and toBeFalsy(). They are what they seem, they are methods used to check if the provided input is true or false.

![](https://lh3.googleusercontent.com/lyPNzehUi30hX9bnGkCU_7Ziykx_hWXyGUvP-k15xLuJwBdNttpcB3q4KVM3bfPEcicAhq72vQOgZEirLaEAHQPlGf7uf_vSZEvGXXGga1gUpWysPM-YOFU11CUQ-la5ZykVXgmq)

* App.component.ts

  This file (along with all other component.ts files) are very important. Here, you can create methods that move data/information, which essentially controls the functionality of the component. Each file on the client side is written in TypeScript which is a language with its own syntax. The files for the server are written in Java which you should have some familiarity with and will be noted by ".java" in the file name.

![](https://lh5.googleusercontent.com/vbcMZgvjtpkRqwqYZczc62bonpCCS-_CczRJ4FQH0GkJ7VtK62iT8eii-fzzcr7hTMe9jCi8qqWuQw7YCfSgLAjg7hv0I-tNj6c-whEKSLJ4LoObmRF8JhxFl9BziNZajRziY05Q)

* App.module.ts

  In this file, you must import and declare each component or it will not work. It is small, but it is necessary for the files to communicate and function.

![](https://lh3.googleusercontent.com/LqimFB8R_nC9267ueSuO110di9CrbU59XLD3TuBCJJxzccqARWtNeSTUzsmuGQB50DKz7cUKlJtQN-2Ar5OE__0mgMmcu7Axy5BGqRohrvlFcUrJ44cB24iyWluipuRFpfE2aS-B)

![](https://lh6.googleusercontent.com/kXWCg-pqa6auv0lCRVxe6rwKGeUr-oD3HLAj08o9MYoh5Czc5Yb9dlpCn-a7-IUv3jyn1T9-O1Fa7ll7jk6u5LzNnkI2i9P8DQriCL3CXnCP5L9nH1eWX1BIe91DBnpwu817l1Uq)

## Running the Server and Running the Client

You are going to want to see what your application looks like while you work on it so you can view any changes being made.

* To run the server: 

  * cd server (If the server is already running this command will not work and say the local host is already running, this also applies if you have the server running in another terminal window).

  * ./gradlew run

  * To run the client:

  * cd client (This only applies if you aren't in the client)

  * ng serve

![](https://lh5.googleusercontent.com/adCh2QvLBnO4Kx5jbNVM1ftUt76Zsd24OWX3FtgtOPqQROxLi_Q8n-MiMWSOoNiQA76_giH_XiNH2n35ATfXe-WgjKDP0iSVC3Z_uBEeNEYedGrQagBoNQ0zVpdHmMEDF8ChKACP)

Then go to localhost:4200 (your application may experience bugs when using different web browsers, typically Google Chrome has worked the best at first) and it will show you your web application in a new web page.

**IMPORTANT**:  When you want to close VS Code and you have run the client and server, you must hit Control+C in the terminal for both the client and server. This shuts down the client and server so it doesn't lock you out the next time you try to access it. There are fixes for this issue if you do forget to use Control+C, but hopefully you can avoid that.

## All about Components

* Component.html

    Files that end with component.html provide the text for a component, such as what words will go on a button (log-in, etc.). It is possible to change the characteristics of the text like making a word bold or choosing a font but this is usually best handled with CSS.

    If a user is providing an email, you can make something like "User's email: (insert here)." Different users will have different emails, but the first part will remain the same. This isn't restricted to just email, any information that the users provide can be displayed if you write the right methods.

![](https://lh5.googleusercontent.com/k2jI9w3WAmbQQG5cCji9GzgJmBDAYQdPdZSYKSUTL1Xpnju1O5-oFCpZDiyneZzMLMdxKvSzSm4lBvXn72vL2q4rpUh-uePK3xeYJc2v-lzOLoaLlorbhSkLySjeVHz8apG_hoFq)

  This file is also where you can add buttons on a webpage. What happens with these buttons are defined in the component.ts file. These buttons (when clicked) can bring the user to another page, so you're able to add a link to this file as a button.

![](https://lh3.googleusercontent.com/vBVSHO3iR8d-YMhoqFFg9Wuqw_S8EBOlZnWz0IwuXR1bQdZ18iDa9-lT7egJhdKscl2cxkopPaRCXTVZRtbMxMeTUNFjufdoEwMnBungTwaSJSWa6kd4Tyb4rW32kyPq_lvuXQ-8)

* Component.ts

  This is the TypeScript file for a component and where the methods for a component are written. As mentioned before, this is where you also define variables which are crucial, because a lot of bugs will most likely result from a variable not being defined or being utilized incorrectly.

  This TypeScript file is similar to a class, where it's methods are defined, and you can utilize them in other places with the defined variables. This is also where variables are initialized in the ngOnInit method. Those variables could be undefined with ngOnDestroy.

  Here's what you usually find in this file:

    * Importing the necessary routes, services, etc.

    * A constructor (usually declaring the imports)

    * An @Component and export class (Component)

    * Variables (defined as string, boolean, etc.)

    * ngOnInit and ngOnDestroy

    * submitForm (optional)

![](https://lh5.googleusercontent.com/T8XIZIg2fZyqK4OzsckoqK5N5DtlzCtEwjvSTh83xoHfQr1pVU53S8dsxcs13A-HOR0x2iX1HhAdIuwXsmthCSXYCYhI3Nfm55WHJp4o9vLM_LBT1gD2St36INrbEIQxW0qH-uM_)

![](https://lh3.googleusercontent.com/YfQZJe4mc4SyDuijxy5PZdlhZGyem7gtxm9VhpSo2d9hzMmnX70-Wu4rMQ_JM9mQhoBrxtqZjqpE_KFbj4sUhtvoDiVsBm6ZwiSpq3KeXYZcl-dBG73paKnbJ9LV_MuQeHgKSN4P)

![](https://lh4.googleusercontent.com/BCkYkpiB4zgoUy7vixtEA7jC_kfLArQQ05p806xNuByiROgggEmqc7DQc87AEoA5AVin_jfdxqqO05zFE4437rpFUA1fb4HeiH283kxL9rkYQj3nr_j8_FcMLALT79NH1Uhfneiv)

![](https://lh5.googleusercontent.com/48Hnrz8kIvJi8OzJDLoWR7AeV08f5txUorLL9PjwT26ZEyWWCLwPtDKz1UpbG51WtHkgASi1jFT32Q2gqYwTesW0g2l1BqTWXVsF8JLTFb3PM8wgguTwIAuHxhsR9MYt058FPRdr)

* Component.spec.ts

  This file is used to test the methods that are written in the component.ts file. It checks to make sure that the methods are behaving how you want them to. Because the tests are local (within VS Code) they can't actually reflect your web application. So we utilize mock testing to test our methods with "fake" data that we create. 

* Mock Testing

  * Testing a component is an important part of this class and the functionality of the project (it also helps with debugging). Mock testing data is in the (nameHere).service.mock.ts file. In the component.spec.ts file, after all the imports, there is a describe method that defines the imports.

  * There is also a beforeEach method that does something before testing a method. If a beforeEach method has "async" then whatever is defined in the beforeEach will happen asynchronously from the other tests.

  * The tests start with an "it" statement telling what the method should do or what it should output. Commonly seen are toBeTruthy() and toBeFalsy() which say if something should be true or false. equals() is also another common statement in a test. 

  * As mentioned before, each test looks at the file (name).service.mock.ts. This is where all the "fake" data is defined and what the tests refer to. This file is like a "fake" database of information that you are testing.

![](https://lh4.googleusercontent.com/f4FkMUUFbpQnirztYtoDEnfMib_qnZarocSSQI7lEx6MbSEp32td2BEy0RJqUBROQq_2gqZHxT3U6Z2fWo5S25-Ek804q14aBPyu4lZGuPslPvgdlgla4vjfk2aFqvQL_ZNcnX0Q)

![](https://lh5.googleusercontent.com/rxXUxpuxKDr1B2XyJEBuc_Kn6ySRuo_7QFwAPnD9gdkj0SlISOoeeqBISvxKhLxjrMYvqURF_JNdDr-qM_t6HDfp6ejgrKxuLghMWx9B1eEWe0RxxLKaJGUvJNdzzj3brVfIZzYy)

* Component.scss

  This is the CSS file for a component. It styles the text along with the pieces of the component itself. You can add color, borders, background images, dropdown menus, etc. This website has a lot of CSS stuff that you can quickly apply: <https://www.w3schools.com/css/css_border.asp>. 

  CSS is a standard but powerful facet for developing web applications. (This will allow you to give your application a professional setting and look for the user). If something looks clean and professional, it's bound to do well, and it gives a sense of confidence. Avoid going over the top with it and ending up with a cluttered UI, but there are enough options to make your web application stand out.

* Creating an Object

  A TypeScript file (not attached to a single component) can be used to define an object. So if you want to create an object that resembled an email, you would declare that the object "email" has a date, body/message, subject line, sent from, and sent to fields. The name for this file would then be "email.ts" So any component that utilizes this object (by importing it) can access any of the fields. 

  Each field has a type. Some common ones are string, boolean, etc. You also have the ability to make user defined types.

  Try to think of this file as multiple people agreeing to speak in the same language. 

![](https://lh4.googleusercontent.com/PLz8-h1YHOxWHCepDTtchRMHpB9ev-r2pQk8CDxeTwM524gcPUqcR3TrlQ7oTnOQ1saiaEey_RsRuOOo85Wg6IMK_BR5YMnUlDuqcZtn3VRpDLSQJlnD2tNI33-UoopO6VsyKbcF)

* Services

  * Services will be an important part of your web application. A service file has a bunch of methods that can be utilized by any component. Unlike a service file, TypeScript files for a component are specifically for that component. 

  * Components that use services, have to share the same information. For example, if two different component files utilize a service, and that service has the variable "note", then "note" is defined the same in both files. To declare that a component is using a service, you need to import it. 

![](https://lh4.googleusercontent.com/01FO-VqDKQ4cprYak2jna1CtW1Dqq0Oz75BuXIHxc3xaQkx3MWcWEIiZXMeT4jMUERFQIcJrlPF_6X4G_h-Z0wc2niau2hpiSpeFWcA3yWBESyFBYkADLgYEWOF-Oao6UMc7J1b0)

  * Spec files for components also need to import services so it can be tested for a component.

  * Services also have spec files to test the methods. NOTE: Inside of these spec files, you create the data that you want the service to test.

![](https://lh3.googleusercontent.com/oDxkMooiETSDqCYBmPpCu-cBJacxe-bKhVQoCqO3bPRAFf_2z2VIRwkKaA2SC2IXp3r_X95n5PFlaVn-duelrL9elYbrcHtWE8hYWyz45M3sS1nUnfpzc-ifDr7m99TmYFb6NsKj)

## Server Side Files

* Controller

  Remember that the server is a way for a user to access specific information from a database. So this controller file has methods that access and change information in a database.

  The controller also has a .java file which is similar to an object file like "email.ts" on the client side. It's where an object/variable is defined and it can be utilized in the methods. 

![](https://lh6.googleusercontent.com/sYk8EkK8RFDnu5Bjfl8BqCQ7cFSaN9a9pF3dPcLZKUzn_4YSHc2nZN1RXtFkrfQrqA9xI0ewI2EmXqAbPxZXns71y-Hwo0ENO21N64Mt3MwOCL8qnyYAPJwKQuTXwzqm5sho8CRc)

  After the .java file comes the Controller file, which is written in Java. As mentioned earlier, this file has methods that work within the parameters you set in the .java file. It "talks" to the database and can retrieve or change information in the database.

  If you have taken Data Structures, you will notice the syntax is a little more complicated, but is still familiar enough that it's understandable.

![](https://lh5.googleusercontent.com/hBJWz_9NHEEGppbM_26Y_LEahCQSUuwxjYOJibGNgYLoPWXJmY0VA5QM__EM-8_mM9cL6YmPoP3e0-nmYxb2olbx-rBiwdOObBM65uTDZQDbtNzU70qUPYCvXExhFB8DKyWeCHTR)

## Controller specs

  The Controller also needs to be tested so you know the server is doing what you want it to. You will configure these tests by writing JUnit tests. 

  Like in the client, this test file also has @BeforeEach to declare what is instantiated before each test.

  The data that you test is also something you define at the beginning of this file. You're essentially creating a mock database.When you add an object to a database, it must have the same fields as it does in the .java file. So our email object would require the fields body/message, subject, etc.

![](https://lh3.googleusercontent.com/Y0yPT_U8-DxJXy9LksmXVBFCAVyYdNT2nbpN6ZZZpMGrNVW7XqjY2G-E9OB0eReShRaq5CrN4AXvReVgetZlL4w_V3yR1hgyiwbeDZpWhxAQU9qOpvZJM0sirV8bHyN1d_wZ-5x4)

  Each test should have an @Test to declare it's a test. It will also provide a "Run Test | Debug Test" option. Clicking Run Test will either give you a check mark or an X (failure). NOTE: Just because a test passes, does not always mean it does what you want.

  At times a failing test can be the result of how the test itself is written but most likely it is an issue with the method. Being able to read why a test is failing, and possibly which line is causing the error, is a necessary skill in order to debug your code.

![](https://lh6.googleusercontent.com/2l6W4UDl5b9bQ-gqxeDGj1GHH5NF-sbUOrD0T7wZ9DGSm4t13TXOdMC_v-PYbQi1LtWygJk7GvzmqqcWY0qo9aDw8Jok4sFLs0VZMv9ZoqwyxWbAIG5agTdW0WceaCOK2XrgVUfg)

  JUnit testing can be tricky and the syntax can cause headaches at times, so this is a topic we would suggest you ask your professor(s) about if you need further clarification.

## Databases 

* About Databases

  Remember that a database works as a bank of information/data. You are able to add, remove, or alter these entries in the database.

  For this class we used MongoDB as our database. When you are working on your iterations/labs, you are able to add sample information to your database with a JSON file. To add sufficient amounts of sample data easily, you can use a JSON generator which can be found online. We have found [Mockaroo.com](https://www.mockaroo.com/) to be the easiest to work with as the fields are easily customizable and there is a straightforward link to download the document.

  To view a database in VS Code, you need to download the Azure extension. From there you should click "Attached Database Accounts." From here you can see what is in a database.

![](https://lh4.googleusercontent.com/FSmVFx37qLxePxwwb34jvi4tjfw0B6zchOSFCBAZAxuN7QzRDPZx4IBCDRh2jaUBdRFKCFy-Pgn81lcEYlArw9PjGGf67KiaemdWtpazoCKNbjQ22RwMylqHlHR0nWRy9Vk5A6_B)

![](https://lh6.googleusercontent.com/Tg4sR4pX3bgmtBLRREU0D3HjYA42arX-qaDC2mkXbCQlErD3LbPNd_-sOFCdWdy3JTSe5dTLuzqsyDby8dPLcoL90FEixY-gGglBYeZl4tWw2amao5K0sEpkDLZYX-7at2DYq2lm)

## Seeding the database

  Seeding the database takes an existing JSON file and adds that to a database. Seeding the database will grab all of the current JSON data in VS Code and add it into the database.

  To seed a database, you need to first cd into the database file. So open a new terminal and the command is cd database. Then ./mongoseed.bat seeds the database.

## E2E testing

E2E (End to End) testing tests the connection between the client and the server. It tests whether or not your client to server interaction works and does what you want it to do such as adding an entry to a field or deleting an object.

The E2E files are in their own folder called e2e. 

![](https://lh6.googleusercontent.com/7JiFoIdKL7RRCs0dy88PnmjK1btuGXWsnKGuwMUqHdKHaYwxkuf6mrpgbuf4gqJ3fWPzZVrGXwZKfR050t-iPastqAsc3ufoy0Gv3i-04GNZEeVGO71CaKJNP9oys2enAItTmjIG)

Like the components in the client, there is a .ts file and spec.ts file. You're basically writing more spec tests (like you did for components) but it doesn't test a certain component, but rather the entire application's functionality, the goal is to write tests that will replicate user scenarios.

![](https://lh5.googleusercontent.com/8Di4AWALKVE4xjB_OxTfrPMhXO1I0QQR4rU70avX6swIXZsTQfLmswyc_50qx4gCM20odivhu-gXUuuBSsid3rCtr56W0y1yjEbLaQd4VXdGI3aQ2fj26KzTGJfj1qGAMI2TgZJl)

![](https://lh5.googleusercontent.com/351PEgCNbcCesgLELL7GEtz--WfCtgqaKUu35B-BA3VLbJBSgYk0WlvJdcTCL8ovTPYlA3qwR-KaZj7UMi4vV6TC31KSMrNFT4bBlQyiG05KqzjaF_Frc4ORDDQSemOSKtnOvvx-)

## VS Live Share

VS Live Share is an extension on VS Code that allows you to pair program with other people. It is similar to Google Drive where multiple people can work on the same code at the same time but in this case one person is hosting the session so they will be responsible for running the client, server, and tests as well as handling commits and pushes.

This is an ideal tool if you have to work remotely, because you and your group can see in real time what is being changed. This also allows you to have an extra set of eyes to look over code which can be very helpful for finding small bugs.

To use it, you first need to download the extension along with the Live Share Whiteboard extension. When you first start or join a collaboration session, you will have to login into GitHub. Then you should have code to share with other people who can join the session

![](https://lh5.googleusercontent.com/299hH3COnl8Kbi2m_1Usg2qWA5l2uJfKgo605wGFqUSw_mqtsEu3EMutdJPXicP_J-kT0fgPH782daBbLA_sD1qevQOu1cxn3ljzI3J36MRNGQsAZKi79hFRoKE12nU11pi3JoHl)