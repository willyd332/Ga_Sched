## Bash Profile

The `~/.bash_profile` file allows you to maintain links to various applications from the command line and setup our development environment. There are other files we can use to modify these but today we just want to be able to open files in Chrome, Safari, Sublime Text, and other files.

To do that you will need to partner up with someone. You're going to work together once you have everything installed on your computer to create aliases on your computer. This will require you to put your terminal knowledge to the test!

#### Goals

- Edit the `~/.bash_profile` file
- File the exact path using `pwd` and tab-completion of apps
- Add `alias` for each application so files may be opened (You can use Atom, Sublime, or both)
- Open files and/or folders using `your_alias_name .` to test your script


##### Editing Bash Profile

- Navigate to your home directory using `cd`
- Open your `.bash_profile` file using `nano ~/.bash_profile`; this will open the file in your editor
- It might look like the following:

```bash
PATH="/usr/local/bin:/usr/local/sbin:$PATH"
```

##### Locating Application

> **Apps** - you should find Chrome, Sublime Text, and/or Atom. Additionally, you may find Atom and any other editor/browser you like.

- In a new terminal tab, navigate to the root of your hard drive using `cd /`
- `cd` into the `Applications` directory (Note some of you will have the Applications in the root Applications folder, while some of you will have it in your `username/Applications`, remember you can use `pwd` to find out where you are.
- `ls -l` to list all of your Applications
- Copy the application name to a blank text file (such as `/Applications/Sublime.app`)
- Repeat for each app

##### Adding Aliases

- At the **end** of your `.bash_profile` file, you may add an alias. You'll need the exact path of your apps to do so.
- You can add an alias by assigning a _command_ like so: `alias ws='open -a /Applications/Atom.app'` (Note yours may be different make sure you are printing your workind directory to get the correct file path, ex2 `# alias subl='open -a "Sublime Text"'`, Note if you have spaces in your application name use double quotes to wrap the space, pay close attention to the ex2, look at the different types of quotations.)
- Here are the aliases you should use for each app:
  * `subl` for Sublime Text
  * `atom` for Atom
  * `chrome` for Chrome

##### Testing

- Save your `.bash_profile`
- Restart your terminal (and close all tabs)
- Until you close & restart terminal, your profile changes will not be seen!
- Create an HTML file using the `touch` command.
- Open it with each application you found!
