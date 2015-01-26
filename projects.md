# Writing a New Project
(these notes are under construction!)

## 0. Introduction

This guide explains how to write a new project for our curriculum. If you encounter a problem, remember that you can look at existing projects to see how it's done!

If you're writing a project and need additional support, you can email projects@codeclub.org.uk.

__To contribute a project to our curriculum, you'll need your own copy of the projects. There are instructions on how to do this in the main [contributing](contributing.md) notes.__

## 1. Using the project template.

+ In the projects repository, find the folder called 'Project Template'.

![screenshot](/images/projects/folder.png)

+ Copy and paste this folder, and rename the copied folder with the name of your project.

+ You should see 2 files with `.md` extensions: 

	+ `Project Template.md` - the file containing the project instructions;
	+ `Project Template - notes.md` - the file containing the club leader notes.

![screenshot](/images/projects/md.png)

These files contain 'markdown', which is used to generate projects on the Code Club website. Rename these 2 files with the name of your project.

## 2. Write your project.

Open the `[project name].md` file in a text editor. You can edit this document by adding in your project instructions. Your project may contain some (or all) of the following:

### Activities

You should break your instructions down into separate activities. Each activity should have an 'activity' heading, which can be added by using the following markdown:

`#Step 1: Step name goes here {.activity}`

Underneath this heading you should briefly explain the step children are about to undertake.

### Activity Checklist

Each step should contain a checklist of activities. To display the 'checklist' graphic, you should include this markdown underneath the activity description:

`## Activity Checklist {.check}`

### Activity Steps

Each step should start with a `+` or a `*`, which will give the step a checkbox. If your step contains multiple paragraphs, or an image, these should be indented by pressing the 'Tab' key.

```
+ Step 1
+ Step 2
```

### Bold and Italic Text

You can add text in _italics_ by placing an underscore or a star around the text:

`_italicised text_` or `*italicised text*`

You can add text in __bold__ by placing two underscores or stars around the text:

`__italicised text__` or `**italicised text**`

### Code

You can add some code to your notes `like this`, by adding backticks (`` ` ``) around the text.

`` here is some code: `move (10) steps` ``

You can also format Scratch code, so that the colour matches the associated Scratch block colour (for example `{.blockdata}` for variables). There are some examples of this in the Scratch project template.

`` here is a `score` {.blockdata} variable ``

![screenshot](/images/projects/scratch-code.png)

### Images

The markdown needed to add an image is:

`![alt text](path/imageName.png)`

The path can be omitted if the image is in the same folder as the project markdown file.

### Hyperlinks

A hyperlink can be added through similar markdown:

`[link text](url)`

### Testing

You should regularly ask children to test their project, so that they can see the effects of the code they're creating. You can even use these points as opportunities to fix bugs and improve code.

The markdown for adding in a test point is:

`## Test your project {.flag}`

![screenshot](/images/projects/test.png)

### Saving

You should also regularly remind children to save their work, by using this markdown:

`## Save your project {.save}`

![screenshot](/images/projects/save.png)

### Challenges

You should add at least 1 challenge, to allow children to apply what they've during the project. You can ask children to fix a problem or improve or adapt their project in some way. The markdown for adding a challenge is:

`## Challenge: Challenge name {.challenge}`

![screenshot](/images/projects/challenge.png)

### Scratch Code Blocks

For Scratch projects, code blocks should be contained within 3 backticks, for example:

```
blocks
	when flag clicked
	point in direction (120 v)
	set pen color to [#FF0000]
	pen down
	forever
		move (1) steps
		if on edge, bounce
	end
```

The code above produces the following image:

![screenshot](/images/projects/scratch-output.png)

You can [test](http://scratchblocks.codeclub.org.uk) your Scratch code, and there is a [guide](http://wiki.scratch.mit.edu/wiki/Block_Plugin/Syntax) to adding Scratch blocks to your project notes. You can even automatically generate Scratch code [directly from your online Scratch project](http://scratchblocks.codeclub.org.uk/generator/).

### Embedded Scratch Projects

For Scratch projects, you can also add an embedded version of the final project, so that children can see what they are working towards. Don't worry, children won't be able to see the code! This is done by adding the following HMTL after the introduction:

```
<div class="scratch-preview">
	<iframe allowtransparency="true" width="485" height="402" src="http://scratch.mit.edu/projects/embed/32722912/?autostart=true" frameborder="0"></iframe>
	<img src="project-final.png">
</div>
```

Simply replace the URL with the URL of your finished project, and remember to include a static screenshot image for the PDF version of the project notes.

![screenshot](/images/projects/embed.png)

## 3. Notes for Club Leaders

Each project should have an associated 'notes' markdown file, giving the volunteer useful information for using the project with their Code Club.

The project notes template can simply be modified for your project, and contains the following sections:

### Notes File Properties
You should change the title and the language of the project (if necessary).

```
---
title: Project Template — Notes for Club Leaders
language: en-GB
embeds: "*.png"
materials: [""]
...
```

### Introduction
Explain the project, focusing on what children will learn. Remember that these notes will be read by club leaders and not children.

### Resources
You should include a completed version of your project to help club leaders. This file should be in the folder called 'Club Leader Resources'. You'll need to change the filenames in the notes to match the name of your project.

For Scratch projects, you should also link to an online version of your completed project. Again, you should replace the URL of the sample project with a link to your completed project.

If your project requires any additional resources (such as images), you should add them to the folder called 'Project Resources'. Again, modify the names of any files in the notes.

### Learning Objectives
List the skills that your new project teaches or consolidates. This can be a key programming skill (such as variables or loops), or a general skill like game design, problem solving, collaboration, etc.

### Challenges
You should add at least 1 challenge to your project, to allow children to apply what they've learnt during the project. You can even ask children to fix a problem or improve or adapt their project in some way.

List the names of the challenges in your project, along with a brief description of the activity children will undertake.

### Frequently Asked Questions
You can also add answers to common questions here. This will help club leaders when undertaking your new project with children. This section can be removed if it is not necessary.

## 4. Add your project to the manifest.

+ You should be able to see a file with a `.manifest` extension in the same folder (or the folder above) the folder containing your new project.

+ Add your project to the 'additional projects' manifest. You can do this by copying and pasting an existing project entry, modifying the parameters. Here's an example:

```
        {
            "number":   3,
            "beta": true,
            "filename": "Project Template/Project Template.md",
            "note":     "Project Template/Project Template - notes.md"
        }
```

Make aure that there is a comma between each project entry (after the `}`) but not after the final project!

## 5. You're done!

Go back to the main notes on [contributing](contributing.md) to see how to upload your new project.
