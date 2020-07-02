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

If you look just under the workshop title, `DHRI-Curriculum/git` at the top of this page, you can see it is `forked from pswee001/Git_DRI_Jan_2018`. That line shows that this particular repository is building on ("forked from") the curriculum for a session I presented at our January 2018 Institute. If you then look at that repository, you will see that it is in turn forked from previous sessions that were developed by other GC Digital Fellows for workshops in past years. 

### Collaborative Writing

Some of us use Git to track changes (*version control* in Git parlance) in writing projects, and find it to be a cleaner, more elegant solution than the Track Changes functionality in Microsoft Word.

#### Case Two: Coauthored Publications

I personally have had Word crash and sections of an article lost, when I was collaborating on a large writing project with co-authors who were using different versions of Word. If we had tracked our revisions using Git, the previous versions of the paper would always be saved and changes documented in case we wanted to return to an idea from an earlier draft, or a section that reviewer 3 *really* wants to see included in the discussion but was cut for space.

### Versions Across Time

Have you ever had a folder full of multiple and conflicting versions of documents that looked like this?


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

Many of us borrow and adapt from syllabi that colleagues have shared with us. For example, when I first taught, I was offered syllabi by colleagues who had taught the course before. I used some of their work as a base to build my particular course, and after developing my own syllabi, I happily emailed them to other graduate students teaching for the first time. 

This common and collegial practice has some challenges, however. As my colleagues and I emailed around Word documents, it became difficult to identify who had created which assignments or language, and we rarely got to see how others developed innovative approaches that would be useful in our own classes. 

#### Case Three: Syllabi

If my colleagues and I had instead forked our syllabi from each other's repositories on GitHub, our individual work would be attributed, and we could follow each other's revisions and additions to better revise our own. I could also easily trace forked repositories back to syllabi from previous semesters and dig up that classic or obscure reading that I wanted to reincorporate into the course.

Later in this workshop, you will create your own syllabus, track different versions of it, and replicate ("push") your local version to GitHub. With luck, this will give you a sense of how some of the above workflows might work in practice.