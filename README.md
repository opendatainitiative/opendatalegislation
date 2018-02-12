# Project Overview
Many open data implementations are the result of good management and their policies. But any good policy can be modified by a change in management. To make good policy permanent, the policy must be made into a law. The law must cover just enough detail to establish a framework that the open data implementation can be built upon. We highlight and review open data legislation.

# Project Details
https://github.com/opendatainitiative/opendatalegislation/wiki

# Release Management 
* Create GitHub issues for features to be added to the project
* Issues and pull requests in the backlog, moved to the sprint while being worked, and then to completed
* Assign issues to milestones? Figure out how many milestones to releases...
* Minor releases 0.2 through 0.13 every week with changes until the major release
* Major release 1.0 scheduled for May2018 
* Finalize release 2.0 planning in Jun2018
* Major release 2.0 scheduled for Nov2018
* Finalize release 3.0 planning in Dec2018

# Working Together
* Minor changes to existing files or new files that do not change the project significantly from the project editors, get merged
* Major changes to the project or proposed changes from users without project rights, use a pull request so the project editors can review your proposed changes. For help on pull requests, go here https://help.github.com/articles/creating-a-pull-request/

# Publishing
* We started by creating the index directly in the ODI website
* Next if there are changes, once a week, changes get tarballed and dropped into http://opendatainitiative.io/tarballs, and the master branch opendatalegislation/index gets pushed into the master branch opendatainitiative.github.io/posts, master branch opendatalegislation/how-to and opendatalegislation/implementation get pushed  into master branch opendatainitiative.github.io/ root.
* Long term, we establish Continuous Delivery (CD) automation that deploys master on the established set schedule
