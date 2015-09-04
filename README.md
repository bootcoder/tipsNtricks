# Tip && Tricks
## For the JR Dev in your life.

**Literally** every thing below is IMHO




### Pro Tip Numero Uno

__HANDS OFF THE F*&^%ING MOUSE!!!__

As a developer your time is a __Super Valuable Resource__...

So every little thing you can do to increase efficiency will pay vast dividends over the course of your career.

You rarely need to actually touch the mouse. Every time you do you must take your hands complete off the keyboard. Grab the mouse. Go click the thing, then transfer back to the keyboard, find the home-row and finally start typing again...Precious seconds that add up to a huge savings.

It won't be easy but start building this skill now. Force yourself to leave the mouse behind. You're better than that mouse. You don't need no stinkin mouse. You have *Dev Hands*!!!


Also worth noting that sublimes ```⌘ p``` is hands down the fastest way to get around a working directory.

### How to search
Possibly the most important thing you will learn here.

See rule number 1. Any time you are leaving the keyboard you are losing time.
  - ⌘ + t -- open a new tab
  - Enter search terms. The first word of your search should always be the language you are looking for.
  - ⏎ -- to search google
  - tab this will take focus from the search bar and place it in the results list. You know you're there because a little blue arrow will appear next to the first result.
  - open the first 5 links into new tabs
    - ⌘ + ⏎ -- to open link
    - down arrow -- to go to next link
  - Cycle through tabs using

    ⌘ + ⇧ + {

    ⌘ + ⇧ + }
  - ⌘ + w -- Close unwanted tabs

### General stuff
  - Use Spotlight ⌘ + spacebar to search your system for files and applications.



### Take care of yourself

This job can be very grueling. Your personal sanity is a thing you should be mindful of always.
  - Eat well
  - Exercise often
  - Yoga is great
  - Work life balance (**after dbc**) is super important
  - Always remember __You are not your Code__
  - Talk to yourself... A LOT

### Take care of your pair
  - They're fragile too.

### Follow the Golden Rule of BLOCKS
As soon as you __OPEN__ the block __CLOSE__ the block.
```ruby

def thing_func

end

thingy.each do

end

{ }

[ ]

```

### Code readability BEATS conciseness 10.times out of 10
This means writing functions that are easy for developers to read. Not just you, but the people that maintain your code down the road.

Don't one line a thing because you want to look cool.

Indentation - OMG do this. All the time. No matter what. Lots of languages are whitespace dependent, meaning you must indent correctly. Better to establish this habit now.

![MaintainYourShit](./readability.jpeg "Fer Realsies")

### File Organization
Good habits when it comes to naming and storing files is something that will pay off big time for you in the long run.

Don't keep you files on the desktop.

Spend some time to figure out a good file structure that works for you. Once you make a plan stick to it. Down the road you will have  away easier time tracking down projects because they will have been placed in to your structure by some standard of your creation.

### Git Workflow

Commit early and often
  - Build test through a feature
  - Commit
  - Pass all tests for a feature
  - Commit

