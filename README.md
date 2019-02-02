# project-template
This project began with an article for creative writers, specifically screenplays.  It is meant to be for those who are not technically minded to learn the "script kiddie" approach to use the tools available to them.

The original form was a long winded and heavily commented bash script.  I chose bash because of my own lack of familiarity.  Still, as I learned more, I couldn't help but fix it up and expand upon it.  Taking a trip through commits may be an excellent, or perhaps funny experience.  That's your call.

Still, if you are new to bash scripting, this may be a great help for you.

## screenplay
This script started it all.  While the big lesson in my article was how to ask the right questions - skipping the details about writing screenplays, and breaking down problems as simple data manipulation - it was helpful to provide a simple script to demonstrate how many tasks can be easily automated without a CS degree just by looking.

This script creates a boilerplate to begin an organized writing session, creating directories and files that will help the writer get started with the project.

It takes a multi-word argument as a screenplay title.

It then creates a folder named after the screenplay with spaces replaced by underscores, and a subfolder called `assets`.  It then creates a file titled `notes.md` and a screenplay file of the screenplay name (with underscores) in the fountain format.

Finally, it populates the front end matter of the fountain file with screenplay name, writer, draft date, and contact information, as well as other supplementary fields that can be filled in by the end user.

## shellscript
This had more to do with wanting to demonstrate that I can write much better code than in `screenplay` than anything else.  Also, it provides a decent front end for my next creation - an all encompassing boilerplate program for any possible project.

This particular script is built around my own personal usage, but the second commit for it will be heavily commented as well.

This script takes a single argument, the shell script name, and creates a boilerplate for a shell script in my `$HOME/.scripts/personal` directory.  The boilerplate is based upon **"Mastering UNIX Shell Scripting"**, but may change.

Upon creation of the file, it calls up **nvim** with the file in the buffer.

I did not do anything to set script permissions, so `chmod +x` will be needed to run it still.

# TODO:
The next logical step is to take both of these templates, and turn them into functions to be used in an all inclusive shell program that will create whatever template I want.  Again, these programs are used for teaching, and will all be heavily commented, so anyone should be able to easily create templates of their own based around file creation, data population, and directory structure.  Even going so far as opening up an entire development environment to specific standards.
