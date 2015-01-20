# Contributing to our Curriculum
(these notes are under construction!)

## 0. Introduction

This guide explains how to contribute to our curriculum. You can:
+ Suggest amendments and improvements to our projects;
+ Write new projects;
+ Translate our projects into other languages.

You don’t have to use this method to contribute. If you prefer, you can also email us with your contribution at projects@codeclub.org.uk. Alternatively, you can raise an issue with our [Scratch](https://github.com/CodeClub/scratch-curriculum/issues), [HTML & CSS](https://github.com/CodeClub/webdev-curriculum/issues) or [Python](https://github.com/CodeClub/python-curriculum/issues) projects directly through Github.

The easiest way to contribute is with a Github account. If you don't have an account, you can [sign up](https://github.com/join). You can also install the Github application, which is available for [windows](https://windows.github.com/) or [mac](https://mac.github.com/).

## 1. Create a copy of the projects

+ Go to the repository you wish to contribute to. We currently have [Scratch](https://github.com/CodeClub/scratch-curriculum), [HTML & CSS](https://github.com/CodeClub/webdev-curriculum) and [Python](https://github.com/CodeClub/python-curriculum) project repositories.

+ Click the 'Fork' button to create your own copy of the projects repository.

+ (For new projects or translations only). Clone the repository to your computer. This will create a copy of your new repository on your local computer.

```
cd ~/Documents
git clone git@github.com:YOUR_NAME/REPOSITORY_NAME.git
```

Note: Replace YOUR_NAME with your GitHub username, 'Documents' with the name of the folder you'd like to save the repository into, and REPOSITORY_NAME with the name of the repository. This will be one of the following:

+ scratch-curriculum
+ webdev-curriculum
+ python-curriculum

## 2. Make your contribution

You can now:
+ [Make amendments and improvements to projects](amending.md);
+ [Write new projects](projects.md);
+ [Translate our projects into other languages](translating.md).

## 3. View your contribution

To view your contribution, you'll need to use the [lesson_format](https://github.com/CodeClub/lesson_format) tool to build a local copy of our projects. Instructions on how to install the lesson formatter are [here](https://github.com/CodeClub/lesson_format/blob/master/README.md).

## 4. Save your contribution

For small changes made on the Github website, you can simply click 'Propose File Change' and then 'Create Pull Request'.

For new projects and translations, the contributions you've written are saved to your local computer, but you'll need to upload them to your Github account. Here's how you upload your contribution:

+ Go to the root folder of your repository, for example:

```
cd ~/Documents/scratch-curriculum
```

+ Add in your files.

```
git add --all
```

+ Commit your contribution:

```
git commit -m 'Your message here'
```

+ Push your contribution to your Github account.

```
git push
```

## 5. Merge your contribution with our curriculum

Click the 'Pull Request' button, which will alert us to your contribution.

When we merge the pull request, your contribution will become part of the main curriculum repository, available for everyone to use and benefit from!

If you've translated a project (or projects), give another native speaker a link to your pull request, which will be something like http://github.com/codeclub/scratch-curriculum/pull/3. If they’re happy, they should leave a comment on the pull request with a :+1: or similar message.
