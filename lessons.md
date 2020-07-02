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

In this session, we'll be using the command line (terminal, bash) from the Command Line workshop. We'll also use your text editor and your browser. We'll be moving between these three spaces throughout the workshop. You may want to use (command + tab) or (ctrl + tab) to move quickly between the three windows on your desktop.

To begin with, we'll review some command line basics, including navigation. For more on the command line, review the [materials for the command line session](https://github.com/DHRI-Curriculum/command-line).

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