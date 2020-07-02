# What are Git, GitHub and Markdown?

## What is Git? 

**Git** is software used for version control—that is, tracking the state of files. Git can be enabled in a folder, and then used to save the state of the contents in that folder at different points in the future designated by you. In the language of Git, a folder is called a *repository*; in the context of this workshop, it refers to anfolder that is being tracked by Git. Using Git, you can view a log of the changes you've made to the files in a repository and compare changes over time. You can also revert back to previous versions, and create branches of a projects to explore different futures. Git is also useful for collaboration, as a repository can be shared across computers, and its contents can be asynchonously developed and eventually, and maybe partially merged with the main project. 

## What is GitHub?

**GitHub** is a online platform for hosting Git repositories.It functions for some, predominantly programmers, as a social network for sharing and collaborating on code-based projects. Users can share their own projects, as well as search for others, which they could then also work on and contribute to in many instances. Digital Humanists, Librarians, and other academics are also finding ways Git and GitHub are useful in writing projects and teaching. GitHub also serves as a web-hosting platform, allowing users to create websites from their repositories.

## What is Markdown?

Markdown is a markup language for formatting text. Like HTML, you add markers to plain text to style and organize the text of a document.

```
In HTML: 
<h1> Heading 1 </h1>

In Markdown
# Heading 1
```

Whereas you use HTML and CSS with WordPress, you use Markdown with GitHub. Markdown has fewer options for marking text than HTML. It was designed to be human-readable, meaning easy to write and edit. 

You'll notice this file is written in markdown—[here](https://raw.githubusercontent.com/DHRI-Curriculum/git/master/sections/concept.md) is what it looks like in its raw, unrendered form.

Compare that with this, showing the source code for the GitHub page, written in HTML: view-source:https://github.com/DHRI-Curriculum/git

It's also arguably more sustainable and accessible than formats like `.docx` because of its simplicity and related ability to be read across multiple platforms. Use is also supported by document-conversion tools like [Pandoc](https://pandoc.org/) that can change a markdown file to an epub with one command entered into your terminal.

## Highlighting Distinctions

As we move forward its important to make sure we're firm on the distinctions between the three different tools outlined above. 

**Git** is a software that you use on your laptop, or your local computer/machine. The repository with your project's files is stored on your harddrive. You also edit the text files on your local machine using a plain text editor, which is another software on your local machine like VS Code. 

**GitHub** is a cloud-based platform that you access through your internet browser. Even though you physically are still in the same place, working on your laptop, you are no longer working on your local machine, you are on the Internet. This is a fundamentally different location than when you're working with your Git repository and editing and creating files in your plain text editor. With GitHub, you are uploading your repository - as described above - to this platform to be shared more broadly. You can also create private repositories if you want to use GitHub to backup a project.  

