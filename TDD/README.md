Test-Driven Development exercise (with groups!)

You're working for ACME Robotics and we need a PID controller implementation for a new mobile robot product development!

This exercise has been completed as a group using pair programming. Once pairs are established, each pair worked as a unit with one "driver" and one "navigator". The roles flipped between the first part and second part of the assignment.

The first part of the assignment has been completed by each pair. Once design was completed, Pair A implemented Pair B's design, held a design review discussion, and eventually submitted a pull request, and vice versa for Pair B. A fully completed assignment has two parts: 1) Forked repository with initial design and a merged pull request from the other pair; and 2) Completing the other pair's implementation and submitting a pull request to their repository.

## Part 1

In GitHub, clone the cpp-boilerplate repository (Links to an external site.) (use driver's account)
Sign in to https://travis-ci.org (Links to an external site.) and https://coveralls.io (Links to an external site.) with your GitHub account (look for sign-in with GitHub button) and enable your newly forked repository. You can do this by following the setup tutorials on each service (start with Travis, then Coveralls). The cpp-boilerplate repository has two badges at the beginning of the README that show you what this should look like.
Update the README.md file with new Travis and Coveralls badges that point to your new repository.
Follow the commenting and style guide procedures from previous homework (Add @author doxygen tag to files you create in addition @file, @brief and @copyright).
Create a new class declaration for a PID controller (Links to an external site.) that computes a new velocity given a target setpoint and actual velocity.
Your class must contain private Kp, Ki, and Kd class members
Do NOT implement the compute method, just the class declaration and stub implementation (i.e. return some constant value)
Generate UML diagrams and add to repository (these can be image files, or links in the README.md file to google docs). Think through the class design and appropriate comments and requirements for implementations (utilize concepts from Weeks 2 and 3 where appropriate). The more detail in the design the easier it'll be for your group members to implement.
Create at least two unit tests for this class. One test must test the compute method. Write good tests to help the other pair in your group!
Update CMakeLists.txt file to compile and link newly created files. You will also need to update the lines used for generating the code coverage by adding any new files that were created.
Build and verify the tests fail
Commit the new changes and push to GitHub
Verify that the tests fail in Travis
Check code coverage in Coveralls (your src files should be listed in the report. If not, update your CMakeLists.txt file).
Inform the other pair and once they complete the below task, accept their GitHub pull request (check notes in readme and add/revise anything in pull request discussion) and merge changes.
Part 2 (Switch driver and navigator roles):

Fork the other pair's repository (fork to driver's account)
Complete the implementation and fix until unit tests pass
Make frequent, logically grouped commits and push the completed implementation 
Verify that the tests pass on Travis
Check code coverage on Coveralls
Set up a time to discuss as a group the history on both Travis and Coveralls. Does the implementation and test passing satisfy the original class design? What additional tests would you add?
Add notes and todo statements to the README file based on the discussions. Commit and push.
Submit pull request on GitHub to the other pair
Additional hints:

Pay attention to your readme.md file. Mid-term project requires much more content and description.
Do not commit old/temporary files to your repository (<filename>~). Modify .gitignore to ignore these.
Only files related to unit testing should go into the test/ sub-directory. Unit tests must use gtest framework in mid-term.
Only header files should go in the include/ sub-directory
Classes should be declared with their own header file, and implemented with a separate source file (put into app/ sub-directory)
Ensure your UML diagram(s) are detailed enough and up to date with final implementation (project guidelines specify uploading versions with different file names on major changes)
Commit messages should be 1-2 sentences (see guidelines). Commits should contain changes that logically go together. Do not define a class, implement it, set up unit tests, and edit your readme, and commit that as one change. Review git staging area if you're unsure how to commit select changes.
Make sure everything is commented properly with doxygen-style comments (project guidelines require generating doxygen docs so you'll see what isn't covered)
Don't forget about cpplint and cppcheck. Follow previous homework guidelines that require adding their output to repository. FIX ALL MAJOR ISSUES FOUND BY THESE TOOLS.
Submit: Link to your GitHub repository created in Part 1 with the merged pull request. Note that groups are only able to submit one link. Please note that as long as each pair clicks "submit", I will be able to see each submission. But just in case, please email me a link to your original repository: dpiet@umd.edu. Don't forget, the implementation phase should be merged back into the original repository via the pull request, so I don't want to review your initial cloned repository.

