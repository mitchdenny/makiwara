# Code Makiwara
A "makiwara" is a padded striking post used in karate training. It allows students of karate to practice and hone their skills. A Code Makiwara is an apparatus for developers to do the same.

Put simply, a Code Makiwara (just Makiwara from here on in) is code which a developer has written that they use to learn how various technologies and patterns interact with a problem domain.

## Mandatory Elements of Makiwara
A Makiwara isn't random snippets of source code. To be classified as a Makiwara your code must have the following essential elements.

1. Your code must revolve around a problem domain. It can be a technical problem domain, or a business problem domain.
2. Your code must demonstrate one or more patterns applied to the problem domain.
3. Your code must demonstrate one or more technologies used to implement the patterns applied to the problem domain.
4. Your code must include a README (or README.md) file which conforms to the Makiwara template (see READMETEMPLATE.md and READMESAMPLE.md). It is essential that the README lists the problem domain, patterns and technologies.

## Optional Elements of Makiwara
While the following items aren't strictly necessary for creating a Makiwara, I would recommend them.

1. Your Makiwara should be version controlled with full commit history to show how the code evolved (a DVCS is best).
2. Your Makiwara should be hosted on a code sharing site so others can fork from it to create their own Makiwara.
3. Your Makiwara should be forked from another Makiwara as a starting point. If you can't fine one, use this repository as a starting point.

## Getting Started
Are you ready to get started creating your own Makiwara? Remember, the fourth essential element of a Makiwara is having a README (or README.md) file based on the READMETEMPLATE.md file in this repository. You can simply download the file, fill it in and drop it into your project, then start coding. Ideally you'll publish the Makiwara somewhere public so that others can use it. That is all pretty manual, which is why I recommend that you use a DVCS and a codesharing site to get started.

### Creating a Makiwara on GitHub
If you want to get up and running quickly, just use GitHub.

1. Fork this repository (see option at the top right hand of the screen).
2. Clone to repository to your local machine.
3. Remove the README.md file in your local workspace.
4. Rename the READMETEMPLATE.md file to README.md.
5. Fill out the new README.md file with some background on your Makiwara (see READMESAMPLE.md for inspiration).
6. Remember to remove READMESAMPLE.md to keep your repository clean.
7. Commit the changes to your local repository.
8. Push the changes back to GitHub.
9. Get started coding on your own Makiwara.

One of the great things about the Makiwara concept is that each one can build upon one that you have created previously. Thus allowing you to blend more patterns, concepts and technologies to see how everything works together. If you are doing this you'll find a bit of a problem with GitHub in that you can fork your own repositories. You could create a branch within your own Makiwara but I think I makes them less discoverable and less reusable for others. So I recommend that you use the following technique to work around the issue.

1. Create a new repository on GitHub for your Makiwara (where you see NewMakiwara below use the name of this repository).
2. Use the following commands within your shell to clone the original Makiwara and then push it to the new repository.

    git clone https://github.com/Username/OriginalMakiwara NewMakiwara
    cd NewMakiwara
    git remote -v
    git remote rename origin upstream
    git remote -v
    git remote add origin https://github.com/Username/NewMakiwara
    git remote -v
    git push -u origin master

Because this new Makiwara is a clone of an existing Makiwara you won't need to worry about cleaning up the READMESAMPLE.md and READMETEMPLATE.md files. Instead you'll just need to revise the contents of the existing README.md file with the things that you are adding.

## Contributing
The whole concept of Makiwara was just a half-baked idea that I had. It will take others to contribute to make it less half-baked so I openly encourage others to contribute. You can contribute by making a Makiwara of your own, or make updates to this document to evolve the Makiwara process. If you want to update this document just create a fork, make the necessary changes and submit a pull request. I'm more likely to accept the pull request if you have created a Makiwara of your own just to work through the process. If you do create your own Makiwara and you want to tell the world about it why not add it to the list of known Makiwara!

### List of Contributors
Here are some people who have gotten onboard with the Makiwara concept.

1. [Mitch Denny](http://blog.mitchdenny.com)

### Known Makiwara
Here is a list of Makiwara that have been created. I recommend that you look through to see whether any of these would be a good starting point for your own Makiwara.

1. [TodoMakiwara](http://github.com/MitchDenny/TodoMakiwara/) by [Mitch Denny](http://blog.mitchdenny.com).

## Acknowledgements
I need to acknowledge the work of others that have influenced the creation of the Makiwara concept.

### CodeKata and Dave Thomas
I would be remiss not to acknowledge the concept of [CodeKata](http://codekata.pragprog.com/) by [Dave Thomas](http://pragdave.pragprog.com/), one of the authors of [The Pragmatic Programmer](http://pragprog.com/book/tpp/the-pragmatic-programmer). In Dave's [background article on CodeKata](http://codekata.pragprog.com/2007/01/code_kata_backg.html#more) he outlines a series of short programming exercises. I strongly recommend doing these an other CodeKata practice sessions that you come across. You could say that a Makiwara is just a CodeKata that is shared.

### Design Patterns
I was first introduced to software patterns through the [Portland Pattern Repository on the C2 Wiki](http://c2.com/ppr/). This service created by [Ward Cunningham](http://en.wikipedia.org/wiki/Ward_Cunningham) has made me a better programmer today. You could say that a Makiwara is just a Software Pattern implemented with a specific technology and applied to a concrete problem.

### Git Tips from Adrian Short
I was struggling to figure out how to form my own repository. [Adrian Short's post](http://alt.adrianshort.co.uk/blog/2011/11/08/create-multiple-forks-of-a-github-repo/) helped me figure it out. Without the ability to create a clone/fork of your own repository Makiwara wouldn't be very useful.