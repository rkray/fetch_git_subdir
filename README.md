# fetch_git_subdir

Overview
========

Short helper script do fetch a subdir from a remote git respective gitlab repository.


Usage
=====

> Usage: fetch_git_subdir [options]
>     -d, --debug                      enable debug mode
>     -v, --verbose                    enable verbose logging
>     -m, --mode (gitlab|git)          set mode, default is 'gitlab'
>     -u, --username USERNAME          set username
>     -p, --passvarname NAME           set set the name with the environment variable
>                                      default is GITPASS
>                                      Example:
>                                        PASS=123 fetch_git_subdir -p PASS
>     -r, --repository URI             set repository URL
>                                      Example: fetch_git_subdir
>     -a, --path PATH                  fetch all files from PATH
>                                      Example: fetch_git_subdir