### Chrome Extensions
[Recomendations](https://github.com/bootcoder/htc_dev_settings/blob/master/chrome_extensions.md)

### Hot Key your iTerm2
```⌘ + \``` is what I use.

Also.... Use iTerm2 instead of terminal.

Get comfy with the pref here.
  - Increase buffer size
  - Increase Transparency
  - Make a jazzy color scheme that works for you and you alone.

## Sublime

### Packages
  * Package Manager
  * Better CoffeeScript
  * BracketHighlighter
  * ERB Snippets
  * GitGutter
  * Haml
  * JSLint
  * Markdown HTML Preview
  * Package Control
  * PowerCursors
  * SideBarEnhancements
  * sublime-github
  * SublimeLinter
  * SublimeLinter-haml
  * TernJS
  * Theme - Brogrammer
  * Tomorrow Color Scheme

### Sublime Shortcuts
[Complete List](http://sublime-text-unofficial-documentation.readthedocs.org/en/latest/reference/keyboard_shortcuts_osx.html)

Super useful ones
- move lines vertically
- jump to line
- jump to file
- global search
- duplicate line
- select word (and repeat)
- commenting code

### Linters
The good the bad and the ugly

Pros
  - help you see errors in your code
  - give you tips on best practices
  - easy to use

Cons
  - can cause stability issues with Sublime
  - others best practices may not always align with your own.

## General Stuff

### NO SUDO NO(despite what the internet tell you)
Short and sweet. If you are using ```sudo``` to install something on your mac....

__You're doing it WRONG__

Ask for help.
Installing something, check for a homebrew formula as your first option.

### APPS (osx)
  - Flycut (clipboard management)
  - Spectacle (window management)
  - Dropbox
  - Alfred
  - Dash
  - iTerm2
  - PostMan REST Client

### Gems (Don't even think about this list till late phase 2 minimum.)
  - bropages(gem)
  - haml
  - guard-rspec
  - guard-livereload
  - guard-spork
  - pry-byebug
  - pry-doc
  - better_errors
  - binding_of_caller
  - dotenv
  - ghrepo


### Links
[Tips for JR Devs](https://blog.newrelic.com/2014/04/23/better-junior-developer/)

[10 Tips to transition from JR to MID level Dev](http://www.techrepublic.com/blog/software-engineer/10-tips-to-go-from-a-beginner-to-an-intermediate-developer/)


[explainshell](http://explainshell.com/)



### Symbol Key
  - ⌘ – the Command Key symbol
  - ⇥ – the Tab Key symbol
  - ⌥ – the Option Key symbol
  - ⇧ – the Shift Key symbol
  - ⏎ – the Return symbol


## Config Stuff

### BASH TIPS
  - control + r == reverse search
  - history
  - man + / for search
  - fn + leftArrow || fn + rightArrow key for front or end of line

### BASH Aliases
```bash
alias e=subl
alias be="bundle exec"
alias g=git
alias cl=clear
alias ga="git ca"
alias gpo="git push origin"
alias gph="git push heroku"
alias db:reset="be rake db:drop && be rake db:create && be rake db:migrate && be rake db:test:prepare && be rake db:seed && rails c"
alias rials="rails"
alias gti="git"
alias shitgun="shotgun"
alias shotfun="shotgun"
alias dbc="cd ~/Dropbox/ACODE/DBC/dayJerbs"
alias code="cd ~/Dropbox/ACODE/adBC
```

### GIT Config
```bash
[core]
  # Excludesfiles allows us to set a global list of things to ignore
  excludesfile = ~/.gitignore_global

# These are custom color options for the console
[color]
  status = auto
  diff = auto

[color "status"]
  untracked = cyan
  changed = green
  added = yellow

# Aliases are command shortcuts
[alias]

  # lg is now a shortcut for a pretty log with short commit messages
  # See the log manpage: https://www.kernel.org/pub/software/scm/git/docs/git-log.html
  # for explanations of what these options do

  lg = log --graph --pretty=format:'%Cred%h%Creset -%C(yellow)%d%Creset %s %Cgreen(%cr) %C(bold blue)<%an>%Creset' --abbrev-commit --date=relative

  # Shorthand for a less noisy status
  s = commit --dry-run --short

  # More sensible names for adding and removing files from the readme
  stage = add
  unstage = reset HEAD

  # Edit the last commit
  amend= commit --verbose --amend

  # one-line log
  l = log --pretty=format:"%C(yellow)%h\\ %ad%Cred%d\\ %Creset%s%Cblue\\ [%cn]" --decorate --date=short

  a = add
  ap = add -p
  c = commit --verbose
  ca = commit -a --verbose
  cm = commit -m
  cam = commit -a -m
  m = commit --amend --verbose

  d = diff
  ds = diff --stat
  dc = diff --cached

  co = checkout
  cob = checkout -b

  # list branches sorted by last modified
  b = "!git for-each-ref --sort='-authordate' --format='%(authordate)%09%(objectname:short)%09%(refname)' refs/heads | sed -e 's-refs/heads/--'"

  # list aliases
  la = "!git config -l | grep alias"
[user]
  email = bootcoder@gmail.com
  name = BootCoder
[credential]
  helper = cache --timeout=14400

```







