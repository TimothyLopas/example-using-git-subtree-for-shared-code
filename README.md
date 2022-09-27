# Use Git submodule for shared robot code

This example robot code repository includes another robot repository (https://github.com/robocorp/example-shared-robot-framework-keywords-and-libraries) as a Git subtree.

The included repository contains (fictional) common shared code used by many robot projects. Instead of copying & pasting the code into each robot project that needs it, isolating and sharing the common code between the robots might make sense!

This project was created using RCC and the standard Robot Framework template.

The robot includes the shared robot code from the other repository as a Git subtree. The subtree is stored in the shared directory.

The shared Git subtree in this project was created with the git subtree add command:

git subtree add https://github.com/robocorp/example-shared-robot-framework-keywords-and-libraries shared
The .gitmodules file defines the path and the URL to the included repository:

[subtree "shared"]
	path = shared
	url = https://github.com/robocorp/example-shared-robot-framework-keywords-and-libraries
See the tasks.robot file for examples of importing and using the shared code.