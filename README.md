# Info

This is a repo for anyone to use as a reference for the ways COMPSA
does stuff -- whether that be just useful info or the events throughout the
year etc.

Also added bonus: we get a chronology of what we do so we can try and/or avoid
to repeat history.

To read any of the documents (.md files) simply click on the filename -- GitHub
will render the Markdown into HTML to make it nice and pretty

## Hiring Packages

There is a Markdown file for each of the [portfolios](hiring-packages)
outlining the different positions compsa may look for.

> If you work here -- make sure all the portfolios are present & up-to-date
> during hiring

## Manuals

Each **portfolio** has an [operations manual](operation-manuals)
which should outline what the portfolio, and any specified **volunteer positions** --
and any improvements or ammendments are encouraged (make a PR! Look at
[Usage](#Usage)).

## Newsletters

The Association has a two newsletters -- email-format and print-format. The
[Markdown](https://www.markdownguide.org/cheat-sheet/) email-format is
converted into HTML using [pandoc](https://pandoc.org) (see [Usage](#Usage)) and then we can send it
off to the <3-ly Computing students @ Queen's.

The print-format is made using some graphic design software however if you can
find a way to do it in a text format (like using md or tex) that'd be great!
(Canva is free, but [gimp](https://www.gimp.org) is
[free](https://youtu.be/9sJUDx7iEJw?t=17)).

They can be categorized as such:

- `email-format == important updates for computing students & events etc.`
- `print-format == funny computing stuff` 

(contact scribe@compsa.queensu.ca if you wanna add something!)

> More info can be found in [the internal affairs manual](operation-manuals/internal.md#Newsletters) 

## General Assembly Minutes

These outline the motions passed at [General Assemblies](ga-minutes). (should
include minutes of new meeting if GA's are abolished -- for history & transparency)

## Constitution

The [Constitution](constitution/constitution.md) of COMPSA, as a ratified Association under the Alma Mater
Society.

# Usage

All documents in this repo are written in
[Markdown](https://www.markdownguide.org/cheat-sheet/) and then can be
converted to virtually any other format using the cli tool
[pandoc](https://pandoc.org).

Thanks to using pandoc -- we can also include additional syntax like LaTeX and
HTML into the Markdown files directly! Essentially allowing us to create richly
formatted documents (if needed) without the boilerplate (but *with* the **Open Source**)!

## Converting

In order to create say, a pdf, or html version of your document -- first make
sure you've installed pandoc:

```bash
Ubuntu 
sudo apt install pandoc

MacOS
brew install pandoc

Windows !! Not recommended, download WSL2 (Ubuntu) -- it will be useful beyond this
https://pandoc.org/installing.html
```

then use the command:

```
pandoc <filename>.md -o <filename>.<format>
```

of course make sure you're either in the directory with the file or include the
path to `<filename>`.

> for converting to `.pdf` make sure you have a LaTeX package installed (CISC
> yay)


## Editing

For editing Markdown, you can use anything you'd like that works (vs-code is a
good option, it can render a html-preview & has git integration). 

You could also just use GitHub (read below first -- you can do the same the the
GitHub gui)

when you want to make a change(s) first **create a branch** off of main:

```bash
# check you're on main
git status
git checkout main

# check that youre up to date
git fetch
git pull

# make new branch
git checkout -b <branch-name>
```

> Try to name it something helpful.

Once you've made a specific/related changes you should commit your work to help
inform what overall changes were made (through commit messages -- which should
also be named helpfully)

Finally, to add these changes to the `main` branch, push your changes and
[create a PR](https://github.com/Queen-s-COMPSA/Constitution/pulls)!

