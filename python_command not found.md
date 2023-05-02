#1./bin/sh: python: command not found

When I installed Python in M1 Mac, and I run my python file, it still shows : /bin/sh: python: command not found

Problem solved :

(1)Hold down command + , to go into settings

(2)type in Code-runner: Executor Map in the search bar

(3)Underneath the Code-runner: Executor Map settings click on Edit in settings.json

(4)In the code-runner.executorMap portion of the .json file, make sure In the python section it says “python”: “python3 -u” (Adding the “3” is what’s different) and not just “python”: “python -u”

(5)Save the changes and run the code through code runner again. That’s what made it work for me.

<img src="https://global.discourse-cdn.com/business7/uploads/codewithmosh/original/2X/c/cba8eabfcf5820c2f3f3a2d21566a839c9439dea.png7" alt="description of image" width="300" height="200">
