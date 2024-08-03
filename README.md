RobotFramework-Practice
Practicing Robot Framework using Browser Library for Web GUI Test Automation and Requests library for APIs Test Automation.

Project Design:
We are implementing the Object Model design pattern (Page Object Model for GUI). And below is the project structure folders:

Object Models folder: Includes the APIs clustered by the services and GUI Pages
Tests folder: Includes all of our Test Suites and Test Cases
Resources folder: Includes any other files that aren't keywords/code/actions like Global Variables, Configurations, Test Data files, etc...
Utilities folder: Includes the common global utility keywords/code/actions to be used in other folders, mainly the Object Models and Tests
Setup:
Install Python™
Install Node.js®
Open a terminal/commandline windows and Install Robot Framework from PyPi with pip: pip install robotframework
Install Browser Library: pip install robotframework-browser then initialize it: rfbrowser init. If rfbrowser is not found/installed for any reason, try python -m Browser.entry init
Install Requests library: pip install robotframework-requests
Install JSON Library: pip install robotframework-jsonlibrary
Install Pabot to be able to perform Parallel execution when needed: pip install -U robotframework-pabot
Install VS Code IDE and install Robot Framework Language Server plugin and you can install Material Icon Theme for better icon visibility.
Execution:
To execute all the test cases please run the following command from the terminal/commandline: robot -d Results Tests
And we can change variables like this to run on Firefox with headless mode robot -v browserType:firefox -v headless:True -d Results Tests
We can perform Parallel Execution with the pabot instead of robot command like this: pabot -d Results Tests
