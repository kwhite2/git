← [Creating Syllabus Content Using Markdown](6-creating-syllabus-content-using-markdown.md)  |  [Pushing to GitHub](8-pushing-to-github.md) →

---

# 7. Staging and Committing Changes

Git's primary function is version control, or to track a project as it exists at particular points in time. Now that we have a file to track—our `syllabus.md`—let's use Git to save the current state of the repository as it exists now.

## A Metaphor for Adding and Committing

In Git, a _commit_ is a snapshot of a repository that is entered into its permanent history. To commit a change to a repository, we take two steps:

1. Adding files to a "staging area," meaning that we intend to commit them.
2. Finalizing the commit.

Staging a file or files is you telling Git, "Hey! Pay attention these files and the changes in them".

Making a commit is a lot like taking a photo. First, you have to decide who will be in the photo and arrange your friends or family in front of the camera (the staging process). Once everyone is present and ready, you take the picture, entering that moment into the permanent record (the commit process).

## Staging Changes with the `add` Command

First, let's see what state Git is currently in. It's a good idea to use this command before and after doing anything in Git so you can always be on the same page as the computer.

Make sure you're in your `/home/<your-name>/Desktop/projects/git-practice` directory using the `pwd` command in the terminal. Once you're there, enter `git status` and you should see the following output:

```console
$ git status
On branch main

No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be committed)

	syllabus.md

nothing added to commit but untracked files present (use "git add" to track)
```

"Nothing added to commit" means that we have initialized our repository, but haven't made any commits yet. _If you're instead getting a message that begins with the word `fatal` when you use `git status`, you may be in the wrong directory or perhaps you haven't run the `git init` command on your directory yet._

Let's follow the recommendation in the status message above and use the `add` command to stage files, making them ready to be committed.

We will go ahead and add `syllabus.md` by writing the following in the terminal:

```console
$ git add syllabus.md
```

You should see no output from the command line, which should be interpreted as a the above command succeeded. It is what we call "succeeding silently." Let's run `git status` again to have a "sanity check"—to make sure that things have changed. You should see output like this:

```
$ git status
On branch main

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)

	new file:   syllabus.md
```

The `new file:   syllabus.md` should be highlighted in green to show that it's ready for commit.

This is Git telling you, "Ok, I see the file(s) you're talking about."

## Committing Changes

Now that our files have been staged, let's commit them, making them part of the permanent record of the repository. In the terminal, type:

```console
$ git commit -m "Initial commit of syllabus file"
```

The `-m` flag provides that the message following the flag (in quotation marks) along with the commit. The message will tell others—or remind a future version of yourself—what the commit was all about. Try not to type `git commit` without the `-m` flag—there's a note about this below.

After running the command, you should see output like this:

```
[main (root-commit) 8bb8306] Initial commit of syllabus file
  1 file changed, 0 insertions(+), 0 deletions(-)
  create mode 100644 syllabus.md
```

This means you have successfully made your first commit in the repository—congratulations!

Let's check the state of our repository after the commit by running `git status`:

```
$ git status
On branch main
nothing to commit, working tree clean
```

This means that everything in the repository is successfully committed and up-to-date. If you edit your syllabus file or create a new file in the repository, the message you get with `git status` will instead list files that have uncommitted changes.

Let's run one other command to see the effect our commit has had. Enter this command:

```console
$ git log
```

You should see output similar to this:

```
commit 8bb8306c1392eed52d4407eb16867a49b49a46ac (HEAD -> main)
Author: Patrick Smyth <patricksmyth01@gmail.com>
Date:   Sun May 20 16:03:39 2018 -0400

    Initial commit of syllabus file
```

This is the log of commits, comprising a history of your repository. There's only one commit here now, though. If you don't see a prompt (the `$`) after running `git log`, you may need to press the <kbd>q</kbd> key (just the <kbd>q</kbd> key by itself) to return to the command line.

## Why Do We Need to Use the `-m` Flag?

The `-m` flag is useful for human purposes and technical purposes. For human purposes, the `-m` flag helps you keep track of the changes you're making. Version control is most useful when you can confidently return to a specific version. It can also help you be more structured in your approach to making changes—your notes to self are limited, so to make them clear, you might make commits after specific tasks are completed. If you update readings for the first week of classes or if you add another reading, you will want to make a. This can also make it easier to reverse a specific change in the future.

Also, if you type `git commit` by itself, git will open the command line's default text editor to allow you to enter the commit message. Unfortunately, the default text editor, `vi`, requires some knowledge to use, and we don't teach it as part of our sessions.

If you find yourself stuck in an unfamiliar screen in the command line after running `git commit` and forgetting the `-m flag`, you're probably in `vi`. Type this to leave that environment and return to the `$` prompt: `:q` followed by <kbd>enter</kbd>.

If you're ever stuck or "trapped" on the command line, try running through these common exit commands to return to the prompt:
- <kbd>Control</kbd> + <kbd>c</kbd>
- <kbd>Control</kbd> + <kbd>d</kbd>
- `q` followed by <kbd>enter</kbd>
- `:q` followed by <kbd>enter</kbd>

<kbd>Control</kbd> + <kbd>c</kbd> attempts to abort the current task and restore user control. <kbd>Control</kbd> + <kbd>d</kbd> escapes the current shell environment—if you use it at the normal `$` prompt, it will end the current command line session. `q` is often used as a command (followed by <kbd>enter</kbd>) to escape from specific programs like `less`. `:q` is the command used in `vi` that changes the mode of interaction (`:`), allowing you to enter the `q`, a one-letter command to quit, which must be followed by <kbd>enter</kbd>. Thus, it's a command specific to `vi`.

## Evaluation

Which best describe the process of _staging_:
- you telling Git to take a snapshot of changes made to a file.
- you telling Git which files with changes you want it to pay attention to.*
- you telling git to pay attention to a folder storing files you want to make changes to.
- the second part of a two-step process.

Which best describes the process of _committing_:
- you telling Git to take a snapshot of changes made to a file.*
- you telling Git which files with changes you want it to pay attention to.
- you telling git to pay attention to a folder storing files you want to make changes to.
- the second part of a two-step process.*

What happens if you _stage_ the files, but don't _commit_ them?
- Git won't know what files you want to take a snapshot of
- Git won't take a snapshot of the files.*
- Git will take the snapshot of the files
- You will have told Git what files you would like it to take a snapshot of.*

What happens if you _commit_ the files, but don't _stage_ them?
- Git won't know what files you want to take a snapshot of*
- Git won't take a snapshot of the files.*
- You will have told Git what files you would like it to take a snapshot of.
- Git will take the snapshot of the files*

Which best describes the `-m` flag used when committing changes to a file?
- a brief description of changes you made to your file*
- Its just something Git needs so it doesn't break
- future aids when you are trying to make sense of or recover changes you previously made to a file*
- It's nonsense—who needs it?!

## Keywords

Do you remember the glossary terms from this section?

- [Commit](https://github.com/DHRI-Curriculum/glossary/blob/v2.0/terms/commit.md)

---

← [Creating Syllabus Content Using Markdown](6-creating-syllabus-content-using-markdown.md)  |  [Pushing to GitHub](8-pushing-to-github.md) →