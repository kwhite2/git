# What are Git, GitHub and Markdown?

## What is Git? 

**Git** is software used for version control—that is, tracking the state of files and changes you make to them over time. Git can be enabled in a folder, and then used to save the state of the contents in that folder at different points in the future, as designated by you. In the language of Git, a folder is called a *repository*. In the context of this workshop, it refers to a folder that is being tracked by Git. Using Git, you can view a log of the changes you've made to the files in a repository and compare changes over time. You can also revert back to previous versions, and create branches of a project to explore different futures. Git is also useful for collaboration, as a repository can be shared across computers, and its contents can be asynchonously developed and eventually merged with the main project. 

## What is GitHub?

**GitHub** is a online platform for hosting Git repositories. It functions for some, predominantly programmers, as a social network for sharing and collaborating on code-based projects. Users can share their own projects, as well as search for others, which they can then often work on and contribute to. Digital Humanists, librarians, and other academics are also finding ways Git and GitHub are useful in writing projects and teaching. GitHub also serves as a web-hosting platform, allowing users to create websites from their repositories.

## What is Markdown?

Markdown is a markup language for formatting text. Like HTML, you add markers to plain text to style and organize the text of a document.

In HTML: 
```html
<h1>Heading 1</h1>
```

In Markdown:

```markdown
# Heading 1
```

Whereas you use HTML and CSS with WordPress, you use Markdown with Git and GitHub. Markdown has fewer options for marking text than HTML. It was designed to be human-readable, meaning easy to write and edit. 

