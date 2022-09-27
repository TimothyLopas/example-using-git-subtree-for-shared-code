# Use Git subtree for shared robot code

This example robot code repository includes another robot repository (https://github.com/robocorp/example-shared-robot-framework-keywords-and-libraries) as a Git subtree.

The included repository contains (fictional) common shared code used by many robot projects. Instead of copying & pasting the code into each robot project that needs it, isolating and sharing the common code between the robots might make sense!

This project was created using RCC and the standard Robot Framework template.

The robot includes the shared robot code from the other repository as a Git subtree. The subtree is stored in the shared directory.

The shared Git subtree in this project was created with the git subtree add command:

git subtree add --prefix shared https://github.com/robocorp/example-shared-robot-framework-keywords-and-libraries.git main --squash 
A new directory is now created in this repository called `shared` that contains a copy of the "example-shared-robot-framework-keywords-and-libraries" repository.