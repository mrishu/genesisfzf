# genesisfzf
![](libg.gif)

**Library Genesis TUI** using **fzf**.  
Using this, you can search the library genesis site, filter your book out using `fzf` as well as download the selected book by just pressing `Enter`; everything right from your terminal!

## Usage
`libg [OPTIONS] <search query>`

### Options:
```
OPTIONS        Description                               Allowed Values
-------        -----------                               --------------
-b <value>     Search By                                 author, title, publisher, year, isbn, language, md5, tags, extension.
-n <value>     Number of Search Results per Page         25, 50, 100.
-d <value>     Depth (Number of result pages to scan)    Any positive integer.
-s <value>     Sort Results By                           id, author, title, publisher, year, pages, language, filesize, extension.
-r             Reverse/Desecending Order
```

## Installation
Since it is just a small shell script, just download the script, give it executable permissions and place it in a directory that is in `PATH`. Also, you can change the default values for each option in the first few lines of the script.  
## Dependency
The only dependency is `fzf`: https://github.com/junegunn/fzf.   
The other dependencies are `sed`(GNU), `awk`, `curl` and `wget` but are present by default in most Linux installs. 

## Todos
1. Add option for selecting different mirrors.