This file you are reading is written in markdown—[here](https://raw.githubusercontent.com/DHRI-Curriculum/git/master/sections/concept.md) is what it looks like in its raw, unrendered form.

Compare that with this - the source code for the GitHub page, written in HTML [here](view-source:https://github.com/DHRI-Curriculum/git).

Markdown is also arguably more sustainable and accessible than formats like `.docx` because of its simplicity and related ability to be read across multiple platforms. Use of Markdown is also supported by document-conversion tools like [Pandoc](https://pandoc.org/) that can change a markdown file to an epub with one command entered into your terminal.

## Highlighting Distinctions

As we move forward its important to make sure we're firm on the distinctions between the three different tools outlined above. 

**Git** is a software that you use on your laptop, or your local computer/machine. The repository with your project's files is stored on your hard drive. You also edit the text files on your local machine using a plain text editor, which is another software on your local machine like VS Code. 

**GitHub** is a cloud-based platform that you access through your internet browser. Even though you physically are still in the same place, working on your laptop, you are no longer working on your local machine, you are on the Internet. This is a fundamentally different location than when you're working with your Git repository and editing and creating files in your plain text editor. With GitHub, you are uploading your repository - as described above - from your local machine to this platform on the Internet to be shared more broadly. You can also create private repositories if you want to use GitHub to backup a project.  

**Markdown** is the language used to format the plain text files in your Git-enabled repository. GitHub reads this language so that the markups made to the file are rendered when you view your file on the platform (i.e. #headers appears as headers, links are inserted).

## Evaluation
Which best describes Version Control:
- a software installed on my local machine
- a language for formatting plain text files
- the practice of tracking and organizing the state of a file over time, as it changes*
- a web-based plaform for storing and sharing files
- a language that can be read and rendered by some web-based platforms
- a version control software
- a cloud-based software
- refers to project folders as "repositories"

Which best describe Git:
- a software installed on my local machine*
- a language for formatting plain text files
- the practice of tracking and organizing the state of a file over time, as it changes
- a web-based plaform for storing and sharing files
- a language that can be read and rendered by some web-based platforms
- a version control software*
- a cloud-based software
- refers to project folders as "repositories"*

Which best describes GitHub:
- a software installed on my local machine
- a language for formatting plain text files
- the practice of tracking and organizing the state of a file over time, as it changes
- a web-based plaform for storing and sharing files*
- a language that can be read and rendered by some web-based platforms
- a version control software
- a cloud-based software*
- refers to project folders as "repositories"*

Which best describes Markdown:
- a software installed on my local machine
- a language for formatting plain text files*
- the practice of tracking and organizing the state of a file over time, as it changes
- a web-based plaform for storing and sharing files
- a language that can be read and rendered by some web-based platforms*
- a version control software
- a cloud-based software
- refers to project folders as "repositories"


# What You Can Do with Git and GitHub

A [study of how Digital Humanists use GitHub](https://digitalscholarship.files.wordpress.com/2016/07/spirosmithdh2016githubpresentationfinal.pdf), conducted by Lisa Spiro and Sean Morey Smith, found that a wide range of users, including professors, research staff, graduate students, IT staff, and librarians commonly used the site in their DH work. They used GitHub for a diverse range of activities, such as:

- Developing software
- Sharing data sets
- Creating websites
- Writing articles and books
- Collating online resources
- Keeping research notes
- Hosting syllabi and course materials

## Why Use GitHub?  
  
Participants in the study said they found GitHub useful in their Digital Humanities work for several reasons. In particular, it facilitated: 

- Sharing and backing up files on multiple computers
- Monitoring changes effectively
- Recovering from bugs or errors by going back in time before the error arose
- Using different branches for experiments and new directions
- Sharing and managing files with others—seeing who added what content and when

## How We Use GitHub:

### Sharing and Attribution

As you can see across these sessions, we use GitHub to host workshop curricula. Hosting sessions on GitHub allows you (and anyone else interested in these topics!) to follow our repositories, and create your own version of the workshop based on our materials. This fosters open scholarship and knowledge sharing. It also facilitates attribution and citation by clearly tracking which content was created by whom, when it was added, and which projects or materials are derived from others.

#### Case One: This Session

If you [go this to workshop on GitHub](https://github.com/DHRI-Curriculum/git/issues/45) and look at the top of the page just under the workshop title, `DHRI-Curriculum/git`, you can see it is `forked from pswee001/Git_DRI_Jan_2018` (next to the red star). That line shows that this particular repository is building on (*"forked from"*) the curriculum for a session I presented at our January 2018 Institute. If you then look at that repository, you will see that it is in turn forked from previous sessions that were developed by other GC Digital Fellows for workshops in past years. 

![Image of what attribution looks like in GitHub](images/attribution.png)

**Forking** is a proper function of the GitHub platform. It supports collaboration by allowing you to copy someone else's repository to your own account on GitHub while maintaining a trail of attribution and derivation. This function is described in further detail in the final lesson of this workshop.

### Collaborative Writing

Git is also used to track changes (*version control* in Git parlance) in writing projects, especially when there are multiple authors working asynchronously. It can be an alternative to using track changes in Microsoft Word, or comments and edits in a Google Doc.

#### Case Two: Coauthored Publications

Git and GitHub - together or independently - support multi-author publishing. Like we have done with the DHRI curriculum, you can have a shared project folder that multiple people are working from asynchronously, even on the same parts if they wanted, and then those different offshoots can be carefully folded back into the master project. This entails the process of creating *branches* and *merging*.

Git and GitHub also help with attribution by tracking individual contributions throughout. Additional branches could be created by a singular author as well, allowing the writer to explore different ways forward. The version control feature also allows authors to easily return to and compare older drafts or retrieve sections previoulsy discarded. 

**Branches** and **merging** are important functions when using Git to collaborate, but they are also advanced and thus beyond the scope of this workshop. See the *Resources* section at the end of the workshop for more information.

### Versions Across Time

How did you initially come by the syllabus you use for your class(es), and did you develop it over time? Many professors borrow and adapt from each other, and most of us probably update our syllabi each semester, even if only a little bit.

Through this process, many of us end up with a set of files that looks something like this:  

```
|
--Documents
   |
   --syllabus.doc
   --syllabus2.doc 
   --syllabusnew.doc 
   --syllabusRevised.doc 
   --syllabusFINAL.doc 
   --syllabus?.doc 
```

While I can tell which version is the "final" one, I can not see what was changed along the way or how the different versions vary from each other. 

With Git, you would save these multiple versions over time as one file, and each version you save includes a note about what has changed so you can easily revert back to an older version if needed. 

By looking at the file list, you also can not tell who the syllabus originally came from, or if there were contributions from many individuals. Git and GitHub can help make attribution clear, and maintain it over time as a the syllabus travels between hands.  

#### Case Three: Syllabi

Increasingly we see that faculty are sharing their syllabi on GitHub (example: [DLCL 204: Digital Humanities Across Borders](https://github.com/quinnanya/dlcl204)). Some are even using GitPages that apply a user-friendly interface to their repository to make it easier to access and navigate for their students (example: [Digital History](https://digitalhistory.github.io/)). 

GitHub offers a way of making a course publicly avaiable on the web, and sometimes easier or more intuitive to users than some learning management systems. Git helps track the changes over time. 

When the softwares are used together, Git and GitHub also support a collaborative appraoch to syllabi development. Copying another's project and modifying and remixing the content to meet your needs is a seamless and transparent process. Attribution of specific changes over time is a foundational function of how Git operates; GitHub explicitly renders attribution, making it easy to see who(s) did what. This is one of the attractions of using the platform. 

In a practical sense, you could search other syllabi on GitHub, and share yours so it could be searched by others. If someone finds a syllabus that includes parts they want to use, they could fork that syllabi to their GitHub account, and download - or *clone* as Git calls it - the files to your local machine and edit it there. Any changes could then be *pushed* back to the repository on GitHub, thereby sharing your amendments publicly. On GitHub, attribution of who contributed what are transparent. Meanwhile, your amended version would be available for others to fork and clone and amend and re-share. 

Even if you were only working with your own self-created syllabus, like we'll do later in this workshop, Git and GitHub can be useful for tracking your changes without the hassle of multiple files. From one file, you can use Git to compare your current version with older versions; you can also compare and share these different versions on GitHub if you wanted.

**Cloning** and **pushing** are proper functionalities of GitHub that describe how you communicate and share files between your local machine and the Internet. These are covered more in-depth in a later lesson in this workshop.

## Evaluation

What tasks could Git and/or GitHub offer support to?:
- Developing software*
- Creating and sharing data sets*
- Creating websites*
- Writing articles and books*
- Collating online resources*
- Keeping research notes*
- Hosting syllabi and course materials*

# Review of the Command Line

During this workshop, you'll be communicating with GitHub from our local machine via the command line (terminal, bash). This section reviews some of the basic commands that will also be used in this workshop.  

In addition to the command line, you'll be using your text editor and your browser. Before continuing, its important that we clearly distinguish between these three different spaces or environments:
- Your plain text editor where you'll be writing your syllabus in Markdown is on your local machine. 
- That syllabus is intiailly saved in a git-enabled repository on your local machine.
- Your browser is where you'll be uploading your repository to GitHub.
- Your terminal is where you'll be communicating with GitHub to send the repository and project files back and forth between the web and your hard drive. 

Because you'll be moving between these three spaces throughout the workshop, you may want to use (command + tab) or (ctrl + tab) to move quickly between the three windows on your desktop.

## Accessing the Terminal

### Mac OS

Press the space bar and the command key at the same time and type `terminal`. Press `Enter`.

### Windows

Press the Windows button on your keyboard. When the search menu pops up, type `git bash` and press `Enter`.

## Practice Navigating the Command Line

In this session, we will be making a syllabus and using Git to keep track of our revisions. Let's create a Git project folder.

You can create the folder anywhere on your hard drive by typing the following into your terminal and hitting `Enter`.  

```sh
$ cd <directory-name> 
```

Let's practice this command by using it to take us to our Desktop. Type the following command into your terminal and hit `Enter`. 

```sh
$ cd Desktop
```

This will change your current working directory from `/Users/<your-name>` to `/Users/<your-name>/Desktop`.

Check your current directory by typing the following command into your terminal and hit enter:

```sh
$ pwd
```	

Now, use the following command to go up one directory:

```sh
$ cd ..
```	

Check your current directory again using the following command. You should be back in your home directory:

```sh
$ pwd
```

Practice going back and forth between your Desktop and your home directory.

When finished, go to your Desktop folder and check that you're there with `pwd`.

## Making a Git Project Folder

If you've worked through the command line session, you should see a `projects` folder on your desktop. Navigate into it using the following command: 

```sh
$ cd projects
```

If you don't have a projects folder on your desktop, create one using the following command: 

```sh
$ mkdir projects
```

From `Desktop`, navigate into your `projects` folder. Then create a `git-practice` folder with the following command:

```sh
$ mkdir git-practice
```

Navigate into the new `git` folder using the following command: 

```sh
$ cd git-practice
```

At this point, when you type `pwd`, your folder structure should look like this:

```
/home/<username>/Desktop/projects/git-practice
```

##Evaluation

Which best describes where you are working when you're writing Markdown in your plain text editor: 
- on my local machine*
- on the internet

Which best describes where you are working when you're using your terminal to communicate with GitHub and share the files: 
- on my local machine*
- on the internet

Which best describes where you are working when you are viewing your files in GitHub: 
- on my local machine*
- on the internet*

Git-enabled repository it means 
- none of the files on my local machine are being tracked
- a specific file on my local machine is being tracked
- a specific folder on my local machine is being tracked*
- all the files on my local machine are being tracked

Which command do you use to make a new folder?
- pwd
- cd
- mkdir*

Which command do you use to enter into a folder?
- pwd
- cd*
- mkdir

Which command do you use to check where you are?
- pwd*
- cd
- mkdir

# Setting Up Git

Our first step in working with Git is letting the software know who we are so it can track our work and attribute our contributions. Through this section, you'll be checking your installation and configuring Git with your own name and information.

## Check Your Install

Let's make sure Git has been successfully installed. In your terminal, type the following command:

```sh
$ git --version
```

If you see a version number, you're all set. If not, click [here](http://git-scm.com/downloads) and install as you would any other software on your system.

## Configuring Git on Your Computer

Next, let's configure git so that it can identify who we are. This information is useful because it connects identifying information with the changes you make in your repository. 

Type the following into your command line, replacing the "John Doe" and johndoe@example.com with your name and email (use quotations where you see them). This does not necessarily need to be the name and email you used to sign up for GitHub. Remember, these are different spaces and different softwares.

```sh
$ git config --global user.name "John Doe"
$ git config --global user.email johndoe@example.com
```

To check your set-up, type the following command into your terminal:

```sh
$ git config --list
```

You should get something that looks like this except with whatever information you entered previously:

```
user.name=Superstar Git User
user.email=gitsuperstar@gmail.com
```

## Evaluation

What are you doing when you set up git?
- You are creating a new version of the software on your local machine.
- You are sending files from your local machnine to GitHub?
- You are introducing yourself to the software, so it knows who you are.*
- You are creating a new version of a project folder on your local machine. 

# Creating a Syllabus with Markdown

The next step is to **initialize** the project folder that we want Git to track. When we initialize a folder, we are telling Git to pay attention to it. This only needs to happen once because what is actually happening through this process is Git is adding a hidden subfolder within your folder that houses the internal data structure required for version control. 

First, use `cd`, navigate to the `git-practice` folder inside `projects`. From your home directory, type the following command into your terminal:

```sh
$ cd Desktop/projects/git-practice
```

Next we're going to **initialize** our repository using the following command:

```sh
$ git init
```

You should see output like this:

```
Initialized empty Git repository in /home/patrick/projects/git/.git/
```

Now Git is tracking our directory. However, it has not done any versioning yet. This is because 1) we haven't told Git to take a snapshot yet, and 2) there are no files in the folder to take a snapshot of. For now, Git knows this folder exists and is prepared to take a snapshot of the files when you tell it to.

Before version control is useful, we'll have to create a text file for Git to track. For this session, the file we will track will be a course syllabus—we'll create that next.

### Creating a Syllabus in Markdown

To create a plain text file, we're going to switch to our text editor, VS Code, to create and edit a file named `syllabus.md` and save it to our 'git-practice' folder. 

If you have not installed VS Code, review [the installation instructions here](https://github.com/DHRI-Curriculum/install/blob/master/sections/vscode.md).

In terminal, check to make sure you are in your `git-practice` folder. (HINT: use 'pwd' to see what directory you are currently in) Next, type:

```sh
$ code syllabus.md
```

to open a `syllabus.md` file in VS Code. You should see a window appear that looks similar to this:

![Image of what VS Code looks like when opening the syllabus.md file](images/vscode1.png)

If VS Code does not open when you use the `code` command in your terminal, open it using the Start Menu on Windows or Spotlight Search on Mac OS as you would any other software. Then click `File > Open File` and use the dialog to navigate to the `/Users/<your-name>/Desktop/projects/git` folder and create a `syllabus.md` file there.

We'll be typing our markdown into this file in the VS Code window. At any time, you can save your file by hitting `Control-s` on Windows or `⌘-s` on Mac OS. Alternatively, you can click the `File` menu on the top right, then select `Save` from the dropdown menu.

Saving frequently is advised. When we get to the version contol functionality of Git, only changes that are saved will be preserved when a version is created. 

## Using Markdown

We'll be using markdown to write a syllabus, and then using Git to track any changes we make to it. Markdown allows us to format textual features like headings, emphasis, links, and lists in a plain text file using a streamlined set of notations that humans can interpret without much training. Markdown files usually have a `.md` extension.

In markdown, we insert headings with a single hash mark like this:

```markdown
# My Syllabus Heading
```

A sub-heading (H2) heading uses two hash marks like this:

```markdown
## Readings
```

To provide emphasis, place asterisks around some text:

```markdown
*This text will appear italicized.*
**This text will appear bold.**
```

For emphasis, you need to mark where it should start and where it should end, so you need astrisks at the beginning and end of whatever text is being emphasized.

To create a bulleted list, put a hyphen at the beginning of each list item:

```markdown
- Reading one
- Reading two
- Reading three
```

To create a link, put the anchor text (the text you will see) in square brackets and the URL in parentheses. Don't put a space between them:

```markdown
I teach at [The Graduate Center, CUNY](https://www.gc.cuny.edu).
```

Paragraphs of text are denoted by putting a blank line between them:

```
This is a paragraph in markdown. It's separated from the paragraph below with a blank line. If you know HTML, it's kind of like the \<p> tag. That means that there is a little space before and after the paragraph when it is rendered.

This is a second paragraph in markdown, which I'll use to tell you what I like about markdown. I like markdown because it looks pretty good, if minimal, whether you're looking at the rendered or unrendered version. It's like tidy HTML.
```

## Challenge
Use these five elements—headings, emphasis, lists, links, and paragraphs—to create a syllabus. Have a main heading that gives the course title (one `#`), then subheadings for, at least, course info and readings. Use emphasis (`*`) for book titles and try to get a list in there somewhere.

## Example

You can look at an example syllabus in raw text form [here](https://raw.githubusercontent.com/DHRI-Curriculum/git/master/sections/syllabus.md). When it's rendered by GitHub, it looks like [this](https://github.com/DHRI-Curriculum/git/blob/master/sections/syllabus.md). When editing the markdown file in VS Code, it might look like this:

![What your markdown might look like when typed into VS Code](images/vscode2.png)

## Tips:

**1)** VS Code also has a preview feature for your markdown. Hit the preview button on the top right while editing your markdown file:

![Button to hit to get a preview in VS Code](images/vscode3.png)

You'll get two side-by-side panels. Your markdown file will be on the left, and your rendered preview will be on the right:

![Side by side markdown and preview in VS Code](images/vscode4.png)

**2)** Remember to save your work with `Control-s` on Windows or `⌘-s` on Mac OS.

## Evaluaton

Which best describes what you're doing when you initialize your project folder: 
- You created a new version of your project folder
- You told Git to pay attention to your project folder*
- You told Git to set up its file structure within your project folder so it can track changes to your files.* 
- You use the command `mkdir` in your terminal
- You use the command `git init` in your terminal*


# Staging and Committing Changes

Git's primary function is version control, or to track a project as it exists at different points in time. Now that we have a file to track—our markdown syllabus—let's use Git to save the current state of the repository as it exists now.

## A Metaphor for Adding and Committing

In Git, a **commit** is a snapshot of a repository that is entered into its permanent history. To commit a change to a repository, we take two steps:

1. Adding files to a "staging area," meaning that we intend to commit them. 
2. Finalizing the commit.

Staging a file or files is you telling Git, "Hey! Pay attention these files and the changes in them".

Making a commit is a lot like taking a photo. First, you have to decide who will be in the photo and arrange your friends or family in front of the camera (the staging process). Once everyone is present and ready, you take the picture, entering that moment into the permanent record (the commit process).

## Staging Changes with the Add Command

First, let's see what state Git is currently in. It's a good idea to use this command before and after doing anything in Git so you can always be on the same page as the computer.

Make sure you're in your `/home/<your-name>/Desktop/projects/git-practice` directory using the `pwd` command in the terminal. Once you're there, enter this command:

```sh
$ git status
```

You should see output like this:

```
On branch master

No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be committed)

	syllabus.md

nothing added to commit but untracked files present (use "git add" to track)
```

This means we've initialized our repository, but haven't made any commits yet. If you're instead getting a message that begins with the word `fatal` when you use `git status`, you may be in the wrong directory or perhaps you haven't run the `git init` command on your directory yet.

Let's follow the recommendation in the status message above and use the `add` command to stage files, making them ready to be committed.

Type this command:

```sh
$ git add syllabus.md
```

You should see no output from the command line, meaning that the above command succeeded. Let's run `git status` again to check if things have changed. You should see output like this:

```
On branch master

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)

	new file:   syllabus.md
```

The `new file:   syllabus.md` should be highlighted in green to show that it's ready for commit. 

This is Git telling you, "Ok, I see the file(s) you're talking about." 

## Committing Changes

Now that our files have been staged, let's commit them, making them part of the permanent record of the repository. Type:

```sh
$ git commit -m "Initial commit of syllabus file"
```

The `-m` flag provides a message along with the commit that will tell others—or remind a future version of yourself—what the commit was all about. Try not to type `git commit` without the `-m` flag—there's a note about this below.

After running the command, you should see output like this:

```
[master (root-commit) 8bb8306] Initial commit of syllabus file
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 syllabus.md
```

This means you have successfully made your first commit in the repository—congratulations!

Let's check the state of our repository after the commit with `git status`:

```
On branch master
nothing to commit, working tree clean
```

This means that everything in the repository is successfully committed and up-to-date. If you edit your syllabus file or create a new file in the repository, the message you get with `git status` will instead list files that have uncommitted changes.

Let's run one other command to see the effect our commit has had. Enter this command:

```sh
$ git log
```

You should see output similar to this:

```
commit 8bb8306c1392eed52d4407eb16867a49b49a46ac (HEAD -> master)
Author: Patrick Smyth <patricksmyth01@gmail.com>
Date:   Sun May 20 16:03:39 2018 -0400

    Initial commit of syllabus file
```

This is the log of commits, comprising a history of your repository. There's only one commit here now, though. If you don't see a prompt (the `$`) after running `git log`, you may need to press the `q` key (just the `q` key by itself) to return to the command line.

## Why Do We Need to Use the -m Flag?

The -m flag is useful for human purposes and technical purposes. For human purposes, the -m flag helps you keep track of the changes you're making. Version control is most useful when you can confidently return to a specific version. It can also help you be more structured in your approach to making changes - your notes to self are limited, so to make them clear you might make commits after specific tasks are completed, such as update readings for week 1 or added S.Noble reading. This can also make it easier to reverse a specific change in the future. 

Also, if you type `git commit` by itself, git will open the command line's default text editor to allow you to enter the commit message. Unfortunately, the default text editor, `vi`, requires some knowledge to use, and we don't teach it as part of our sessions.

If you find yourself stuck in an unfamiliar screen in the command line after running `git commit`, you're probably in `vi`. Type this to leave that environment and return to the `$` prompt:

```
:q
```

If you're ever stuck or "trapped" on the command line, try running through these common exit commands to return to the prompt:

```
Control-c
Control-d
q
:q
```

`Control-c` attempts to abort the current task and restore user control. `Control-d` escapes the current shell environment—if you use it at the normal `$` prompt, it will end the current command line session. `q` is used to escape from specific utilities like `less`. `:q` first changes the mode in `vi`, allowing you to enter the `q` key to quit, so it's a command specific to `vi`.

##Evaluation
Which best describe the process of Staging:
- you telling Git to take a snapshot of changes made to a file.
- you telling Git which files with changes you want it to pay attention to.*
- you telling git to pay attention to a folder storing files you want to make changes to.
- the second part of a two-step process.

Which best describes the process of Committing: 
- you telling Git to take a snapshot of changes made to a file.*
- you telling Git which files with changes you want it to pay attention to.
- you telling git to pay attention to a folder storing files you want to make changes to.
- the second part of a two-step process.*

What happens if you Stage the files, but don't Commit them?
- Git won't know what files you want to take a snapshot of
- Git won't take a snapshot of the files.* 
- Git will take the snapshot of the files
- You will have told Git what files you would like it to take a snapshot of.*

What happens if you Commit the files, but don't Stage them? 
- Git won't know what files you want to take a snapshot of*
- Git won't take a snapshot of the files.* 
- You will have told Git what files you would like it to take a snapshot of.
- Git will take the snapshot of the files*

Which best describes the -m flag used when committing changes to a file?
- a brief description of changes you made to your file*
- Its just something Git needs so it doesn't break
- future aids when you are trying to make sense of or recover changes you previously made to a file*
- It's nonsense - who needs it?!

# Pushing to GitHub

Now, you may want to backup or share that file on the Internet. Let's connect the directory you made on your local machine to GitHub, on the web. 

Remember, GitHub is a service that allows you to host files, collaborate, and find the work of others. Once our syllabus is on GitHub, it will be publicly visible. Note that repositories on GitHub can also be private.

Go to GitHub in your browser and click the plus sign in the upper right hand corner.

![You can find the plus sign button to add a repo on the top right of github](images/addrepo.png)

After clicking the plus button, select `New repository` from the dropdown menu.

![The dropdown menu where you select New Repository](images/createrepo.png)

After clicking `New repository`, you'll have to enter some information, including a name and description for your repository.

![Screen on GitHub where you enter your repository information](images/createrepo2.png)

- Choose a name, such as `git-practice`.
- Enter a description, such as `Test syllabus for learning Git and GitHub`.
- Keep the `Public — Anyone can see this repository` selector checked.
- Do *not* select `Initialize this repository with a README` since you will be importing an existing repository from your computer.
- Click `Create repository`.

You should end up inside your newly created git-practice repo. It will look like a set of instructions that you might want to use to connect your GitHub repository to a local repository.

The instructions we want consist of two lines underneath the heading `...or push an existing repository from the command line`. The hand in this screenshot points to where these directions are on the page:

![The commands you need to copy from the new repo page on GitHub](images/connect-repo.png)

Copy out the first command and paste it in your terminal. It should look something like this:

```sh
$ git remote add origin git@github.com:<username>/<repository-name>.git
```

You'll need the command copied from your new repo, since it will contain the correct URL.

Next, paste the second command. It will look exactly like this:

```sh
$ git push -u origin master
```

After running this command, you should see output that looks like this:

```
Total 4 (delta 3), reused 0 (delta 0)
remote: Resolving deltas: 100% (3/3), completed with 3 local objects.
To github.com:<repo-name>/git.git
   916998f..9779fa7  master -> master
```

If you see output like this, go back to your new repository page in the browser and click the `Refresh` button. You should see your `syllabus.md` file on GitHub!

## Review

We have covered the basic steps of creating a file and tracking changes within a file on your local machine and on GitHub. 

This has involved coordinating across three different environments, so let's go through that one more time. Note that this process is very slightly different. I'll highlight it when it comes up. 

To start, let's add something to our syllabus. Another week of materials or a new reading. 

Save that file. 

Use `git add` via the command line to stage the file--tell Git what document you want it to pay attention to. 

Use `git commit` via the command line to save the changes you've just made as a snapshot or new version of you file. Remember to use the -m flag and include a message about the change you just made. 

So far, we have not done anything with GitHub or on the Internet. We have used Git, installed on our local machine, to save a version of file as it stands now. We could stop here if we only had an interest in using Git for version control. But if we also wanted to use GitHub to back up our files, or to share our project with a team or publicly, we want to upload, or push, that repository to GitHub on the Internet. 

Use `git push origin master` to push that file to your repository on GitHub. After refreshing the webpage, your file should appear online. **The difference I noted above appears here.** Note the absense of the `-u` flag from the command. That flag was used the first time to establish the connection between the repository on your local machine and on GitHub. Now that that connection has been established, that flag is not needed.   

## Challenges 

**1)** Go through the process a few more times by adding additional readings and weeks of course material. Remember to commit changes intentionally so your commit messages make sense. Use `git log` to review your changes. 

**2)** Also try creating a new file and adding an assignment. Rewrite the assignment using Markdown, or edit and add in the markers. Go through the process of staging and commiting that file, and pushing it to your repository on GitHub. 

**3** Test your understanding by thinking through the following questions:
- Do you need to push the file to GitHub each time you commit changes to the file, or can you make several commits to a file and push them all to GitHub at once? 
- Do you need to use `git init` after after adding a new assignment file to your folder? 
- What about the -u flag in the git push origin master? Does this flag need to be used to add the assignment to your repository on GitHub?

## Solution

In response to **Challenge 3**: 
- No, you don't need to push to GitHub every time, or at all even, if you didn't want to share your changes publicly. Git is the software that tracks the changes, and you review them on your local machine using Git as well. 
- No, you don't need to initialize the folder after adding a new file for an assignment or otherwise. In this case, we've already initialized the process; Git is tracking the folder. After the file is added, we just need to notify Git to take a snapshot of the additions and changes using the `git add`, `git commit` sequence. We can also use `git push` to share those changes on GitHub. 
- No, the -u fly does not need to be used again. This flag is only necessary when setting up the original connection between the folder on your local machine and the folder on GitHub. 

## Evaluation

Which best describes what you're doing when you use the command 'git push'
- you telling Git to take a snapshot of changes made to a file.*
- you telling Git which files with changes you want it to pay attention to.
- you telling git to pay attention to a folder storing files you want to make changes to.
- you are copying the updated files with the changes to the repository on GitHub*
- the second part of a two-step process.*

How does the process of pushing differ from the processes of staging and committing discussed in the previous lesson?
- There is no fundamental difference between these processes. 
- Staging and Committing set up the files whereas pushing is the act of taking the snapshot.
- Staging and committing the files is to communicate with GitHub on the Internet, pushing the changes happens on your local machine. 
- Staging and committing the files happens on your local machine, pushing the changes is to communicate with GitHub on the Internet. 


What happens if you use git push without staging and committing files?
- Git won't know what files you want to take a snapshot of.*
- Git won't take a snapshot of the files.*
- Your computer won't know what changes to share with GitHub.*
- Git will take the snapshot of the files
- You will have successfully created a new version of the file.
- You will have communicated with GitHub and shared a copy of the updated files.
- You will have communicated with GitHub to copy a set of files from their servers to your local machine.

What happens if you stage and commit files, but not push the changes?
- Git won't know what files you want to take a snapshot of.
- Git won't take a snapshot of the files.
- Your computer won't know what changes to share with GitHub.
- Git will take the snapshot of the files*
- You will have successfully created a new version of the file.*
- You will have communicated with GitHub and shared a copy of the updated files.
- You will have communicated with GitHub to copy a set of files from their servers to your local machine.

# Cloning & Forking

GitHub was built for sharing and collaborating on projects. A key advantage of the platform is that you can find lots of bits of software that do many different things--such as code for plugins for WordPress or Leaflet. Increasingly, you might find syllabi or open writing projects. If a project is public, you can save a copy of it to your local machine, work on it, save your admendations and share it on your own GitHub account. Like we've already mentioned, GitHub usefully helps track attribution along the way.

Cloning and forking are the basic functions of this capability. Each are first explained below, and followed by an example and activity to further explain. 

## Cloning

**Cloning** a repository means making a copy of a repository on GitHub, to download and work on locally--on your local machine. By entering the following code into your terminal, you can clone any public directory on GitHub: 

```sh
$ git clone <repository-url>
```

When you clone a repository from GitHub, the folder that shows up on your local machine comes built-in with a few things. First, Git is already present, so you don't need to initialize the folder. Also, the connection between your local copy and the online repository is already made, so `git push origin master` will work (no -u flag needed). 

For practice, let's clone the repository for this workshop about Git and GitHub.

First, let's navigate back to your Desktop folder.

```sh
$ cd ~/Desktop
```

Remember that the ~ refers to your home directory. Now let's find the URL we need to clone the lesson.

First, follow [this link to the main page of this lesson on Git and GitHub](https://github.com/DHRI-Curriculum/git).

On the main page, there should be a green `Clone or download` button on the right side:

![Image pointing out where the clone or download button is on GitHub](images/clone.png)

Click the green button and you will see a box with highlighted text under a heading that says `Clone with HTTPS`. If you instead see `Cloning with SSH`, click the small link that says `Use HTTPS`.

Now copy out the text in the box:

![Image showing where the text you need to copy is located](images/copy-clone-text.png)

Now that you have the text copied, go back to your terminal. Remember, you should be on the desktop.

Type

```sh
$ git clone <copied-url>
```

If the command is successful, the full Git lesson will be replicated on your local machine. You can type

```sh
$ cd git
```

to enter the lesson folder, since the lesson repository is simply called `git`. Use the `ls` command to take a look at the various files in the lesson folder.

Cloning can be especially useful when you're joining a group project that is hosted on GitHub, and you want your changes to eventually be pushed and shared with that same repository. 

But maybe that is not possible or ideal. Maybe you don't want to contribute your changes to someone else's repository. Maybe you want to make a derivative of their folder for yourself, on your GitHub account, and make changes there.

Forking is the step you could take before cloning to do this.

## Forking

**Forking** a repository means making a copy of someone else's repository on GitHub, and saving it to your account on GitHub. This function happens within GitHub, and has nothing to do with what is happening on your local machine. 

For example, go to [the repository for this workshop](https://github.com/DHRI-Curriculum/git) on GitHub. Note the `Fork` button in the upper right hand corner. By clicking that button, you can copy, or fork, this repository to your account. 

![Image showing where the button to fork a repo is located](images/fork-button.jpeg)

Doing so would also adjust the attribution information in the upper left hand corner. Your username would replace `DHRI-Curriculum`, showing that you are looking at a copy of the repository on your account now. Additionally, it will reference the origin account, in this case, `DHRI-Curriculum` below after `forked from`.

![Image showing the changes in attribution that happen when a repo is forked](images/forking-attrib-chng.jpeg)

Your local machine would come into play when you want to **clone** that repository so you can work on it locally. This also means that when you push those changes to GitHub, you would be pushing them to a forked repository associated with your own account. 

You might use this method if you were going to teach your own Git & GitHub workshop. You could use our repository as a base for getting started, and add more examples or change some language, clarify something further, or create a connection to another workshop you are giving, etc. This allows us to continue to use the workshop as we have it as well. Also, maybe at a later time, we want to merge some of your changes with ours. We can do that too by revisiting your version history. 

## Challenge

1. Fork and clone [the repository for this workshop](https://github.com/DHRI-Curriculum/git). Note not only *what* you are doing, but also *where* you are working when completing these two different tasks.
2. Make changes to the files on your local machine. Remember to save them!
3. Use the 3-step process of stage, commit and push to return the amended files to the repository on GitHub. 

## Solution

Rather than write out the solution here, I want to encourage you to go back through the lessons as needed. 

You'll know you've completed step one when the project folder shows up on your local machine. 

After you've made and saved the changes, you'll know you've completed step three when your changes appear in the project folder on GitHub. 

## Evaluation

Which best describes cloning?
- copying a repository from GitHub to your local machine.*
- copying a repository from your local machince to GitHub
- copying a repository from someone else's GitHub account to your own
- copying a repository from your account to someone else's account

Which best describes forking
- copying a repository from GitHub to your local machine. 
- copying a repository from your local machince to GitHub
- copying a repository from someone else's GitHub account to your own*
- copying a repository from your account to someone else's account
