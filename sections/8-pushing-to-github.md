← [Staging and Committing Changes](7-staging-and-committing-changes.md)  |  [Cloning and Forking](9-cloning-and-forking.md) →

---

# 8. Pushing to GitHub

Now, you may want to backup or share and collaborate around a file on the Internet. Let's connect the directory you created on your local computer to GitHub's cloud service, which you can access through the web.

Remember, GitHub is a service that allows you to host files, collaborate, and find the work of others. Once our syllabus is on GitHub, it will be publicly visible. (Repositories on GitHub can also be private but are public by default.)

Go to GitHub in your browser and click the plus sign in the upper right hand corner.

![You can find the plus sign button to add a repo on the top right of github](../images/addrepo.png)

After clicking the plus button, select `New repository` from the dropdown menu.

![The dropdown menu where you select New Repository](../images/createrepo.png)

After clicking `New repository`, you'll have to enter some information, including a name and description for your repository.

![Screen on GitHub where you enter your repository information](../images/createrepo2.png)

- Choose a name, such as `git-practice`. (This does _not_ need to match your folder name although it may be less confusing if you choose the same name here.)
- Enter a description, such as `Test syllabus for learning Git and GitHub`.
- Keep the `Public — Anyone can see this repository` selector checked. (If you choose the Private option, you will need additional steps, not covered in this workshop, to synchronize your GitHub repository with the folder on your computer.)
- Do _not_ select `Initialize this repository with a README` since you will be importing an existing repository from your computer.
- Click `Create repository`.

You should end up inside your newly created repository. It will look like a set of instructions that you might want to use to connect your GitHub repository to a local repository.

The instructions we want consist of two lines underneath the heading `...or push an existing repository from the command line`. The hand in this screenshot points to where these directions are on the page:

![The commands you need to copy from the new repo page on GitHub](../images/connect-repo.png)

Copy out the first command and paste it in your terminal. It should look something like this:

```console
$ git remote add origin git@github.com:<username>/<repository-name>.git
```

You'll need the command copied from your new repository, since it will contain the correct URL.

Next, paste the second command. It will look exactly like this:

```console
$ git push -u origin main
```

After running this command, you should see output that looks like this:

```
Total 4 (delta 3), reused 0 (delta 0)
remote: Resolving deltas: 100% (3/3), completed with 3 local objects.
To github.com:<repo-name>/git.git
   916998f..9779fa7  main -> main
```

If you see output like this, go back to your new repository page in the browser and click the `Refresh` button. You should see your `syllabus.md` file on GitHub!

## Review

We have covered the basic steps of creating a file and tracking changes within a file on your local machine and on GitHub.

This has involved coordinating across three different environments, so let's go through that one more time. Note that this process is very slightly different. I'll highlight it when it comes up.

To start, let's add something to our syllabus. Another week of materials or a new reading.

Save that file.

Use `git add` via the command line to stage the file—tell Git what document you want it to pay attention to.

Use `git commit` via the command line to save the changes you've just made as a snapshot or new version of you file. Remember to use the `-m` flag and include a message about the change you just made.

So far, we have not done anything with GitHub or on the Internet. We have used Git, installed on our local machine, to save a version of file as it stands now. We could stop here if we only had an interest in using Git for version control. But if we also wanted to use GitHub to back up our files, or to share our project with a team or publicly, we want to upload, or push, that repository to GitHub on the Internet.

Use `git push origin main` to _push_ that file to your repository on GitHub. After refreshing the webpage, your file should appear online. **The difference I noted above appears here.** Note the absense of the `-u` flag from the command. That flag was used the first time to establish the connection between the repository on your local machine and on GitHub. Now that that connection has been established, that flag is not needed.

## Challenges

1. Go through the process a few more times by adding additional readings and weeks of course material. Remember to commit changes intentionally so your commit messages make sense. Use `git log` to review your changes.

2. Also try creating a new file and adding an assignment. Rewrite the assignment using Markdown, or edit and add in the markers. Go through the process of staging and commiting that file, and pushing it to your repository on GitHub.

3. Test your understanding by thinking through the following questions:
- Do you need to push the file to GitHub each time you commit changes to the file, or can you make several commits to a file and push them all to GitHub at once?
- Do you need to use `git init` after after adding a new assignment file to your folder?
- What about the `-u` flag in the `git push origin main` command? Does this flag need to be used to add the assignment to your repository on GitHub?

## Solution

In response to _Challenge 3_:
- No, you don't need to push to GitHub every time, or at all even, if you didn't want to share your changes publicly. Git is the software that tracks the changes, and you review them on your local machine using Git as well.
- No, you don't need to initialize the folder after adding a new file for an assignment or otherwise. In this case, we've already initialized the process; Git is tracking the folder. After the file is added, we just need to notify Git to take a snapshot of the additions and changes using the `git add`, `git commit` sequence. We can also use `git push` to share those changes on GitHub.
- No, the `-u` flag does not need to be used again. This flag is only necessary when setting up the original connection between the folder on your local machine and the folder on GitHub.

## Evaluation

Which best describes what you're doing when you use the command `git push`?
- you telling Git to take a snapshot of changes made to a file.*
- you telling Git which files with changes you want it to pay attention to.
- you telling git to pay attention to a folder storing files you want to make changes to.
- you are copying the updated files with the changes to the repository on GitHub*
- the second part of a two-step process.*

How does the process of _pushing_ differ from the processes of _staging_ and _committing_ discussed in the previous lesson?
- There is no fundamental difference between these processes.
- Staging and Committing set up the files whereas pushing is the act of taking the snapshot.
- Staging and committing the files is to communicate with GitHub on the Internet, pushing the changes happens on your local machine.
- Staging and committing the files happens on your local machine, pushing the changes is to communicate with GitHub on the Internet.

What happens if you use `git push` without staging and committing files?
- Git won't know what files you want to take a snapshot of.*
- Git won't take a snapshot of the files.*
- Your computer won't know what changes to share with GitHub.*
- Git will take the snapshot of the files
- You will have successfully created a new version of the file.
- You will have communicated with GitHub and shared a copy of the updated files.
- You will have communicated with GitHub to copy a set of files from their servers to your local machine.

What happens if you _stage_ and _commit_ files, but not _push_ the changes?
- Git won't know what files you want to take a snapshot of.
- Git won't take a snapshot of the files.
- Your computer won't know what changes to share with GitHub.
- Git will take the snapshot of the files*
- You will have successfully created a new version of the file.*
- You will have communicated with GitHub and shared a copy of the updated files.
- You will have communicated with GitHub to copy a set of files from their servers to your local machine.

## Keywords

Do you remember the glossary terms from this section?

- [Push](https://github.com/DHRI-Curriculum/glossary/blob/v2.0/terms/push.md)
- [Repository](https://github.com/DHRI-Curriculum/glossary/blob/v2.0/terms/repository.md)

---

← [Staging and Committing Changes](7-staging-and-committing-changes.md)  |  [Cloning and Forking](9-cloning-and-forking.md) →