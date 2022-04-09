---
title: "Knowledge as a Code"
description: "My note taking journey: from paper to blog creation"
date: 2022-04-09T12:18:54+02:00
draft: false
# table of content
toc: true 
image: ""
tags: [Personal thoughts, Obsidian]
categories: [Blog]
---

## Paper
During my school years I used to learn new stuffs writing them down on papers. Writing always helped me 
organizing concepts and repeating words.
However, writing on paper has several downsides:
1. It requires a lot of paper
2. Papers occupies space and get lost, or you don't have the right book when you need it
3. It is not easy to search for something you wrote and it is even harder expand an already written chapter

## Obsidian
Due to the problems listed in previous section, I slowly started writing my notes on my pc.
I tried several stuffs from plain words file, to latex, onenote but the most handful one was
 [obsidian](https://obsidian.md/).
 ![Obsidian main page](https://raw.githubusercontent.com/Ste29/blog-dev/main/static/img/blog/obsidian.jpeg)
Obsidian is a tool which allows to create notes in markdown and connect different files in a powerful knowledge
graph.
It is based on [Zettelkasten](https://en.wikipedia.org/wiki/Zettelkasten) theory in order to associate notes
with each other.
> The Zettelkasten is based on two kind of notes: fleeting notes and permanent notes. Starting from thoughts and
media consumption fleeting notes are produced, then aggregating several notes a permanent is produced.
> Each note is atomic, contains only one argument, but it is closely related with several other notes.

Furthermore, Obsidian comes with a variety of useful plugin:
- [Dataview](https://blacksmithgu.github.io/obsidian-dataview/), which allows to query notes like a database,
small guide [here](https://medium.com/os-techblog/how-to-get-started-with-obsidian-dataview-and-dataviewjs-5d6b5733d4a4#:~:text=%20If%20you%20haven%E2%80%99t%20installed%20a%20plugin%20in,the%20Dataview%20plugin%2C%20then%20the%20Install...%20More%20)
- [MindMap](https://github.com/lynchjames/obsidian-mind-map)
- Templater, which allows to execute javascript code, i.e. it is possible to create a ToDo note for each day 
Obsidian is opened
- Many others are listed [here](https://www.youtube.com/watch?v=W7kTtn9empU) and I will go into further details of
my Obsidian environment during future posts

However, Obsidian has some downsides too...
1. Syncing notes between different devices cost 10$ per month
2. Using the free version doesn't backup the notes

In order to solve the second problem I started uploading my Obsidian vaults on Github, but then I asked myself:
> If I'm saving markdown files in Github, why can't I create a blog?

## My Own Blog
Creating a blog, while continuing to use Obsidian, allows me several advantages:
1. To store consolidated notes
2. To share knowledge with other people and receving from them a feedback
3. Versioning what I know exactly how I would do with some code i wrote

The 3rd benefit is really interesting.
It allows you to check how your knowledge on a certain topic evolves with time, what you discover and what
you thought it was true and it revealed false.

Also, in my opinion knowledge as a Code is strictly related with recent trends used in 
[code documentation](https://sysdig.com/blog/adopting-docs-as-code/) which is closely related with 
CI/CD pipelines and automating knowledge transfer from code repos to something more narrow and easily
accessible.