**Markdown** is the language used to format the plain text files in your Git-enabled repository. GitHub reads this language so your markups to the file are rendered when you view your file on the platform (i.e. #headers appears as headers, links are inserted).

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

If you look just under the workshop title, `DHRI-Curriculum/git` at the top of this page, you can see it is `forked from pswee001/Git_DRI_Jan_2018`. That line shows that this particular repository is building on ("forked from"*) the curriculum for a session I presented at our January 2018 Institute. If you then look at that repository, you will see that it is in turn forked from previous sessions that were developed by other GC Digital Fellows for workshops in past years. 

*Forking* is a proper function of GitHub. It supports collaboration by maintaining a trail of attribution and derivation.

### Collaborative Writing

Git is also used to track changes (*version control* in Git parlance) in writing projects, especially when there are multiple authors working asynchronously. It can be an alternative to using track changes in Microsoft Word, or comments and edits in a Google Doc.

#### Case Two: Coauthored Publications

Git and GitHub - together or independently - support multi-author publishing. Like we have done with the DHRI curriculum, you can have a shared project folder that multiple people are working from asynchronously, even on the same parts if they wanted, and then those different offshoots can be carefully folded back into the master project. These are the process of creating branches, and merging. Git and GitHub also help with attribution by tracking individual contributions throughout. Additional branches could be created by a singular author as well, allowing the writer to explore different ways forward. The version control feature also allows authors to easily return to and compare older drafts or retrieve sections previoulsy discarded. 

### Versions Across Time

How do you come by and develop your syllabi over time? Many of us borrow and adapt from each other, and most of us probably update our syllabi each semester, even if only a little bit.

Put your hand up if you have  a folder somewhere that looks something like this. Or even multiple folders. 

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

Put your other hand up if you can't remember who you initially got this syllabus from. Do you know if there were other contributors befor them? 

#### Case Three: Syllabi

Increasingly we see that faculty are sharing their syllabi on GitHub. Some are even using GitPages that apply a user-friendly interface to their repository to make it easier to access and navigate for their students. Using Git and GitHub, you could fork that syllabi to your account, and download - or clone as Git calls is - it to your local machine to edit. After making changes to the files and pushing them to your repo on GitHub, someone else could compare the changes you made, and fork your version, or return to the original and fork from there. Both Git and GitHub help with attribution here; tracking who changes and adds what is a key feature of both tools.

Even if you were only working with your own self-created syllabus, like we'll do later in this workshop, Git and GitHub can be useful for tracking your changes without the hassle of multiple files. From one file, you can use Git to compare your current version with older versions; you can also compare and share these different versions on GitHub.

# Review of the Command Line

During this workshop, you'll be communicating with GitHub from our local machine via the command line (terminal, bash). It will be useful if you've taken [the Command Line Workshop](https://github.com/DHRI-Curriculum/command-line) before continuing. This section reviews some of the basic commands that will also be used in this workshop.  

In addition to the command line, you'll be using your text editor and your browser. Before continuing, its important that we clearly distinguish between these three different spaces or environments:
- your plain text editor where you'll be writing your syllabus in markdown, which will be saved in the git-enabled repository on your local machine,
- your browser, where you'll be uploading your repository to GitHub
- your terminal where you'll be communicating with GitHub to send the repository and project files back and forth between the web to your hard drive. 

Because you'll be moving between these three spaces throughout the workshop, you may want to use (command + tab) or (ctrl + tab) to move quickly between the three windows on your desktop.

## Accessing the Terminal

### Mac OS

Press the space bar and the command key at the same time and type `terminal`. Press `Enter`.

### Windows

Press the Windows button on your keyboard. When the search menu pops up, type `git bash` and press `Enter`.

## Practice Navigating the Command Line

In this session, we will be making a syllabus and using Git to keep track of our revisions. Let's create a Git project folder

	cd <directory-name> 
	
will let you navigate inside a directory of your choosing.

Type 

	cd Desktop
	
and hit `Enter`. This will change your current working directory from `/Users/<your-name>` to `/Users/<your-name>/Desktop`.

To check your current directory, type

	pwd
	
Try this now to make sure you're in your Desktop directory.

Now, use 

	cd ..
	
to go up one directory. In this case, this will take you back to your home directory.

Practice going back and forth between your Desktop and your home directory.

When finished, go to your Desktop folder and check that you're there with `pwd`.

## Making a Git Project Folder

If you've worked through the command line session, you should see a `projects` folder on your desktop. Navigate into it with

	cd projects
	
If you don't have a projects folder on your desktop, create one with

	mkdir projects

From `Desktop`, navigate into your `projects` folder. Then create a `git-practice` folder with the below command:

	mkdir git-practice

Enter the new `git` folder with

	cd git-practice

At this point, when you type `pwd`, your folder structure should look like this:

	/home/<username>/Desktop/projects/git-practice

# Setting Up Git

Our first step in working with Git is letting the software know who we are so it can track our work and attribute our contributions. Through this section, you'll be checking your installation and configuring Git with your own name and information.

## Check Your Install

Let's make sure Git has been successfully installed. In your terminal, type

	git --version

If you see a version number, you're all set. If not, click [here](http://git-scm.com/downloads) and install as you would any other software on your system.

## Configuring Git on Your Computer

Next, let's configure git so that it can identify who we are. This information is useful because it connects identifying information with the changes you make in your repository. 

Type the following into your command line, filling in the sections—below labelled "John Doe"—for your name and email (use quotations where you see them). This does not necessarily need to be the name and email you used to sign up for GitHub. Remember, these are different spaces and softwares.

	git config --global user.name "John Doe"
	git config --global user.email johndoe@example.com

To check your set-up, use:

	git config --list

You'll get something that looks like this:

	user.name=Superstar Git User
	user.email=gitsuperstar@gmail.com

# Creating a Syllabus with Markdown

Using `cd`, navigate to the `git-practice` folder inside `projects`. From your home directory, type:

	cd Desktop/projects/git-practice

Now we're going to **initialize** our repository, which means telling Git to pay attention to it:

	git init

You should see output like this:

	Initialized empty Git repository in /home/patrick/projects/git/.git/
	
Now Git is tracking our directory. Importantly, it has not done any versioning yet. There is no history of changes as of yet: 1) because there are no files and we haven't made any changes, 2) becuase we have to tell Git when to take a snapshot, which we go through in the next section. For now, Git knows this folder exists and is prepared to take a snapshot of the files when you tel it to.

Before version control useful, we'll have to create a text file for Git to track. For this session, the file we'll track will be a course syllabus—we'll create that next.

### Creating a Syllabus in Markdown

To create a plain text file, we're going to switch to our text editor, VS Code, to create and edit a file named `syllabus.md` and save it to our 'git-practice' folder. If you have not installed VS Code, review [the installation instructions here](https://github.com/DHRI-Curriculum/install/blob/master/sections/vscode.md).

In terminal, check to make sure you are in your `git-practice` folder. (HINT: use 'pwd' to see what directory you are currently in) Next, type:

	code syllabus.md
	
to open a `syllabus.md` file in VS Code. You should see a window appear that looks similar to this:

![Image of what VS Code looks like when opening the syllabus.md file](../images/vscode1.png)

If VS Code does not open when you use the `code` command in your terminal, open it using the Start Menu on Windows or Spotlight Search on Mac OS as you would any other software. Then click `File > Open File` and use the dialog to navigate to the `/Users/<your-name>/Desktop/projects/git` folder and create a `syllabus.md` file there.

We'll be typing our markdown into this file in the VS Code window. At any time, you can save your file by hitting `Control-s` on Windows or `⌘-s` on Mac OS. Alternatively, you can click the `File` menu on the top right, then select `Save` from the dropdown menu.

Saving frequently is advised. When we get to the version contol functionality of Git, only changes that are saved will be preserved when a version is created. 

## Using Markdown

We'll be using markdown to write a syllabus, and then using Git to track any changes we make to it. Markdown allows us to format textual features like headings, emphasis, links, and lists in a plain text file using a streamlined set of notations that humans can interpret without much training. Markdown files usually have a `.md` extension.

In markdown, we insert headings with a single hash mark like this:
```
	# My Syllabus Heading
```	
A sub-heading (H2) heading uses two hash marks like this:
```
	## Readings
```	
To provide emphasis, place asterisks around some text:
```
	*This text will appear italicized.*
	**This text will appear bold.**
```
For emphasis, you need to mark where it should start and where it should end, so you need astrisks at the beginning and end of whatever text is being emphasized.

To create a bulleted list, put a hyphen at the beginning of each list item:
```
	- Reading one
	- Reading two
	- Reading three
```	
To create a link, put the anchor text (the text you will see) in square brackets and the URL in parentheses. Don't put a space between them:
```
	I teach at [The Graduate Center, CUNY](https://www.gc.cuny.edu).
```	
Paragraphs of text are denoted by putting a blank line between them:
```
> This is a paragraph in markdown. It's separated from the paragraph below with a blank line. If you know HTML, it's kind of like the \<p> tag. That means that there is a little space before and after the paragraph when it is rendered.
> 
> This is a second paragraph in markdown, which I'll use to tell you what I like about markdown. I like markdown because it looks pretty good, if minimal, whether you're looking at the rendered or unrendered version. It's like tidy HTML.
```

Try using these five elements—headings, emphasis, lists, links, and paragraphs—to create a syllabus. Have a main heading that gives the course title (one `#`), then subheadings for, at least, course info and readings. Use emphasis (`*`) for book titles and try to get a list in there somewhere.

You can look at an example syllabus in raw text form [here](https://raw.githubusercontent.com/DHRI-Curriculum/git/master/sections/syllabus.md). When it's rendered by GitHub, it looks like [this](https://github.com/DHRI-Curriculum/git/blob/master/sections/syllabus.md). When editing the markdown file in VS Code, it might look like this:

![What your markdown might look like when typed into VS Code](../images/vscode2.png)

VS Code also has a preview feature for your markdown. Hit the preview button on the top right while editing your markdown file:

![Button to hit to get a preview in VS Code](../images/vscode3.png)

You'll get two side-by-side panels. Your markdown file will be on the left, and your rendered preview will be on the right:

![Side by side markdown and preview in VS Code](../images/vscode4.png)

Remember to save your work with `Control-s` on Windows or `⌘-s` on Mac OS.

# Staging and Committing Changes

Git's primary function is version control, or to track a project as it exists at different points in time. Now that we have a file to track—our markdown syllabus—let's use Git to save the current state of the repository as it exists now.

## A Metaphor for Adding and Committing

In Git, a **commit** is a snapshot of a repository that is entered into its permanent history. To commit a change to a repository, we take two steps:

1. Adding files to a "staging area," meaning that we intend to commit them. 
2. Finalizing the commit.

Staging a file or files is you telling Git, "hey! pay attention these files and the changes in them". 
Making a commit is a lot like taking a photo. First, you have to decide who will be in the photo and arrange your friends or family in front of the camera (the staging process). Once everyone is present and ready, you take the picture, entering that moment into the permanent record (the commit process).

## Staging Changes with the Add Command

First, let's see what state Git is currently in. It's a good idea to use this command before and after doing anything in Git so you can always be on the same page as the computer.

Make sure you're in your `/home/<your-name>/Desktop/projects/git-practice` directory using the `pwd` command in the terminal. Once you're there, enter this command:
```
	git status
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

	git add syllabus.md
	
You should see no output from the command line, meaning that the above command succeeded. Let's run `git status` again to check if things have changed. You should see output like this:

```
On branch master

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)

	new file:   syllabus.md
```

The `new file:   syllabus.md` should be highlighted in green to show that it's ready for commit. This is Git telling you, "Ok, I see the file(s) you're talking about." 

## Committing Changes

Now that our files have been staged, let's commit them, making them part of the permanent record of the repository. Type:

	git commit -m "Initial commit of syllabus file"
	
The `-m` flag provides a message along with the commit that will tell others—or remind a future version of yourself—what the commit was all about. Try not to type `git commit` without the `-m` flag for now—there's a note about this below.

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

	git log
	
You should see output similar to this:

```
commit 8bb8306c1392eed52d4407eb16867a49b49a46ac (HEAD -> master)
Author: Patrick Smyth <patricksmyth01@gmail.com>
Date:   Sun May 20 16:03:39 2018 -0400

    Initial commit of syllabus file
```

This is the log of commits, comprising a history of your repository. There's only one commit here now, though. If you don't see a prompt (the `$`) after running `git log`, you may need to press the `q` key (just the `q` key by itself) to return to the command line.

## Why Do We Need to Use the -m Flag?

The -m flag is useful for human purposes and technical purposes. For human purposes, the -m flag helps you keep track of the changes you're making. Version control is most useful when you can confidently return to a specific version. It can also help you be more structured in your approach to making changes - your notes to self are limited, so to make the clear you might make commits after specific tasks are completed, such as: update readings for week 1 - X Author added.This can also make it easier to reverse a specific change in the future. 

Also, if you type `git commit` by itself, git will open the command line's default text editor to allow you to enter the commit message. Unfortunately, the default text editor, `vi`, requires some knowledge to use, and we don't teach it as part of our sessions.

If you find yourself stuck in an unfamiliar screen in the command line after running `git commit`, you're probably in `vi`. Type this to leave that environment and return to the `$` prompt:

	:q
	
If you're ever stuck or "trapped" on the command line, try running through these common exit commands to return to the prompt:

```
Control-c
Control-d
q
:q
```

`Control-c` attempts to abort the current task and restore user control. `Control-d` escapes the current shell environment—if you use it at the normal `$` prompt, it will end the current command line session. `q` is used to escape from specific utilities like `less`. `:q` first changes the mode in `vi`, allowing you to enter the `q` key to quit, so it's a command specific to `vi`.

# Pushing to GitHub

Now, you may want to backup or share that file on the Internet. Let's connect the directory you made on your local machine to GitHub, on the web. 

Remember, GitHub is a service that allows us to host files, collaborate, and find the work of others. Once our syllabus is on GitHub, it will be publicly visible.

Go to GitHub in your browser and click the plus sign in the upper right hand corner.

![You can find the plus sign button to add a repo on the top right of github](../images/addrepo.png)

After clicking the plus button, select `New repository` from the dropdown menu.

![The dropdown menu where you select New Repository](../images/createrepo.png)

After clicking `New repository`, you'll have to enter some information, including a name and description for your repository.

![Screen on GitHub where you enter your repository information](../images/createrepo2.png)

- Choose a name, such as `git-practice`.
- Enter a description, such as `Test syllabus for learning Git and GitHub`.
- Keep the `Public — Anyone can see this repository` selector checked.
- Do *not* select `Initialize this repository with a README` since you will be importing an existing repository from your computer.
- Click `Create repository`.

You should end up inside your newly created git-practice repo. It will look like a set of instructions that you might want to use to connect your GitHub repository to a local repository.

The instructions we want consist of two lines underneath the heading `...or push an existing repository from the command line`. The hand in this screenshot points to where these directions are on the page:

![The commands you need to copy from the new repo page on GitHub](../images/connect-repo.png)

Copy out the first command and paste it in your terminal. It should look something like this:

	git remote add origin git@github.com:<username>/<repository-name>.git
	
You'll need the command copied from your new repo, since it will contain the correct URL.

Next, paste the second command. It will look exactly like this:

	git push -u origin master

After running this command, you should see output that looks like this:

```
Total 4 (delta 3), reused 0 (delta 0)
remote: Resolving deltas: 100% (3/3), completed with 3 local objects.
To github.com:<repo-name>/git.git
   916998f..9779fa7  master -> master
```

If you see output like this, go back to your new repository page in the browser and click the `Refresh` button. You should see your `syllabus.md` file on GitHub!

