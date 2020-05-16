# FZF

FZF is a command line fuzzy finder, that can work on any list. Typing

`FZF`

will start the interactive finder searching through files.

Running

`history | FZF`

will allow you to fuzzy search over command history

can use * * to activate in command line such as:

`cd src/**`

and can use 

``` 
vim -o `fzf`
```
to open the output of an interactive fzf search.
