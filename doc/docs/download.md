# Download

`csvtk` is implemented in [Go](https://golang.org/) programming language,
 executable binary files **for most popular operating system** are freely available
  in [release](https://github.com/shenwei356/csvtk/releases) page.

## Current Version

[csvtk v0.11.0](https://github.com/shenwei356/csvtk/releases/tag/v0.11.0)
[![Github Releases (by Release)](https://img.shields.io/github/downloads/shenwei356/csvtk/v0.11.0/total.svg)](https://github.com/shenwei356/csvtk/releases/tag/v0.11.0)

- add command `split` to split CSV/TSV into multiple files according to column values
- add command `splitxlxs` to split XLSX sheet into multiple sheets according to column values
- `csvtk`, automatically check BOM (byte-order mark) and discard it

Links:

***Tips***

- run `csvtk version` to check update !!!
- run `csvtk genautocomplete` to update Bash completion !!!

OS     |Arch      |File, 中国镜像                                                                                                                                                                              |Download Count
:------|:---------|:-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|:-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
Linux  |32-bit    |[csvtk_linux_386.tar.gz](https://github.com/shenwei356/csvtk/releases/download/v0.11.0/csvtk_linux_386.tar.gz),<br/> [中国镜像](http://app.shenwei.me/data/csvtk/csvtk_linux_386.tar.gz)                            |[![Github Releases (by Asset)](https://img.shields.io/github/downloads/shenwei356/csvtk/latest/csvtk_linux_386.tar.gz.svg?maxAge=3600)](https://github.com/shenwei356/csvtk/releases/download/v0.11.0/csvtk_linux_386.tar.gz)
Linux  |**64-bit**|[**csvtk_linux_amd64.tar.gz**](https://github.com/shenwei356/csvtk/releases/download/v0.11.0/csvtk_linux_amd64.tar.gz),<br/> [中国镜像](http://app.shenwei.me/data/csvtk/csvtk_linux_amd64.tar.gz)                  |[![Github Releases (by Asset)](https://img.shields.io/github/downloads/shenwei356/csvtk/latest/csvtk_linux_amd64.tar.gz.svg?maxAge=3600)](https://github.com/shenwei356/csvtk/releases/download/v0.11.0/csvtk_linux_amd64.tar.gz)
OS X   |32-bit    |[csvtk_darwin_386.tar.gz](https://github.com/shenwei356/csvtk/releases/download/v0.11.0/csvtk_darwin_386.tar.gz),<br/> [中国镜像](http://app.shenwei.me/data/csvtk/csvtk_darwin_386.tar.gz)                         |[![Github Releases (by Asset)](https://img.shields.io/github/downloads/shenwei356/csvtk/latest/csvtk_darwin_386.tar.gz.svg?maxAge=3600)](https://github.com/shenwei356/csvtk/releases/download/v0.11.0/csvtk_darwin_386.tar.gz)
OS X   |**64-bit**|[**csvtk_darwin_amd64.tar.gz**](https://github.com/shenwei356/csvtk/releases/download/v0.11.0/csvtk_darwin_amd64.tar.gz),<br/> [中国镜像](http://app.shenwei.me/data/csvtk/csvtk_darwin_amd64.tar.gz)               |[![Github Releases (by Asset)](https://img.shields.io/github/downloads/shenwei356/csvtk/latest/csvtk_darwin_amd64.tar.gz.svg?maxAge=3600)](https://github.com/shenwei356/csvtk/releases/download/v0.11.0/csvtk_darwin_amd64.tar.gz)
Windows|32-bit    |[csvtk_windows_386.exe.tar.gz](https://github.com/shenwei356/csvtk/releases/download/v0.11.0/csvtk_windows_386.exe.tar.gz),<br/> [中国镜像](http://app.shenwei.me/data/csvtk/csvtk_windows_386.exe.tar.gz)          |[![Github Releases (by Asset)](https://img.shields.io/github/downloads/shenwei356/csvtk/latest/csvtk_windows_386.exe.tar.gz.svg?maxAge=3600)](https://github.com/shenwei356/csvtk/releases/download/v0.11.0/csvtk_windows_386.exe.tar.gz)
Windows|**64-bit**|[**csvtk_windows_amd64.exe.tar.gz**](https://github.com/shenwei356/csvtk/releases/download/v0.11.0/csvtk_windows_amd64.exe.tar.gz),<br/> [中国镜像](http://app.shenwei.me/data/csvtk/csvtk_windows_amd64.exe.tar.gz)|[![Github Releases (by Asset)](https://img.shields.io/github/downloads/shenwei356/csvtk/latest/csvtk_windows_amd64.exe.tar.gz.svg?maxAge=3600)](https://github.com/shenwei356/csvtk/releases/download/v0.11.0/csvtk_windows_amd64.exe.tar.gz)

## Installation

[Download Page](https://github.com/shenwei356/csvtk/releases)

`csvtk` is implemented in [Go](https://golang.org/) programming language,
 executable binary files **for most popular operating systems** are freely available
  in [release](https://github.com/shenwei356/csvtk/releases) page.

#### Method 1: Download binaries

Just [download](https://github.com/shenwei356/csvtk/releases) compressed
executable file of your operating system,
and decompress it with `tar -zxvf *.tar.gz` command or other tools.
And then:

1. **For Linux-like systems**
    1. If you have root privilege simply copy it to `/usr/local/bin`:

            sudo cp csvtk /usr/local/bin/

    1. Or add the current directory of the executable file to environment variable
    `PATH`:

            echo export PATH=\$PATH:\"$(pwd)\" >> ~/.bashrc
            source ~/.bashrc


1. **For windows**, just copy `csvtk.exe` to `C:\WINDOWS\system32`.

#### Method 2: Install via conda [![Install-with-conda](https://anaconda.org/bioconda/csvtk/badges/installer/conda.svg)](http://bioinf.shenwei.me/csvtk/download/) [![Anaconda Cloud](	https://anaconda.org/bioconda/csvtk/badges/version.svg)](https://anaconda.org/bioconda/csvtk) [![downloads](https://anaconda.org/bioconda/csvtk/badges/downloads.svg)](https://anaconda.org/bioconda/csvtk)

    conda install -c bioconda csvtk

#### Method 3: For Go developer

    go get -u github.com/shenwei356/csvtk/csvtk

#### Method 4: For ArchLinux AUR users

    yaourt -S csvtk

## Bash-completion

Note: The current version supports Bash only.
This should work for *nix systems with Bash installed.

Howto:

1. run: `csvtk genautocomplete`

2. create and edit `~/.bash_completion` file if you don't have it.

        nano ~/.bash_completion

    add the following:

        for bcfile in ~/.bash_completion.d/* ; do
          . $bcfile
        done

## Previous Versions

- [csvtk v0.10.0](https://github.com/shenwei356/csvtk/releases/tag/v0.10.0)
[![Github Releases (by Release)](https://img.shields.io/github/downloads/shenwei356/csvtk/v0.10.0/total.svg)](https://github.com/shenwei356/csvtk/releases/tag/v0.10.0)
    - add subcommand `xlsx2csv` to convert XLSX to CSV format
    - `grep`, `filter`, `filter2`: add flag `-n/--line-number` to print line-number as the first column
    - `cut`: add flag `-i/--ignore-case` to ignore case of column name
- [csvtk v0.9.1](https://github.com/shenwei356/csvtk/releases/tag/v0.9.1)
[![Github Releases (by Release)](https://img.shields.io/github/downloads/shenwei356/csvtk/v0.9.1/total.svg)](https://github.com/shenwei356/csvtk/releases/tag/v0.9.1)
    - `csvtk replace`: fix bug when replacing with key-value pairs brought in v0.8.0
- [csvtk v0.9.0](https://github.com/shenwei356/csvtk/releases/tag/v0.9.0)
[![Github Releases (by Release)](https://img.shields.io/github/downloads/shenwei356/csvtk/v0.9.0/total.svg)](https://github.com/shenwei356/csvtk/releases/tag/v0.9.0)
    - add subcommand `csvtk mutate2`: create new column from selected fields by **awk-like artithmetic/string expressions**
    - add new command `genautocomplete` to generate **shell autocompletion** script!
- [csvtk v0.8.0](https://github.com/shenwei356/csvtk/releases/tag/v0.8.0)
[![Github Releases (by Release)](https://img.shields.io/github/downloads/shenwei356/csvtk/v0.8.0/total.svg)](https://github.com/shenwei356/csvtk/releases/tag/v0.8.0)
    - **new command `csvtk gather` for gathering columns into key-value pairs**.
    - `csvtk sort`: support **sorting by user-defined order**.
    - fix bug of *unselecting field*: wrongly reporting error of fields not existing.
    affected commands: `cut`, `filter`, `fitler2`, `freq`, `grep`, `inter`, `mutate`,
    `rename`, `rename2`, `replace`, `stats2`, `uniq`.
    - update help message of flag `-F/--fuzzy-fields`.
    - update help message of global flag `-t`, which overrides both `-d` and `-D`.
      If you want other delimiter for tabular input, use `-t $'\t' -D "delimiter"`.
- [csvtk v0.7.1](https://github.com/shenwei356/csvtk/releases/tag/v0.7.1)
[![Github Releases (by Release)](https://img.shields.io/github/downloads/shenwei356/csvtk/v0.7.1/total.svg)](https://github.com/shenwei356/csvtk/releases/tag/v0.7.1)
    - `csvtk plot box` and `csvtk plot line`: fix bugs for special cases of input
    - compile with go1.8.1
- [csvtk v0.7.0](https://github.com/shenwei356/csvtk/releases/tag/v0.7.0)
[![Github Releases (by Release)](https://img.shields.io/github/downloads/shenwei356/csvtk/v0.7.0/total.svg)](https://github.com/shenwei356/csvtk/releases/tag/v0.7.0)
    - fig bug of "stricter field checking" in v0.6.0 and v0.6.1 when using flag `-F/--fuzzy-fields`
    - `csvtk pretty` and `csvtk csv2md`: add attention that
      these commands treat the first row as header line and require them to be unique.
    - `csvtk stat` renamed to `csvtk stats`, old name is still available as an alias.
    - `csvtk stat2` renamed to `csvtk stats2`, old name is still available as an alias.
    - [issues/13](https://github.com/shenwei356/csvtk/issues/13) **seamlessly support for data with meta line of separator declaration used by MS Excel**.
- [csvtk v0.6.1](https://github.com/shenwei356/csvtk/releases/tag/v0.6.1)
[![Github Releases (by Release)](https://img.shields.io/github/downloads/shenwei356/csvtk/v0.6.1/total.svg)](https://github.com/shenwei356/csvtk/releases/tag/v0.6.1)
    - `csvtk cut`: minor bug: panic when no fields given. i.e., `csvtk cut`.
All relevant commands have been fixed.
- [csvtk v0.6.0](https://github.com/shenwei356/csvtk/releases/tag/v0.6.0)
[![Github Releases (by Release)](https://img.shields.io/github/downloads/shenwei356/csvtk/v0.6.0/total.svg)](https://github.com/shenwei356/csvtk/releases/tag/v0.6.0)
    - `csvtk grep`: **large performance improvement by discarding goroutine** (multiple threads),
      and **keeping output in order of input**.
    - Better column name checking and **stricter field checking,
      fields out of range are not ignored now**.
      Affected commands include `cut`, `filter`, `freq`, `grep`, `inter`, `mutate`,
      `rename`, `rename2`, `replace`, `stat2`, and `uniq`.
    - **New command: `csvtk filter2`, filtering rows by artithmetic/string expressions like `awk`**.
- [csvtk v0.5.0](https://github.com/shenwei356/csvtk/releases/tag/v0.5.0)
[![Github Releases (by Release)](https://img.shields.io/github/downloads/shenwei356/csvtk/v0.5.0/total.svg)](https://github.com/shenwei356/csvtk/releases/tag/v0.5.0)
    - `csvtk cut`: delete flag `-n/--names`, move it to a new command `csvtk headers`
    - new command: `csvtk headers`
    - new command: `csvtk head`
    - new command: `csvtk sample`
- [csvtk v0.4.6](https://github.com/shenwei356/csvtk/releases/tag/v0.4.6)
[![Github Releases (by Release)](https://img.shields.io/github/downloads/shenwei356/csvtk/v0.4.6/total.svg)](https://github.com/shenwei356/csvtk/releases/tag/v0.4.6)
    - `csvtk grep`: fix result highlight when flag `-v` is on.
- [csvtk v0.4.5](https://github.com/shenwei356/csvtk/releases/tag/v0.4.5)
[![Github Releases (by Release)](https://img.shields.io/github/downloads/shenwei356/csvtk/v0.4.5/total.svg)](https://github.com/shenwei356/csvtk/releases/tag/v0.4.5)
    - `csvtk join`: support the 2nd or later files with entries with same ID.
- [csvtk v0.4.4](https://github.com/shenwei356/csvtk/releases/tag/v0.4.4)
[![Github Releases (by Release)](https://img.shields.io/github/downloads/shenwei356/csvtk/v0.4.4/total.svg)](https://github.com/shenwei356/csvtk/releases/tag/v0.4.4)
    - add command `csvtk freq`: frequencies of selected fields
    - add lots of examples in [usage page](http://bioinf.shenwei.me/csvtk/usage/)
- [csvtk v0.4.3](https://github.com/shenwei356/csvtk/releases/tag/v0.4.3)
[![Github Releases (by Release)](https://img.shields.io/github/downloads/shenwei356/csvtk/v0.4.3/total.svg)](https://github.com/shenwei356/csvtk/releases/tag/v0.4.3)
    - improvement of using experience: flag `-n` is not required anymore when flag `-H` in `csvtk mutate`
- [csvtk v0.4.2](https://github.com/shenwei356/csvtk/releases/tag/v0.4.2)
[![Github Releases (by Release)](https://img.shields.io/github/downloads/shenwei356/csvtk/v0.4.2/total.svg)](https://github.com/shenwei356/csvtk/releases/tag/v0.4.2)
    - fix highlight bug of `csvtk grep`: if the pattern matches multiple parts,
    the text will be wrongly edited.
    - changes: disable highlight when pattern file given.
    - change the default output of all ploting commands to STDOUT, now you can
    pipe the image to "display" command of Imagemagic.
- [csvtk v0.4.1](https://github.com/shenwei356/csvtk/releases/tag/v0.4.1)
[![Github Releases (by Release)](https://img.shields.io/github/downloads/shenwei356/csvtk/v0.4.1/total.svg)](https://github.com/shenwei356/csvtk/releases/tag/v0.4.1)
    - Nothing changed. Just fix the links due to inappropriate deployment of v0.4.0
- [csvtk v0.4.0](https://github.com/shenwei356/csvtk/releases/tag/v0.4.0)
[![Github Releases (by Release)](https://img.shields.io/github/downloads/shenwei356/csvtk/v0.4.0/total.svg)](https://github.com/shenwei356/csvtk/releases/tag/v0.4.0)
    - add flag for `csvtk replace`: `-K` (`--keep-key`) keep the key as value when
    no value found for the key. This is open in default in previous versions.
- [csvtk v0.3.9](https://github.com/shenwei356/csvtk/releases/tag/v0.3.9)
  [![Github Releases (by Release)](https://img.shields.io/github/downloads/shenwei356/csvtk/v0.3.9/total.svg)](https://github.com/shenwei356/csvtk/releases/tag/v0.4.0)
    - fix bug: header row incomplete in `csvtk sort` result
- [csvtk v0.3.8.1](https://github.com/shenwei356/csvtk/releases/tag/v0.3.8.1)
  [![Github Releases (by Release)](https://img.shields.io/github/downloads/shenwei356/csvtk/v0.3.8.1/total.svg)](https://github.com/shenwei356/csvtk/releases/tag/v0.3.8.1)
    - fix bug of flag parsing library [pflag](https://github.com/spf13/pflag),
    [detail](https://github.com/spf13/pflag/pull/98).
    The bug affected the `csvtk grep -r -p`, when value of `-p` contain "[" and "]"
    at the beginning or end, they are wrongly parsed.
- [csvtk v0.3.8](https://github.com/shenwei356/csvtk/releases/tag/v0.3.8)
  [![Github Releases (by Release)](https://img.shields.io/github/downloads/shenwei356/csvtk/v0.3.8/total.svg)](https://github.com/shenwei356/csvtk/releases/tag/v0.3.8)
    - new feature: `csvtk cut` supports ordered fields output. e.g., `csvtk cut -f 2,1`
      outputs the 2nd column in front of 1th column.
    - new commands: `csvtk plot` can plot three types of plots by subcommands:
        - `csvtk plot hist`: histogram
        - `csvtk plot box`: boxplot
        - `csvtk plot line`: line plot and scatter plot
- [csvtk v0.3.7](https://github.com/shenwei356/csvtk/releases/tag/v0.3.7)
  [![Github Releases (by Release)](https://img.shields.io/github/downloads/shenwei356/csvtk/v0.3.7/total.svg)](https://github.com/shenwei356/csvtk/releases/tag/v0.3.7)
    - fix a serious bug of using negative field of column name, e.g. `-f "-id"`
- [csvtk v0.3.6](https://github.com/shenwei356/csvtk/releases/tag/v0.3.6)
  [![Github Releases (by Release)](https://img.shields.io/github/downloads/shenwei356/csvtk/v0.3.6/total.svg)](https://github.com/shenwei356/csvtk/releases/tag/v0.3.6)
    - `csvtk replace` support replacement symbols `{nr}` (record number)
      and `{kv}` (corresponding value of the key ($1) by key-value file)
- [csvtk v0.3.5.2](https://github.com/shenwei356/csvtk/releases/tag/v0.5.2)
  [![Github Releases (by Release)](https://img.shields.io/github/downloads/shenwei356/csvtk/v0.3.5.2/total.svg)](https://github.com/shenwei356/csvtk/releases/tag/v0.3.5.2)
    - add flag `--fill` for `csvtk join`, so we can fill the unmatched data
    - fix typo
- [csvtk v0.3.5.1](https://github.com/shenwei356/csvtk/releases/tag/v0.3.5.1)
  [![Github Releases (by Release)](https://img.shields.io/github/downloads/shenwei356/csvtk/v0.3.5.1/total.svg)](https://github.com/shenwei356/csvtk/releases/tag/v0.3.5.1)
    - fix minor bug of reading lines ending with `\r\n` from a dependency package
- [csvtk v0.3.5](https://github.com/shenwei356/csvtk/releases/tag/v0.3.5)
  [![Github Releases (by Release)](https://img.shields.io/github/downloads/shenwei356/csvtk/v0.3.5/total.svg)](https://github.com/shenwei356/csvtk/releases/tag/v0.3.5)
    - fix minor bug of `csv2md`
    - add subcommand `version` which could check for update
- [csvtk v0.3.4](https://github.com/shenwei356/csvtk/releases/tag/v0.3.4)
  [![Github Releases (by Release)](https://img.shields.io/github/downloads/shenwei356/csvtk/v0.3.4/total.svg)](https://github.com/shenwei356/csvtk/releases/tag/v0.3.4)
    - fix bug of `csvtk replace` that head row should not be edited.
- [csvtk v0.3.3](https://github.com/shenwei356/csvtk/releases/tag/v0.3.3)
  [![Github Releases (by Release)](https://img.shields.io/github/downloads/shenwei356/csvtk/v0.3.3/total.svg)](https://github.com/shenwei356/csvtk/releases/tag/v0.3.3)
    - fix bug of `csvtk grep -t -P`
- [csvtk v0.3.2](https://github.com/shenwei356/csvtk/releases/tag/v0.3.2)
  [![Github Releases (by Release)](https://img.shields.io/github/downloads/shenwei356/csvtk/v0.3.2/total.svg)](https://github.com/shenwei356/csvtk/releases/tag/v0.3.2)
    - fix bug of `inter`
- [csvtk v0.3.1](https://github.com/shenwei356/csvtk/releases/tag/v0.3.1)
  [![Github Releases (by Release)](https://img.shields.io/github/downloads/shenwei356/csvtk/v0.3.1/total.svg)](https://github.com/shenwei356/csvtk/releases/tag/v0.3.1)
    - add support of search multiple fields for `grep`
- [csvtk v0.3](https://github.com/shenwei356/csvtk/releases/tag/v0.3)
  [![Github Releases (by Release)](https://img.shields.io/github/downloads/shenwei356/csvtk/v0.3/total.svg)](https://github.com/shenwei356/csvtk/releases/tag/v0.3)
    - add subcommand `csv2md`
- [csvtk v0.2.9](https://github.com/shenwei356/csvtk/releases/tag/v0.2.9)
  [![Github Releases (by Release)](https://img.shields.io/github/downloads/shenwei356/csvtk/v0.2.9/total.svg)](https://github.com/shenwei356/csvtk/releases/tag/v0.2.9)
    - add more flags to subcommand `pretty`
    - fix bug of `csvtk cut -n`
    - add subcommand `filter`
- [csvtk v0.2.8](https://github.com/shenwei356/csvtk/releases/tag/v0.2.8)
  [![Github Releases (by Release)](https://img.shields.io/github/downloads/shenwei356/csvtk/v0.2.8/total.svg)](https://github.com/shenwei356/csvtk/releases/tag/v0.2.8)
    - add subcommand `pretty` -- convert CSV to readable aligned table
- [csvtk v0.2.7](https://github.com/shenwei356/csvtk/releases/tag/v0.2.7)
  [![Github Releases (by Release)](https://img.shields.io/github/downloads/shenwei356/csvtk/v0.2.7/total.svg)](https://github.com/shenwei356/csvtk/releases/tag/v0.2.7)
    - fix highlight failing in windows
- [csvtk v0.2.6](https://github.com/shenwei356/csvtk/releases/tag/v0.2.6)
  [![Github Releases (by Release)](https://img.shields.io/github/downloads/shenwei356/csvtk/v0.2.6/total.svg)](https://github.com/shenwei356/csvtk/releases/tag/v0.2.6)
    - fix one error message of `grep`
    - highlight matched fields in result of `grep`
- [csvtk v0.2.5](https://github.com/shenwei356/csvtk/releases/tag/v0.2.5)
  [![Github Releases (by Release)](https://img.shields.io/github/downloads/shenwei356/csvtk/v0.2.5/total.svg)](https://github.com/shenwei356/csvtk/releases/tag/v0.2.5)
    - fix bug of `stat` that failed to considerate files with header row
    - add subcommand `stat2` - summary of selected number fields
    - make the output of `stat` prettier
- [csvtk v0.2.4](https://github.com/shenwei356/csvtk/releases/tag/v0.2.4)
  [![Github Releases (by Release)](https://img.shields.io/github/downloads/shenwei356/csvtk/v0.2.4/total.svg)](https://github.com/shenwei356/csvtk/releases/tag/v0.2.4)
    - fix bug of handling comment lines
    - add some notes before using csvtk
- [csvtk v0.2.3](https://github.com/shenwei356/csvtk/releases/tag/v0.2.3)
  [![Github Releases (by Release)](https://img.shields.io/github/downloads/shenwei356/csvtk/v0.2.3/total.svg)](https://github.com/shenwei356/csvtk/releases/tag/v0.2.3)
    - add flag `--colnames` to `cut`
    - flag `-f` (`--fields`) of `join` supports single value now
- [csvtk v0.2.2](https://github.com/shenwei356/csvtk/releases/tag/v0.2.2)
  [![Github Releases (by Release)](https://img.shields.io/github/downloads/shenwei356/csvtk/v0.2.2/total.svg)](https://github.com/shenwei356/csvtk/releases/tag/v0.2.2)
    - add flag `--keep-unmathed` to `join`
- [csvtk v0.2](https://github.com/shenwei356/csvtk/releases/tag/v0.2)
  [![Github Releases (by Release)](https://img.shields.io/github/downloads/shenwei356/csvtk/v0.2/total.svg)](https://github.com/shenwei356/csvtk/releases/tag/v0.2)
    - finish almost functions
- [csvtk v0.2.1](https://github.com/shenwei356/csvtk/releases/tag/v0.2.1)
  [![Github Releases (by Release)](https://img.shields.io/github/downloads/shenwei356/csvtk/v0.2.1/total.svg)](https://github.com/shenwei356/csvtk/releases/tag/v0.2.1)
    - fix bug of `mutate`


<div id="disqus_thread"></div>
<script>
/**
* RECOMMENDED CONFIGURATION VARIABLES: EDIT AND UNCOMMENT THE SECTION BELOW TO INSERT DYNAMIC VALUES FROM YOUR PLATFORM OR CMS.
* LEARN WHY DEFINING THESE VARIABLES IS IMPORTANT: https://disqus.com/admin/universalcode/#configuration-variables
*/
/*
var disqus_config = function () {
this.page.url = PAGE_URL; // Replace PAGE_URL with your page's canonical URL variable
this.page.identifier = PAGE_IDENTIFIER; // Replace PAGE_IDENTIFIER with your page's unique identifier variable
};
*/
(function() { // DON'T EDIT BELOW THIS LINE
var d = document, s = d.createElement('script');

s.src = '//csvtk.disqus.com/embed.js';

s.setAttribute('data-timestamp', +new Date());
(d.head || d.body).appendChild(s);
})();
</script>
<noscript>Please enable JavaScript to view the <a href="https://disqus.com/?ref_noscript" rel="nofollow">comments powered by Disqus.</a></noscript>
