# Hello, AI!

Today, we'll build on our knowledge of HTML tags by making our first changes to HTML, and practice using our new knowledge of GitHub. You'll learn two new skills: how to preview your work in a web browser as you change it, and how to test your changes and see feedback in GitHub. You'll also have a chance to explore AI.

## Requirements

- [ ] Change the title of the page to "Hello, world!"
- [ ] Add a heading in the first line of the body tag with the text "Hello, world!", using the `<h1>` tag.
- [ ] Add a paragraph on the next line telling us who you are using the format "My name is ________" (Add your name in the blank). Use a `<p>` tag.
- [ ] **Optional:** Use the Cody AI plugin in VSCode to see how far you can get with each level of this assignment from the goal example below by **describing what you see and want to do**. How far you get will not affect your grade on this assignment, so don't be afraid to try your best and take risks! One prompt you could use to start is `How can I make a rectangle with a red line around the outside in CSS?`?

How far the class gets in general with this assignment, along with the weekly reflection, will help me fine-tune what I teach you this semester.

## Finished Assignment Example

### Before AI (this is the part you will be graded on)
<img width="1103" alt="Screen Shot 2023-09-05 at 3 08 19 PM" src="https://github.com/ProfessorKolodziej/cm523-hello-ai/assets/1828613/308802e7-3b64-467d-bccf-b472981dff7a">

### See if you're able to get to this with Cody AI
This part is optional. The goal is to see if this is a tool we as a class might want to use to help boost our coding skills this semester. While it seems unintuitive to try doing this when I haven't taught you how to do any code yet, learning to describe what you want to accomplish in plain language can help you find the right steps in code more quickly. Take small steps and do your best - you will not be graded on this. One prompt you could use to start is `How can I make a rectangle with a red line around the outside in CSS?`? As long as you have an h1 and a p tag in your code, doing this experiment won't affect your grade, no matter how good or bad it ends up looking.

This is my first time trying this idea out, so if you can't get it, or only get part of it, it's okay! 

Hint: you will need to add the line `<link rel="stylesheet" href="css/style.css">` to accomplish this in in the head tag of your HTML.

<img width="1103" alt="Screen Shot 2023-09-05 at 3 08 05 PM" src="https://github.com/ProfessorKolodziej/cm523-hello-ai/assets/1828613/59cd7ab4-5b3b-4c84-b6f5-9b9d2320ad79">

## First: What new things are we learning in this lesson, and why?

Today, we're going to learn all about how to preview and test your changes, so you can be successful in this class! We'll be doing this using a program called `npm`. `npm` stands for Node Package Manager, and it helps us leverage other people's code to make our lives easier while developing websites. You don't need to know much about `npm` yet, except that you'll see it in some commands you can run, like this: `npm run start`. This command is the command you'll use to preview your work.

One of the hardest things to learn when learning a new programming language is the **syntax** of the language. The syntax of a new language is all those little rules that everyone agrees are consistent so that we are all on the same page about the _meaning_ of what we're saying. Computers are especially picky about syntax. In HTML, syntax includes things like how a **tag** is written. Everyone agrees that HTML tags have a syntax like this: `<tagname>your content</tagname>`. Notice the placement of things like `<`, `>`, and `/` in the example. That's syntax!

Because syntax can be hard to get right the first time, I've also added a special command, `npm run test`, that will test your code to make sure the syntax is right, and that your assignment meets the assignment requirements. If you run this and get a message that all tests passed, you'll know you're getting full points on this assignment! The same checks here are the same checks you'll see in Gradescope. This is called autograding.

### New terms

- **Syntax:** A special set of rules for how to write code that tells a computer how to read the code. Each language has its own syntax.
- **Tag:** A piece of HTML code that helps a computer understand the meaning of your content. Different tags have different meanings, and tags have a **syntax** that helps a computer understand where that meaning starts and ends, like so: `<tagname>your content</tagname>`. For example, an h1 tag means that the content inside is the main heading for the page, and looks like `<h1>Your Title Here</h1>`.
- **npm:** Node Package Manager. A package manager helps us use and leverage other people's code to make our lives easier. As your professor, I'm using `npm` to create a special command that will help you see your HTML, CSS, and JavaScript changes instantly in a browser. You'll learn more about `npm` as we go!
- **`npm run start`:** A Terminal command that will show a preview of your work in the browser.
- **`npm run test`:** A Terminal command that will help you check if you completed all the assignment requirements correctly.

