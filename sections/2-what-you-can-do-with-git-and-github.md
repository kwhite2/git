[What are Git, GitHub and Markdown?](1-what-are-git-github-and-markdown.md)  |  [Review of the Command Line](3-review-of-the-command-line.md) →

---

# 2. What You Can Do with Git and GitHub

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

**Case One: This Session**

If you [go this to workshop on GitHub](https://github.com/DHRI-Curriculum/git) and look at the top of the page just under the workshop title, `DHRI-Curriculum/git`, you can see it is `forked from pswee001/Git_DRI_Jan_2018` (next to the red star). That line shows that this particular repository is building on (_"forked from"_) the curriculum for a session presented at our January 2018 Institute by "pswee" (former Graduate Center Digital Fellow Patrick Sweeney). If you then look at that repository, you will see that it is in turn forked from previous sessions that were developed by other GC Digital Fellows for workshops in past years.

![Image of what attribution looks like in GitHub](../images/attribution.png)

_Forking_ is a proper function of the GitHub platform. It supports collaboration by allowing you to copy someone else's repository to your own account on GitHub while maintaining a trail of attribution and derivation. This function is described in further detail in the final lesson of this workshop.

### Collaborative Writing

Git is also used to track changes (_version control_ in Git parlance) in writing projects, especially when there are multiple authors working asynchronously. It can be an alternative to using track changes in Microsoft Word, or comments and edits in a Google Doc.

**Case Two: Coauthored Publications**

Git and GitHub—together or independently—support multi-author publishing. Like we have done with the DHRI curriculum, you can have a shared project folder that multiple people are working from asynchronously, even on the same parts if they wanted, and then those different offshoots can be carefully folded back into the main project. This entails the process of creating _branches_ and _merging_.

Git and GitHub also help with attribution by tracking individual contributions throughout. Additional branches could be created by a singular author as well, allowing the writer to explore different ways forward. The version control feature also allows authors to easily return to and compare older drafts or retrieve sections previoulsy discarded.

_Branches_ and _merging_ are important functions when using Git to collaborate, but they are also advanced and thus beyond the scope of this workshop. See the _Resources_ section at the end of the workshop for more information.

### Versions Across Time

How did you initially come by the syllabus you use for your class(es), and did you develop it over time? Many professors borrow and adapt from each other, and most of us probably update our syllabi each semester, even if only a little bit.

Through this process, many of us end up with a set of files that looks something like this:

```
Documents
│
└───syllabus.docx
│
└───syllabus2.docx
│
└───syllabusRevised.docx
│
└───syllabusFINAL.docx
│
└───syllabusFINALFINAL.docx
│
└───syllabus--WHICH_VERSION??.docx
```

While I probably can tell which version is the "final" one, I can not see what was changed along the way or how the different versions vary from each other.

With Git, you would save these multiple versions over time as one file, and each version you save includes a note about what has changed so you can easily revert back to an older version if needed.

By looking at the file list, you also can not tell who the syllabus originally came from, or if there were contributions from many individuals. Git and GitHub can help make attribution clear, and maintain it over time as a the syllabus travels between hands.

**Case Three: Syllabi**

Increasingly we see that faculty are sharing their syllabi on GitHub (example: [DLCL 204: Digital Humanities Across Borders](https://github.com/quinnanya/dlcl204)). Some are even using GitPages that apply a user-friendly interface to their repository to make it easier to access and navigate for their students (example: [Digital History](https://digitalhistory.github.io/)).

GitHub offers a way of making a course publicly avaiable on the web, and sometimes easier or more intuitive to users than some learning management systems. Git helps track the changes over time.

When the softwares are used together, Git and GitHub also support a collaborative appraoch to syllabi development. Copying another's project and modifying and remixing the content to meet your needs is a seamless and transparent process. Attribution of specific changes over time is a foundational function of how Git operates; GitHub explicitly renders attribution, making it easy to see who(s) did what. This is one of the attractions of using the platform.

In a practical sense, you could search other syllabi on GitHub, and share yours so it could be searched by others. If someone finds a syllabus that includes parts they want to use, they could fork that syllabi to their GitHub account, and download—or _clone_ as Git calls it—the files to your local machine and edit them there. Any changes could then be _pushed_ back to the repository on GitHub, thereby sharing your amendments publicly. On GitHub, attribution of who contributed what are transparent. Meanwhile, your amended version would be available for others to fork and clone and amend and re-share.

Even if you were only working with your own self-created syllabus, like we'll do later in this workshop, Git and GitHub can be useful for tracking your changes without the hassle of multiple files. From one file, you can use Git to compare your current version with older versions; you can also compare and share these different versions on GitHub if you wanted.

_Cloning_ and _pushing_ are proper functionalities of GitHub that describe how you communicate and share files between your local machine and the Internet. These are covered more in-depth in a later lesson in this workshop.

## Evaluation

What tasks could Git and/or GitHub offer support to?
- Developing software*
- Creating and sharing data sets*
- Creating websites*
- Writing articles and books*
- Collating online resources*
- Keeping research notes*
- Hosting syllabi and course materials*

## Keywords

Do you remember the glossary terms from this section?

- [Version Control](https://github.com/DHRI-Curriculum/glossary/blob/v2.0/terms/versioncontrol.md)
- [Branch](https://github.com/DHRI-Curriculum/glossary/blob/v2.0/terms/branch.md)

---

[What are Git, GitHub and Markdown?](1-what-are-git-github-and-markdown.md)  |  [Review of the Command Line](3-review-of-the-command-line.md) →