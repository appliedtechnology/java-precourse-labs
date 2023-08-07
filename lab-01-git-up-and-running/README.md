# Time to git up and running

## Info

Ask a 100 software developers what you need to know as a developers and you'll get a 100 different answers, except for one thing, 99 of them will tell you to learn about Git.

Git and versions control is universal nowadays. It's not hard, but can be slow and confusing when you are a beginner. Let's alleviate that!

## What you will be working on

Today will be all about working with git. Is to just use the tool so that it mecomes more natural working with it. The lab instructions will be vage on purope, the goal is for you to look through documentation and resources in order to find out what the next step is.

## A word of warning

It's incredibly easy to have AI tell you what to do next if you get stuck. That defeats the purpose of this excersise. Asking AI for help is like learning a new language, using Google Translate instead of folowing the exersise seteps.

The learning is in the doing and if you do not take the time to things yourself, your long term learning will suffer.

## Setup

## Resources

[Git It? How to use Git and Github](https://www.youtube.com/watch?v=HkdAHXoRtos)
[Conventional commits](https://www.conventionalcommits.org/en/v1.0.0/)
[Best practices for using Git](https://deepsource.com/blog/git-best-practices)

## Lab instructions

#### Let's first set everything up:

1. Make a new prive repo on GitHub.com and clone it to your own computer.

1. Open this cloed folder in VS-Code, create a new file named `news.md`, add a "Hello World" inside and commit that file with an appropriate commit message.

1. Once you've committed the `news.md` file, push your commit to the remote repository on GitHub.

#### Your change should now be available on GitHub. Let's branch out to make a change!

1. In the news.md file, add anything interesting you've learned about recently. Once added, commit!

1. Create a new branch named `feature/update-news`. Switch to this new branch. This is where you will make more changes to your `news.md` file.

1. In the `feature/update-news` branch, add another paragraph in the news.md file (maybe link to a news article you've read?). Commit!

1. Now, push this new branch to your GitHub repository. Then go to the Repo online and make sure it's there.

1. Online at GitHub, create a Pull Request (PR) from the `feature/update-news` branch to the main branch. This will merge the changes from your new branch to the main one.

1. Review the changes to make sure whoever did the changes did not do anything wrong and then, merge the pull request.

1. Now, go back to your local environment. Switch to the `main` branch and pull. Your changes should now be available.

#### What if we have something not ready for commiting?

1. Make a change to `news.md` but don't commit it. Stash these changes!

1. Switch to another branch or create a new one. Here, make some different changes and commit them.

1. Now, do back to the prevoud branch (hint `git checkout -`) and restore your stashed files

## Conclusion

Congratulations! You've just done some very common git work. From cloning a repository to making changes, committing them, working with branches, creating PRs, and using stash.

Remember, the more you practice, the more comfortable you'll become. And, just like any other skill, consistency is key. So, keep "gitting" at it!
