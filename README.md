# project-template
This is a script to create a project template for writing screenplays.

The script is very easy to modify for whatever project structure you may need.

Here is how I used it, with very verbose comments.

## Script execution
Script is stored in a directory on my path and `chmod +x screenplay` makes it executable.

Script is used by calling `screenplay '<name of screenplay>'` in the directory that the project will be created.

## Assign argument to variables
The name of the screenplay is assigned to two variables, `name` and `directory`.  `name` is the argument in all caps, and `directory` is the argument with blank spaces replaced by underscores.

## Checking
The conditional checks to see if `directory` exists already.  If it does, the script will end with no actions taken.
If this step is not included, then the initial files will be rewritten and any previous work will be lost.

## Creating the project
The actions are well commented, and can easily be modified, but the end result is to create a screenplay directory, and an assets subdirectory.

In the main directory is a `notes.md` file which is empty, and a .fountain text file with the front end matter automatically populated.

The script inserts the first two lines to the .fountain file, a `Title:` key, followed by the title in all caps along with bold and underlined formatting for the fountain markup - this is standard formatting for screenplays.

The script then populates the rest of the front end matter with the rest of the key / value pairs that contain my personal information by reading the file stored in `~/.templates/screenplay`, which is a simple text file written out as regular front end matter.  I have included the text file for reference.

The rest of the script simply explains what the script has done to the user.

The end result is a file structure;
~~~
-<screenplay_name>/
| <screenplay_name>.fountain
| notes.md
  - /assets/
~~~
and the `<screenplay_name>.fountain` file containing
~~~
Title:
        _**<SCREENPLAY NAME>**_
Credit: Written by
Author: Shiva Rodriguez & D. Duckie Rodriguez
Source:
Draft date:
Contact:
        Siren Productions Media
        121 Birch Tree Drive
        Ormond Beach, FL 32172
        (123)456-7890
        someone@gmail.com
        someone-else@gmail.com
~~~

## TODO
Auto populate the date when I get around to it.