## Instructions

These instructions will build on your knowledge by having you practice the same set of skills you learned in Test Your Connections, but without the step by step screenshots. See if you can remember how to do each step without the help of the screenshots. If you are having trouble or getting stuck, head back over to the Test Your Connections assignment instructions for a reminder.

### 1. Clone this repository and find it on your computer

1. Use the "Open with Github Desktop" button to open this repository in GitHub Desktop.
1. When the window opens in GitHub Desktop, choose Clone.
1. Right click on your repository name in the upper left, and then select "Open in Visual Studio Code".

### 2. New: Install development dependencies (Only once per assignment)

You only need to install development dependencies when you first start the assignment. Once you've run `npm install` on an assignment, you don't need to do it again. When you start a **new** assignment, that's when you'll run this command.

We run commands in the Terminal. The easiest way to do this is in the VSCode Terminal panel, which will run the command in your assignment.

| Step | Screenshot |
| --- | --- |
| Open the Terminal panel in VSCode by selecting View > Terminal from the menu. | <img width="2048" alt="Screen Shot 2021-09-06 at 1 14 25 PM" src="https://github.com/ProfessorKolodziej/cm523-hello-ai/assets/1828613/baf1ed80-db7b-4549-8f25-fb07fff875d8"> |
| Type the following command into the Terminal panel, and then hit enter: `npm install`. Notice the name of the project folder in the terminal panel as you do this. This is called the current working directory. | <img width="918" alt="Screen Shot 2021-09-06 at 1 23 33 PM" src="https://github.com/ProfessorKolodziej/cm523-hello-ai/assets/1828613/3719fc6a-d625-4435-b299-49f9bfd1373b"> |
| Allow the install script to run. This is installing your development dependencies - the things that make your website run. Wait until you see a screen similar to this. You can ignore the vulnerabilities message - that's my job to maintain! | <img width="918" alt="Screen Shot 2021-09-06 at 1 24 39 PM" src="https://github.com/ProfessorKolodziej/cm523-hello-ai/assets/1828613/0fe43bda-8c3a-4315-81a1-6648d2364a66"> | 

### 3. New: Start the assignment (When you're ready to start work)

You'll run the `npm run start` command each time you're ready to start work. For example, if you work, and then shut your computer down, and then come back the next day, you'll only have to run `npm run start`.

Note: if you run into any trouble or errors, such as `EPERM: operation not permitted, uv_cwd vscode`, try clicking the trash can in the Terminal panel, and then reopening it and trying again. Sometimes VSCode's integrated terminal can be buggy with permissions.

| Step | Screenshot |
| --- | --- |
| Clear the Terminal panel screen using the `clear` command if you are on a Mac, or `cls` and hit enter if you are on Windows. This will make it easier to see what you are doing, and is a good habit to get into each time you run a new command. Then type `npm run start`, and hit enter. | <img width="918" alt="Screen Shot 2021-09-06 at 1 27 10 PM" src="https://github.com/ProfessorKolodziej/cm523-hello-ai/assets/1828613/30eea495-fafc-45f4-804a-eaf121f14f56"> | 
| <p>A new browser window will open, and your terminal panel will look like the screenshot to the right. What is happening is that the terminal is watching your files for changes, and at this point, you can safely ignore it and focus on your code.</p> <p>The browser shows a preview of your assignment. There's nothing there yet - that's okay! Next, you'll make a change in VSCode, and the browser will show your changes automatically.</p> | <img width="996" alt="Screen Shot 2021-09-06 at 1 28 45 PM" src="https://github.com/ProfessorKolodziej/cm523-hello-ai/assets/1828613/30eea495-fafc-45f4-804a-eaf121f14f56"> | 

### 4. Make changes to the HTML

