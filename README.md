# Exercise

GitHub:
For your solution fork this repo and create a pull request
https://help.github.com/articles/fork-a-repo/
https://help.github.com/articles/creating-a-pull-request-from-a-fork/

======================================================

The following Tips are for NetBeans, but you can use any IDE you like for this Exercise.
You can get NetBeans from https://netbeans.org/downloads/
The "Java SE" Package is sufficient.

Import the Project:
Menu > Team > Git > Clone...

Commit your changes to your local copy:
Right click project > Git > Commit...

Push your changes to your Fork on GitHub:
Right click project > Git > Remote > Push to upstream

Clean and Build:
If there are any compile errors, or if anything strange happens, right click the project and click "Clean and Build".
This builds the whole project from scratch.

Run All Tests:
Tests are written in JUnit 4.12. There is an example in "Test Packages" (src/main/test).
Right click the project and select "Test" to run all tests.
You can also set a keyboard shortcut via
Menu > Tools > Options > KeyMap > Enter "Test" into "Search:" Textfield

======================================================

Exercise:
Implement the following requirements and write (unit-)tests to demonstrate that your solution works.

- Implement Words.asString() so that it returns all the words found in the Reader separated by spaces:
new Words("first line\nsecond line").asString() == "first line second line"
HINT: You can implement it as you like, but BufferedReader and Stream should provide everything you need

- Enhance the "Words" class so that it can also read text files? (character encoding is irrelevant)
HINT: there is a subclass of Reader that is helpful here

- Redesign (e.g. add methods or change into interface) the "Words" class so that you can control
    - how words are discovered:
        e.g. transform "one-two#three" to "one two three"
    - how words are returned:
        e.g. transform "one two three" to "one-two-three"