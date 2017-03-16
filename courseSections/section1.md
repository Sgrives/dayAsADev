Section 1 - Creating a Development Environment
=============================================

Developers generally work closer to the bare bones of the computer than your average user. That means lots of time in the 'command line' and not relying on 'GUI' (Graphical User Interface) tools. However, to get your computer setup for web development is an are in and of itself - especially on Windows.

Fortunately, there are a number of cloud based development environments available that provide almost identical experience but with everything ready for you out of the box. For this course we will be using [Cloud9](https://c9.io/).


1. [Create a free Cloud9 account](https://c9.io/signup)
2. Choose `Create a new workspace`
3. Call your workspace `prototype-website`
4. Choose a Hosted workspace and make it Pubic
5. Choose `Blank` as a template
6. Create the workspace (This may take a minute or two)

![Cloud9 setup](../images/c9Setup.png)

When your workspace has been created you should see it open in your browser. It will look something like this:

![Cloud9 Initial Page](../images/c9InitialReadme.png)

What you are seeing in this image is an **Integrated Development Environment (IDE)**. IDEs are highly complex applications and take a bit of getting used to. Think Microsoft Word, on steroids, exposed to radiation in a secret nuclear incident and having gained super powers...something like that. Regardless, the important thing is that Cloud9 gives us the four critical components of our developement environment:

 - A **file system** to store our source files (code, images, HTML, CSS and others)
 - An **editor** to edit the above mentioned source files
 - An **operating system** to run the program described by these files
 - Finally, a **command line** or **terminal** to send instructions to the operating system

 Updating the README
----------------------------

You'll notice that a single file has been created for you already - `README.md`. It's a convention of all good projects to have a README file that explains what the project is for and provides information about how to install and run the program.

If you double click the file in the tree view, it will open for editing in the main pane. The file has a `.md` extension, which means it is intended to be written in **Markdown** a popular syntax for lightly styling text files. Markdown is ubiquitous on **Github** [and here is a useful guide to it](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet) For now though, let's just create a basic placeholder for information. 

Delete the contents of the file and replace them with the following:

```
Prototype Website
=================

Built by [Your names here]
```

Makre sure you save the file. Switch to the preview tab: has it been updated with your new content?

Introducing Ruby
---------------

uby is a programming language. It comes pre-installed on your Cloud9 workspace. To test this, go to the command line and type (don't include the `$`)

```
$ ruby -v
```
(...then hit return to enter it.) and you should see something like this:

```
ruby 2.3.0p0 (2015-12-25 revision 53290) [x86_64-darwin15]
```

> We'll use the `$` sign to represent the command line prompt and to differentiate commands you should enter from output you should see.

This tells us the currently installed version of Ruby (which we requested by passing the `-v` to the `ruby` command).

Writing a Ruby Program
----------------------

Create a file in your workspace called `hello.rb`. By convention, Ruby files have the extension `.rb`. The benefit of this convention is that Cloud9 will provide Ruby **syntax highlighting** for all files with the `.rb` extension.

Open the file in the editor and add the following content:

```ruby
puts 'Hello Ruby'
```

See how syntax highlighting works? The IDE recognises the Ruby language and uses colours to differentiate elements of the 'frammar'. You may see different colours depending on your chosen theme.

Save the file. Now go to the command line and enter the following: 

```
$ ruby hello.rb
```
This tells the Ruby engine to run the code in the `hello.rb` file. You should see the following output:
```
Hello Ruby
```
You've just written a command-line program: you run from the command line and it outputs to the command line!

[Previous section](./section0.md) | [Continue to Step 2](./section2.md)