2. Read the requirements above carefully. Then, use the information in the requirements to make a change to your code.
3. Save your changes. Your browser should automatically update and reflect the changes when you save!
4. Keep working until you are happy with your assignment progress, and ready to double check it meets the assignment requirements. Check your Terminal panel if changes stop showing up in the browser - there is probably an error in your code.
5. Once you've reviewed the requirements and sample image to be sure your code looks similar, commit it! You can commit as many times as you like. You could also commit if you are done with code for the evening, but want to come back to it the next day.

### 5. Commit and push your changes to GitHub

1. Open GitHub Desktop, and make sure you are in the CM523 Hello AI assignment by checking the repository name in the upper left.
2. Review the files in the Changes tab. Make sure that everything you want changed has a checkmark by it. You can click individual file names to see what the changes are and be sure that the changes are intentional.
3. Write a commit message in the Commit Subject area. Keep it short and descriptive of the changes you made.
4. Hit “Commit”. This creates a commit, and your changes will “disappear”.
5. Look for a small arrow with a number next to your **branch**. This is how many changes you will be pushing. Click the small up arrow to push your changes to GitHub.

### 6. New: Test your code

| Step | Screenshot |
| --- | --- |
| To run the test, you will need to stop the command you have been running (`npm run start`). Use the Control + C shortcut in the Terminal panel to stop the start command. Your Terminal will look like the right (click to see a larger view). If you have the folder name and percent sign at the bottom, that is how you know it is stopped. | ![Screen Shot 2021-09-06 at 3 33 47 PM](https://github.com/ProfessorKolodziej/cm523-hello-ai/assets/1828613/f98b0f95-39b0-49b1-9db8-572a940652f0) | 
| Clear the terminal using the `clear` or `cls` command, and then run the following command: `npm run test`. | ![Screen Shot 2021-09-06 at 4 26 04 PM](https://github.com/ProfessorKolodziej/cm523-hello-ai/assets/1828613/81148591-0242-40b5-ae50-db35beae11e5) | 
| If there is a problem with your HTML, the test will stop, and your results will look like this. Follow the tips on the screen, and work on errors from top to bottom, rerunning `npm run test` each time you make a change to see if the change worked. In this example, the error is related to a missing end bracket on the title tag. | ![Screen Shot 2021-09-06 at 4 11 32 PM](https://github.com/ProfessorKolodziej/cm523-hello-ai/assets/1828613/8d690941-aa65-4f87-9619-991670139449) | 
| If your HTML is valid, but you are missing an assignment requirement, your test results will look similar to this. Look for phrases or sentences in the error that are familiar. Again, rerun `npm run test` each time you make a change. | <img width="1777" alt="Screen Shot 2021-09-06 at 3 47 36 PM" src="https://github.com/ProfessorKolodziej/cm523-hello-ai/assets/1828613/1eeaa7ff-f9a3-4376-9fbb-b7102d898ae4"> | 
| A successful test will look similar to this. Keep going until your test is successful! If you're stuck, don't get discouraged, and reach out to your classmates to compare notes. You can use Pronto to do this, or talk in class directly. | ![Screen Shot 2021-09-06 at 4 17 14 PM](https://github.com/ProfessorKolodziej/cm523-hello-ai/assets/1828613/610e6b09-c858-4a48-9f1b-c5fdef4a6802) | 
| Return to GitHub Desktop, and then commit and push any new changes you've made to Github. | ![Screen Shot 2021-09-06 at 4 17 14 PM](https://github.com/ProfessorKolodziej/cm523-hello-ai/assets/1828613/9e736ef5-b4fd-44c9-8a53-c2a7841fdc19) | 

## 7. Check Gradescope to see how you did!

1. Go to this week's module in Blackboard, and find the assignment submission link.
2. Submit your assignment using this repository and the main branch.
3. Gradescope is where you will see the results of Autograding, and any additional comments I make on your assignment. In later assignments, I'll give you additional feedback on things like performance and coding style, so you know how to improve your code for next time.
4. With luck, all the tests will pass, since Gradescope uses the same `npm run test` command as you did earlier.
5. Your grade in Gradescope should sync with Blackboard automatically once I release grades. If not, please let me know!
