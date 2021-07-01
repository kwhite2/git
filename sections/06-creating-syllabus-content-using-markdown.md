← [Creating a Syllabus File](05-creating-a-syllabus-file.md)&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;[Staging and Committing Changes](07-staging-and-committing-changes.md) →

---

# 6. Creating Syllabus Content Using Markdown

We'll be using **Markdown** to write a syllabus, and then using **Git** to track any changes we make to it. Markdown allows us to format textual features like headings, emphasis, links, and lists in a plain text file using a streamlined set of notations that humans can interpret without much training. Markdown files usually have a `.md` extension.  

**Markdown** is a markup language for formatting text. Like HTML, you add markers to plain text to style and organize the text of a document.

Whereas you use HTML and CSS with WordPress, you use Markdown to render legible documents on GitHub. Markdown has fewer options for marking text than HTML. It was designed to be easier to write and edit.  

For comparison, you learned to create headers in HTML like this:

```html
<h1>My Syllabus Heading</h1>
```

In Markdown, we insert headings with a single hash mark like this:

```markdown
# My Syllabus Heading
```

A sub-heading (H2) heading uses two hash marks like this:

```markdown
## Readings
```

The lessons of this workshop were originally written in markdown. You can see [here](https://raw.githubusercontent.com/DHRI-Curriculum/git/v2.0/lessons.md) what they look like in their raw, unrendered form.

Compare that with this—the source code for this lesson's web page, written in HTML [here](view-source:http://curriculum.dhinstitutes.org/workshops/git/lessons/).

Markdown is also arguably more sustainable and accessible than formats like `.docx` because of its simplicity and related ability to be read across multiple platforms. Use of Markdown is also supported by document-conversion tools like [Pandoc](https://pandoc.org/) that can change a markdown file to an `.epub` with one command entered into your terminal.

Here are a few more key elements to get you ready to make your own syllabus in Markdown. 

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

To create a link, put the anchor text (the text you will see) in square brackets and the URL in parentheses, directly following the anchor text in brackets. Don't put a space between them:

```markdown
I teach at [The Graduate Center, CUNY](https://www.gc.cuny.edu).
```

Paragraphs of text are denoted by putting a blank line between them:

```markdown
This is a paragraph in markdown. It's separated from the paragraph below with a blank line. If you know HTML, it's kind of like the <p> tag. That means that there is a little space before and after the paragraph when it is rendered.

This is a second paragraph in markdown, which I'll use to tell you what I like about markdown. I like markdown because it looks pretty good, if minimal, whether you're looking at the rendered or unrendered version. It's like tidy HTML.
```

## Challenge

Use these five elements—headings, emphasis, lists, links, and paragraphs—to create a syllabus. Have a main heading that gives the course title (one `#`), then subheadings for, at least, course info and readings. Use emphasis (`*`) for book titles and try to get a list in there somewhere.

If you want an a more advanced challenge, you can review some additional markdown elements on [this page](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet) and add some extra features like images, blockquotes, or horizontal rules.

## Example

You can look at an example syllabus in raw text form [here](https://raw.githubusercontent.com/DHRI-Curriculum/git/main/sections/syllabus.md). When it's rendered by GitHub, it looks like [this](https://github.com/DHRI-Curriculum/git/blob/main/sections/syllabus.md). When editing the markdown file in Visual Studio Code, it might look like this:

![What your markdown might look like when typed into Visual Studio Code](../images/vscode2.png)

## Tips

1. Visual Studio Code also has a preview feature for your markdown. Hit the preview button on the top right while editing your markdown file:

    ![Button to hit to get a preview in Visual Studio Code](../images/vscode3.png)

    You'll get two side-by-side panels. Your markdown file will be on the left, and your rendered preview will be on the right:

    ![Side by side markdown and preview in Visual Studio Code](../images/vscode4.png)

2. Remember to save your work—regularly!—with <kbd>control</kbd> + <kbd>s</kbd> on Windows or <kbd>⌘</kbd> + <kbd>s</kbd> on macOS.

## Evaluation

Which best describes what you're doing when you initialize your project folder:
- You created a new version of your project folder
- You told Git to pay attention to your project folder*
- You told Git to set up its file structure within your project folder so it can track changes to your files.*
- You use the command `mkdir` in your terminal
- You use the command `git init` in your terminal*

Which best describes Markdown:
- a software installed on my local machine
- a language for formatting plain text files*
- a language that can be read and rendered by some web-based platforms*
- a version control software
- a cloud-based software
- refers to project folders as "repositories"

## Keywords

Do you remember the glossary terms from this section?

- [Markdown](https://github.com/DHRI-Curriculum/glossary/blob/v2.0/terms/markdown.md)

---

← [Creating a Syllabus File](05-creating-a-syllabus-file.md)&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;[Staging and Committing Changes](07-staging-and-committing-changes.md) →
