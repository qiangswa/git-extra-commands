<!-- START doctoc generated TOC please keep comment here to allow auto update -->
<!-- DON'T EDIT THIS SECTION, INSTEAD RE-RUN doctoc TO UPDATE -->
**Table of Contents**  *generated with [DocToc](https://github.com/thlorenz/doctoc)*

- [git-extra-commands](#git-extra-commands)
  - [Installing](#installing)
    - [Pre-requisites](#pre-requisites)
    - [Antigen](#antigen)
    - [oh-my-zsh](#oh-my-zsh)
    - [zgen](#zgen)
    - [Without using any frameworks, or if you're a bash user](#without-using-any-frameworks-or-if-youre-a-bash-user)
  - [Other useful git stuff](#other-useful-git-stuff)
  - [Credits](#credits)
  - [Contributing](#contributing)

<!-- END doctoc generated TOC please keep comment here to allow auto update -->

# git-extra-commands

A zsh plugin that packages some extra git helper scripts I've found. I only wrote a few of these scripts, and the ones I didn't each have whatever licensing is included in the file.

This collection doesn't actually require zsh, but packaging as a ZSH plugin makes it more convenient for people using a ZSH framework to use this collection.

If you wrote one of these scripts and want it removed from this repository, please either make a PR or file an issue against the repo and I will remove it.

## Installing

### Pre-requisites

Some of these scripts use dash. `brew install dash` if you're on OS X.

### Antigen

If you're using [Antigen](https://github.com/zsh-users/antigen):

1. Add `antigen bundle unixorn/git-extra-commands` to your `.zshrc` where you've listed your other plugins.
2. Close and reopen your Terminal/iTerm window to **refresh context** and use the plugin. Alternatively, you can run `antigen bundle unixorn/git-extra-commands` in a running shell to have antigen load the new plugin.

### oh-my-zsh

If you're using [oh-my-zsh](github.com/robbyrussell/oh-my-zsh):

1. In the command line, change to _oh-my-zsh_'s custom plugin directory :

    `cd ~/.oh-my-zsh/custom/plugins/`

2. Clone the repository into a new `git-extra-commands` directory:

    `git clone https://github.com/unixorn/git-extra-commands.git git-extra-commands`

3. Edit your `~/.zshrc` and add `git-extra-commands` – same as clone directory – to the list of plugins to enable:

    `plugins=( ... git-extra-commands )`

4. Then, restart your terminal application to **refresh context** and use the plugin. Alternatively, you can source your current shell configuration:

    `source ~/.zshrc`

### zgen

If you're using [zgen](https://github.com/tarjoilija/zgen):

1. Add `zgen load unixorn/git-extra-commands` to your `.zshrc` along with your other `zgen load` commands.
2. `rm ${ZGEN_INIT}/init.zsh && zgen save`

### Manual Installation

Nothing here actually requires you to use ZSH or zgen, that's just a convenient distribution method for anyone using a ZSH framework.

If you aren't using any zsh frameworks, or if you're a bash user, do the following steps:

1. git clone this repository
2. Add it to your `$PATH`.

## Other useful git stuff

* Scott Chacon's [Pro Git](http://git-scm.com/book) book is a great resource for getting more out of git.

* Peter Hurford's [git-it-on.zsh](https://github.com/peterhurford/git-it-on.zsh) plugin. It adds a gitit command that will open your current directory on github, in your current branch.

* Peter also wrote [git-aliases.zsh](https://github.com/peterhurford/git-aliases.zsh), which you may prefer to the git plugin from oh-my-zsh.

* [git-up](https://github.com/aanand/git-up) - Fetch and rebase all locally-tracked remote branches

* Zach Dennis has a great [blog post](http://www.mutuallyhuman.com/blog/2012/06/22/a-git-walkthrough/) - it's worth reading on it's own, but here are a couple of good sites I found through it:
    * [gitready.com/](http://gitready.com/) is another great reference which has been collecting information and tips for git since 2009.
    * [gitimmersion.com/](http://gitimmersion.com/)

* [gitsh](https://github.com/thoughtbot/gitsh) - An interactive shell for git. From within gitsh you can issue any git command, even using your local aliases and configuration.

* Kate Hudson maintains the [git flight rules](https://github.com/k88hudson/git-flight-rules) collection of useful git usage tips.

* [awesome-github](https://github.com/fffaraz/awesome-github) - Faraz Fallahi maintains a curated list of Github & Git resources.

* [git_history_visualizer](https://github.com/kidpixo/git_history_visualizer) - python script to visualize the history of files in a git repository

* [git-fastclone](https://github.com/square/git-fastclone) - Think `git clone --recursive` on steroids. If you're doing repeated checkouts of a given repo on a machine (like a ci box), **git-fastclone** will speed things up considerably.

* There’s a quick [introduction to git](http://learnxinyminutes.com/docs/git/) on learnxinyminutes.com

## Credits

* git-big-file - Mislav Marohnić's [dotfiles](https://github.com/mislav/dotfiles)
* git-change-author - Michael Demmer in [jut-io/git-scripts](https://github.com/jut-io/git-scripts/blob/master/bin/git-change-author)
* git-changes - Michael Markert's [dotfiles](https://github.com/cofi/dotfiles)
* git-churn - Gary Bernhardt's [dotfiles](https://github.com/garybernhardt/dotfiles/blob/master/bin/git-churn)
* git-copy-branch-name - Zach Holman's [dotfiles](https://github.com/holman/dotfiles)
* git-credit - Zach Holman's [dotfiles](https://github.com/holman/dotfiles)
* git-cut-branch - Ryan Tomayko's [dotfiles](https://github.com/rtomayko/dotfiles)
* git-delete-local-merged - [https://plus.google.com/115587336092124934674/posts/dXsagsvLakJ](https://plus.google.com/115587336092124934674/posts/dXsagsvLakJ)
* git-divergence - Gary Bernhardt's [dotfiles](https://github.com/garybernhardt/dotfiles/blob/master/bin/git-churn)
* git-find-dirty - Matthew McCullough's [scripts](https://github.com/matthewmccullough/scripts/) repository
* git-flush - John Wiegley's [git-scripts](https://github.com/jwiegley/git-scripts)
* git-grab - Ryan Tomayko's [dotfiles](https://github.com/rtomayko/dotfiles)
* git-improved-merge - Mislav Marohnić's [dotfiles](https://github.com/mislav/dotfiles)
* git-incoming - Michael Markert's [dotfiles](https://github.com/cofi/dotfiles)
* git-incoming-commits - Ryan Tomayko's [dotfiles](https://github.com/rtomayko/dotfiles)
* git-ls-object-refs - Ryan Tomayko's [dotfiles](https://github.com/rtomayko/dotfiles)
* git-maxpack - John Wiegley's [git-scripts](https://github.com/jwiegley/git-scripts)
* git-nuke - Zach Holman's [dotfiles](https://github.com/holman/dotfiles)
* git-object-deflate - Ryan Tomayko's [dotfiles](https://github.com/rtomayko/dotfiles)
* git-outgoing - Michael Markert's [dotfiles](https://github.com/cofi/dotfiles)
* git-pie-ify - JeeBak Kim's [gist](https://gist.github.com/jeebak/f9088cede18d31f2d3a0)
* git-promote - Trevor's [Improving My git Workflow](http://hoth.entp.com/2008/11/10/improving-my-git-workflow) blog post
* git-prune-branches - Michael Demmer in [jut-io/git-scripts](https://github.com/jut-io/git-scripts/blob/master/bin/git-prune-branches)
* git-publish - Michael Markert's [dotfiles](https://github.com/cofi/dotfiles)
* git-purge-from-history - David Underhill’s [blog](http://dound.com/2009/04/git-forever-remove-files-or-folders-from-history/)
* git-pylint - Runs pylint on any .py files modified or added in the git status
* git-rank-contributors - William Morgan <wmorgan-git-wt-add@masanjin.net>
* git-rebase-authors - Mislav Marohnić's [dotfiles](https://github.com/mislav/dotfiles)
* git-rel - Ryan Tomayko's [dotfiles](http://github.com/rtomayko/dotfiles)
* git-run-command-on-revisions - Gary Bernhardt's [dotfiles](https://github.com/garybernhardt/dotfiles)
* git-shamend - Danielle Sucher's [git-shamend](http://www.daniellesucher.com/2014/05/08/git-shamend/) blog post
* git-show-overwritten - Mislav Marohnić's [dotfiles](https://github.com/mislav/dotfiles)
* git-submodule-rm - Greg V's [dotfiles](https://github.com/myfreeweb/dotfiles)
* git-thanks - Mislav Marohnić's [dotfiles](https://github.com/mislav/dotfiles)
* git-track - Zach Holman's [dotfiles](https://github.com/holman/dotfiles)
* git-trail - Daniel Hahler's [dotfiles](https://github.com/blueyed/dotfiles/blob/master/usr/bin/git-trail)
* git-undo-push -
* git-unpushed - Zach Holman's [dotfiles](https://github.com/holman/dotfiles)
* git-unreleased - Mislav Marohnić's [dotfiles](https://github.com/mislav/dotfiles)
* git-up - Ryan Tomayko's [dotfiles](http://github.com/rtomayko/dotfiles)
* git-upstream-sync - One of my personal scripts
* git-when-merged - Michael Haggerty [git-when-merged](https://github.com/mhagger/git-when-merged)
* git-where - Mislav Marohnić's [dotfiles](https://github.com/mislav/dotfiles)
* git-winner - Garry Dolley [https://github.com/up_the_irons/git-winner](https://github.com/up_the_irons/git-winner)
* git-wtf - William Morgan <wmorgan at the masanjin dot nets>
* github-open - Ryan Tomayko's [dotfiles](http://github.com/rtomayko/dotfiles)

## Contributing

Please include an entry in the credits section of README.md for any scripts in your PRs so authors get their work credited correctly. Please use `#!/usr/bin/env interpreter` instead of a direct path to the interpreter, this makes it easier for people to use more recent versions when the ones packaged with their OS (OS X, I'm looking at you) are stale.
