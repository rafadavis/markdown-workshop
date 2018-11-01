# Introduction

## Intro to GCDI

## What is markdown, and markup languages in general?

- A markup language is a system for annotating your text through instruction encapsulated by tags.
- You write in plain text to create rich text.
    - Most famous one: [HTML](https://blog.experient-inc.com/wp-content/uploads/2013/06/bigstock-html-code-12355271.jpg)
- Markdown is a language designed for writing.
- It is light enough that allows us to read the text without visual polution.
	
## Why not Microsoft Word or Google Docs?

- Word seems easy now, but it will drive you crazy in the long run.
- Microsoft Office package is expensive.
- Files are not universal.
- Word is very distractive.
- Problems with incompatibility.
- Files are heavier and tend to corrupt.
- Problems merging files, copying text from other files, numbering.


## Why should I use Markdown?
- You can make beautiful professional formatting without much work. <!-- show joshua's article vs regular article -->
- It can easly be converted to other formats: doc, pdf, html, etc.
- Separation of form and content allows you to focus on your writing.
- Text editors are meant to be worked with text structure, so they force you to think about the organization of your writing.
- Future proofing your files: plain text files are universal. They will work on any computer, of any operational system, forever.
- There is no lock-in. If you don't like it, you can convert the files to doc files (bleargh) and go back to work the way you used to.
- Variety: You can use multiple great softwares to write your dissertation, a lot of them free and open source. It is so light, you can take a look at your work in your cellphone in the subway and edit that paragraph that you cang get off of your mind.
- The more you learn, the more powerful tools you can access, such as automatic citations.
- If you are writing a dissertation, or a thesis, there is a good chance your university has the template ready, so you don't need to worry about adjusting to their standards.


# Writing in Markdown

## What do we need?
- A text editor
    - Suggestion: [VS Code](https://code.visualstudio.com/) works in Mac, Linux and Windows.
- [Pandoc](https://github.com/jgm/pandoc/releases/tag/2.3.1) to convert to different files.
- Some latex version to create pdf files 
    - [Miktex](https://miktex.org/) works on Mac, Linux and Windows.
    - On mac, [basictex](www.tug.org/mactex/morepackages.html) also worked fine.
- Online alternative: <https://dillinger.io/>


## Create a Markdown file

A Markdow file is nothing more than a text file, saved with the extension ".md". This extension helps the text editor recognize that you are writing in Markdown.

Everything installed, let's create a Markdown file, and let's do it in the terminal. We will need to use the terminal later, when we will convert our markdown file, so we might as well start getting used to it right now.

If you have never used the terminal, it might seem a bit scary. Don't worry, we won't need to learn too much here, just some simple commands. For now, they will be `pwd`, `ls`, `mkdir`, `cd` and `code`.

1. Open your terminal
    - For mac, press *CMD + Space*, type "terminal" and press *Enter*
	- For linux, press *Ctrl + Alt + T*
	- For windows, hit *Super/Windows* key, type "powershell" and press Enter

    Something like this will show up: "user-name@computer-name:~$". This varies with the operational system you are using.

1. Let's check first where we are in the terminal: type "pwd" and press *Enter* or *Return*  (pwd means "Print Working Directory").

    The result will be something like: "/home/user-name". Again, this varies with the OS you use.

1. If you want to see what is in your current directory, type "ls" and press *Enter*. Try it.
    - Check if you see a Document folder in that list
	- In case you do, type "cd Documents" to go to the Document folder. ("cd" means change directory)
	- In case you don't see a document folder, don't worry, just stay where you are.
	
1. Let's create a folder to save our markdown file, calling it "markdown": type "mkdir markdown" and press *Enter* (meaning "make directory" and name it "markdown").

1. Move to this new folder: type "cd markdown" and press *Enter*
1. Try "pwd" and *Enter* again to make sure you are on the markdown folder.
1. If you try "ls" and *Enter* again, you should get nothing in return. That makes sense, because we haven't added anything to our folder yet.

1. Before we create our markdown file, let's just quickly practice moving from folders.
    - To go to a parent folder, type "cd .." and press *Enter*. Notice that there is a space between "cd" and ".."

    Now you should be back to the folder you were before we created our markdown folder. In case you are not one hundred percent sure, remember that you can type "pwd" and press *Enter*

1. We are good to go now. Go to your markdown folder. If you are in Documents, "cd markdown" should do the trick. If you are in the home folder, "cd Documents/markdown" will probably get you there. If you are lost, remember to use `pwd` and `ls`.

1. Once you are in your markdown folder, type "code test.md" and press *Enter* to create and open a markdown file named "test". (this command won't work if you don't have vs code installed) Notice that opening with a different editor will require a different command line.



## Headings

Headings are how we structure our text. When we are writing, we should be thinking about the divisions and subdivisions of our text. Markdown helps us with that. To start a new heading, we need to use to start a line with the pound  symbol "#" (also called "hash", "number", among other words). 

The level of your heading is equal to the number of "#". This is an example of how it works. The following could be the structure of an article:

***

```
# Development

# Introduction

Here I would write my introduction.

## Hypothesis A

Describe some valid hypothesis.

## Hypothesis B

Here I describe another interesting point.

# Conclusion

Here is my conclusion.

``` 
***

Now let's try something.

- In the beginning of your new file, type "# Basic Formatting" and press *Enter*
- On the next line, type "## Headings" and press *Enter*
- On the next line, write "Just a simple text line so we can see how it looks like."

Let's see how it went:

- In VS Code, on the upper right corner, there is an icon for Open Preview. (Alternatively, you can press  "Ctrl/Cmd + k" than "v", but that won't work if you do it slowly.)

		
## Paragraphs and line breaks

To create a new paragraph, press *enter* twice and start typing. This will create a blank line between the last piece of text and the next one. Try the following:

***

```
## Paragraph

If you write this here and then  write in the next line.
Like this.
All those three lines will be together in the same paragraph.

However, this will be a new paragraph, since we skipped a line.
```
***

For line breaks, there are two options. You can either press space twice in the end of the line, or you can type "/" in the end of the line. The second method is preferred, since it is something you and other people can see in the code. 

Let's say we want to try a little poem. Try to make this (or any other short poem in your mind):

***

``` 
## Line Breaks

Ah, what an age it is
When to speak of trees is almost a crime
For it is a kind of silence about injustice!
And he who walks calmly across the street,
Is he not out of reach of his friends
In trouble?
```

***



## Emphasis

- Wrap the word/sentence with * to make it *Italic*.
- Wrap the word/sentence with ** to make it **Bold**.

Therefore, if you write this:

```
This sentence is normal, but this word is *italic*, 
this one is **bold**,and these are ***italic and bold***.

*This whole sentence is italic, but this word is also **bold***.
```

You will get this:

>This sentence is normal, but this word is *italic*, this one is **bold**, and these are ***italic and bold***.

>*This whole sentence is italic, but this word is also **bold***.

### Exercise:

- Type "## Emphasis" and press *enter* to go to the next line.
- Use the charachter "\*" to write something **bold**, something *italic*, and something ***bold and italic***.
- *Write this whole sentence in italic with **these three words** in bold.*

## Block quotes:

Start a line with greater than ">", press space and start writing. To write a blockquote which is longer than a paragraph, make sure to use the ">" sign in the blank line between one paragraph and the other.

- Type "## Block Quotes", press *enter*
- Now, try to make produce this:

> This is my first block quote. I will just write some more to make sure it is longer than a line.
>
> Amazing, it even has two different paragraphs.

## Lists:

- Type "## Lists" and press *enter*

Lists are easy to do. Unordered lists can be done with \*, + or - symbols. Simply start your paragraph with one of them, press *space* and type the list item. Than, press *enter* to go to the next line and do the same. 

To make a nested list, with sub-items, just press *space* for times before using the list symbol.

- Type "### Unordered" and press *enter*

Now try to make this groceries list:

- Bread
- Eggs
- Fruits
    - Apple
	- Bananas
- Milk

Ordered lists can be done either with "1." or "1)". The number don't actually matter. you can always use "1." if you want, the program will make sure to count and put it in the right order. This is good because you don't have to worry about chaning the numbers if you decide to change the order. You can also mix unordered and ordered lists.

- Type "### Unordered" and press *enter*.
- Now try to make this list of steps to make a trip:

1. Buy airplane tickets
1. Make hotel reservation
1. Packing
    - Shoes
	- Socks
	- Shirts
1. Ask mama to water the plants

# Advanced Tools
## Comments

- Type "## Comments" and press *enter*

Comments are a fundamental part of coding, but it can also be very handy to academic writing. Whatever you comment on your file is not going to show up in your final document. This is useful for writing alternative paragraphs that you can decide to change later, leaving comments to yourself of stuff you need to work, decreasing the lenght of an article for a specific publication, etc.

To open a comment, just type \<\!-\- ,  and close it with \-\-\> . Whatever is inside those, will not show up in the final version.


- Now type this and see what happens:

> This should show up in the final version, \<\!\-\- This should not show up, \-\-\> and this should also show up.


## Links

- Type "## Links" and press *enter*

The way to create a link is: `[This is the text of the link](link address)`

- Now try this: \[GCDI](https://gcdi.commons.gc.cuny.edu)

- If you just want to show the address, there is a simpler way to do it. Just wrap it with < and >. For example: \<https://gcdi.commons.gc.cuny.edu/>


## Images

- Type "## Images" and press *enter*

The way to create images is:  `![text](filename.extension)`

- For instance: `![weird cat](cat.jpg)`. For this to work, you need to have the image file (in this case, "cat.jpg) in the same folder as your text file. 

    - If you are working with a lot of images, it might make sense to have a sub-folder of all the images you are using in this project. In that case, your link could be `![weird cat](images/cat.jpg)`

- Another option is to use a link in the web. Try this: `![satisfied dog](goo.gl/uGkft3)`

## Footnotes

- Type "Footnotes" and press *Enter*

Footnotes are also easy. You just need to type this: `[^x]` where you want a footnote. "x" can be a number, can be a letter, can be a word. Somewhere else, usually in the end of the text, you write the content of that footnote:

`[^x]: This is my footnote`

Some people prefer to leave it in the end of the text, some people prefer to have it close to the part of the text that this footnote refers to. Type the following:

>We will try a couple different things to see how footnotes work. Our first one will come here.\[\^1] Now, another footnote here.\[\^3] How about a third footnote here.\[\^2] And a random footnote here.\[\^a] How about a last footnote here.\[\^banana]
>
>
>\[\^1]: First footnote\
>\[\^banana]: Last footnote\
>\[\^2]: Third footnote\
>\[\^a]: Fourth footnote\
>\[\^3]: Second footnote\


And let's see where this is gonna show up. This is probably not gonna work well on the simulators. Therefore, this is a good opportunity for us to make our first pdf files and test everything we've made.

# Pandoc

- Make sure to save your test.md file.
- Go to your terminal
- Make sure you are in the folder that you've created the test.md file
    - Remember, you can use `pwd` to check your directory, and `ls` to see all the files in the directory. 
	- If ls shows you test.md, you are good to go.

Pandoc is the software that converts your markdown file in other files, such as pdf html, docx, etc. It only works in the command line. But don't worry, the basic command is quite simple.

The command we will use is "pandoc -o test2.pdf test.md". Before trying it, let's quickly understand it. This command is asking pandoc to make a pdf file called test2, based on a markdown file named test. The "-o" part is called a flag. In this case, this flag is telling pandoc to guess what kind of file it should create based on the extension we gave. You do not have to worry about this, though.

Let's try it now. 

- Type "pandoc -o test2.pdf test.md" and press *Enter*
- If everything worked, you will get not message, and the standard terminal line will show up again.
- This is a moment that some errors might come up. This can be a bit frustrating, but once you solve it, it will work every time, and it will be fast.
    - If Pandoc or Latex is not correctly installed, this will not work
- If it worked, go to Files and take a look at your pdf file.
- To create a other types of documents, you only need to change the extension. For instance, if you want a Word doc, type "pandoc -o test2.docx test.md". Same goes for ".html", ".odt", etc. 

# YAML Metadata Block

- Close your pdf file and go back to your markdown file.
- Let's try something fancy. Go to the top of your document.
- On the very first line, type "-" three times and press *Enter* to go to the second line.
- On the second line, type "title: the title for this text"
- On the third line, type "author: Your Name"
- On the next line, type "date: November 1, 2018"
- On the next line, type "-" three times again, and press *Enter*
- The beggining of your project should be something like this:

```
---
title: My First Markdown File
author: Rafael Davis Portela
date: November 1, 2018
---
```
- Now save your file.
- Go back to the terminal.
- type "pandoc -o test2.pdf test.md" and press *Enter*.
    - Alternatively, you can press the up arrow key to bring back the last commands you have used. This saves you from typing the same commands over and over again.
- Go to files and open your "test2.pdf" file.
# Evals
Please click [here](www.cuny.is/gcdievals) or go to <www.cuny.is/gcdievals>

# What else? Links and resources
- Publish as e-book, kindle format: <https://leanpub.com>
- Creating presentations:<https://remarkjs.com/#1> and <http://jdan.github.io/cleaver/>
- Version Control (track changes) and  collaborative work on Github. Check [this great explanation](https://blog.red-badger.com/blog/2016/11/29/gitgithub-in-plain-english) on how Github works.
- Kelsey's [awesome blog post](https://digitalfellows.commons.gc.cuny.edu/2018/10/25/uses-of-tech-while-drafting-my-second-exam-bibs/) on using markdown and github to draft the book list for her oral's exam.
- Advanced tools in Pandoc: <http://pandoc.org/MANUAL.html>

# Bonus: Automatic Citation and Reference List

You can try this at home. If it does not work, or if you have any other questions, please come see me in my next office hours, which is going to be on December 5, 5-7pm.

To use automatic citation, you need to follow a few steps.

1. You need a bib file with your Bibliography. 
    - You need to save it **in the same folder as your markdown file**.
    - You can make it manually, but it makes little sense. 
    - If you use zotero, just select all the references and export is as a bib file. 
    - Remember to rename it with a bib extension, in case Zotero doesn't do it automatically. For instance, "project2.bib"
1. In your YAML block, add another line with "bibliography: yourbibfile.bib"
1. Notice that in your bib file, all references will start with something like this: "@book{velasco_barrio_2015," 
    - "velasco_barrio_2015" is the keyword you will use for that reference
1. To create a reference in your text (in your regular file, the one you are writing, not the bib file), type [@name, page]. 
    -For example, "[@velasco_barrio_2015, 37]
1. When it is time to generate your pdf, you will have to add a command to tell pandoc that you are using an automatic citation.
    - Your pandoc line should be something like "pandoc -o test.pdf --filter pandoc-citeproc test.md". It is almost the same as before, you just added "--filter pandoc-citeproc" between the pdf and md file.
1. By standard, pandoc will use Chicago-Style author-date. If that is your style, lucky you. If not you have a few extra steps.
    - Find the code for your citation style here: <http://editor.citationstyles.org/searchByName/>
    - Copy all of the code, paste on a new file and save it **in the same folder as your markdown file** with a csl extension. For instance: "apa.csl"
    - In your YAML block, add another line with "csl: apa.csl"
    - Now it should work

Example of a YAML block:

```
---
title:  |
    | History 127-05
    | MICROHISTORIES: JUSTICE, LAW & CITIZENSHIP IN LATIN AMERICA
    | ---
    | John Jay College of Criminal Justice
date: Spring 2017
author: Rafael Davis Portela
bibliography: project.bib
csl: chicagofull.csl
---
```




