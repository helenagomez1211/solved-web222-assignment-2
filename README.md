Download Link: https://assignmentchef.com/product/solved-web222-assignment-2
<br>
This assignment will help you learn and practice working with Arrays and Objects in JavaScript.

<h1>Setup</h1>

This assignment uses a technique called “Unit Testing”, and relies on a number of dependencies, which must be installed on your computer. A dependency is a library, tool, or other piece of software that is needed in order to build, test, and run another piece of software. JavaScript projects often rely on hundreds or thousands of dependencies, and getting used to installing and using them is an important step.

In order to install these dependencies, you must first install Node.js on your computer. See installation instructions at: https://nodejs.org/en/

You can install the LTS (Long Term Support) version of node.js, which is currently 12.14.1, although any 12.x.x version should work.

<h1>Install Dependencies</h1>

Open a command line terminal and navigate (i.e., cd) to the directory where you have unzipped the assignment files. When you type dir (Windows) or ls (Linux/macOS) you should see this README.md file, package.json, etc.

In this directory, install the assignment dependencies using the

Node.js Package Manager command, named npm. The npm command is installed along with node.js. In your terminal, type the following:

npm install

This will download and save all the necessary dependency files to a folder named node_modules/ in the current directory.

If you have trouble getting “npm install” to work:

Did you install node.js?

If you type “node –version” in your terminal, does it print the version? Are you in the right directory (you must cd into the correct directory)

If you need help, ask your classmates and/or talk to your professor.

<h1>Install a Proper Editor</h1>

You will need a proper editor to write code for the web. The most popular choice is Microsoft Visual Studio Code (aka, VSCode). VSCode runs on Windows, Linux, and macOS. You can download and install it for free from:

https://code.visualstudio.com/

NOTE: VSCode is not the same as Visual Studio. You should have both installed

A number of extensions are available that will work automatically with the scripts and configuration in this project, and are recommended:

eslint https://marketplace.visualstudio.com/items?itemName=dbaeumer.vscode-eslint prettier https://marketplace.visualstudio.com/items?itemName=esbenp.prettier-vscode

When you open this project’s folder, VSCode should offer to install these recommended extensions. Once these are installed VSCode will automatically show you errors as you type, automatically format your code when you save, and show you spelling mistakes in your code comments and names.

If you want to use a different editor, that’s fine. Confirm with your professor that it will work for our needs. You may not use Notepad, for example.

<h1>Learn how to Run the Assignment Tests</h1>

You are asked to complete the code in the file src/solutions.js. A basic file layout has already been created with various functions and variables.

Also, detailed comments have been left above each function you need to implement.

In addition, unit tests have been written for each function. They are named

src/problem-0.test.js, src/problem-1.test.js and so on. A Unit Test tests the smallest possible unit of a software system or component, and we write many small Unit Tests to prove that our implementation works as we expect. For example, we expect 2 + 2 to return 4, not 5. We can write a unit test for this to confirm that our code does what we expect. See http://softwaretestingfundamentals.com/unit-testing/ for more info about unit tests.

These tests will help you determine if your code is working correctly: running the tests should produce the output that the tests expect, and that tests will either pass or fail.

To run the tests, use the npm command:

npm test

Your goal is to get all of the tests to pass correctly. If a test fails, pay attention to the error messages that get produced, what was expected vs. what was actually returned, and make corrections to your code in assignment1.js.

<h2>Different Ways to Run Tests</h2>

If you are going to run your tests over and over as you make changes to src/solutions.js, you can run the tests so they automatically watch for changes, and re-run whenever you save your file:

npm run test-watch

You can stop the tests from running using CTRL + c.

Next, you can run a single test instead of all tests:

npm test problem-0

This will only run the tests in problem-0.test.js, making it easier to work on only one problem at a time.

<h2>Debugging Code and Tests</h2>

You can also use VSCode’s built in debugging tools to run and debug your code, or the test code, within the editor, step through code, inspect variables, <a href="https://github.com/microsoft/vscode-recipes/tree/master/debugging-jest-tests#debugging-all-tests">examine call stacks, etc. See the </a><a href="https://github.com/microsoft/vscode-recipes/tree/master/debugging-jest-tests#debugging-all-tests">following instructions (https://github.com/microsoft/vscoderecipes/tree/master/debugging-jest-tests#debugging-all-tests)</a><a href="https://github.com/microsoft/vscode-recipes/tree/master/debugging-jest-tests#debugging-all-tests"> for more details.</a>

<h1>Learn how to Lint your Code</h1>

In addition to running unit tests, you can also run a linter called eslint.

Linting helps to find and remove common errors in code, for example, missing a semi-colon, or forgetting to declare a variable.

To run eslint, use the npm command:

npm run eslint

If there are no problems, there will be no output. If there is any output, pay attention to what it says, so you can make corrections. For example:

assignment1/assignment1.js

18:9  error  ‘x’ is defined but never used  no-unused-vars

Here, we see a lint error, which has various information:

<ol>

 <li>The filename is listed first, assignment1/assignment1.js</li>

 <li>The line number is listed next: 18</li>

 <li>The column number on line 18 is listed next: 9</li>

 <li>The actual error or warning comes next: error ‘x’ is defined but never used</li>

 <li>The rule name comes last: no-unused-vars. You can lookup how to fix these errors using the rule name, for example: https://eslint.org/docs/rules/no-unused-vars</li>

</ol>

Your code should have no lint errors when you submit it.

<h1>Learn how to Properly Format your Code</h1>

Source code needs to be properly structured, use consistent indenting, semi-colons, etc. Doing so makes it easier to understand, read, and debug your code.

Your code must be properly and consistently formatted. You can do it by hand, or, you can use Prettier (https://prettier.io/) to do it automatically.

There are two ways to use Prettier. First, using the npm command:

npm run prettier

This will rewrite your files to use proper formatting. NOTE: running this command will overwrite your file, so make sure you have saved your work before you run it.

The second way to run Prettier is using the Prettier extension, and format-on-save. If you install the recommended extensions and settings for this project, saving your file will result in Prettier automatically fixing your code for you.