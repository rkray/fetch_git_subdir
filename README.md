# fetch_git_subdir

Overview
========

Short helper script do fetch a subdir from a remote git respective gitlab repository.


Usage
=====

    Usage: fetch_git_subdir [options]
        -h, --help                       Prints this help
        -d, --debug                      enable debug mode
        -v, --verbose                    enable verbose printing
        -u, --username USERNAME          set username
        -p, --passvarname NAME           the name with the environment variable
                                         default is GITPASS. If no environment
                                         variable is set, the programm tries to
                                         read the password from stdin.
        -r, --repository URI             HTTP/HTTPS repository URL as shown by gitlab
                                         project page
        -a, --path PATH                  fetch all files from PATH

      Examples:
        # read password from environment
        PASS=123 fetch_git_subdir -p PASS -u user -r https://...

        # read password from stdin
        echo 123 | ssh user@host 'fetch_git_subdir -u user -r https://...'

        # example repo url
        fetch_git_subdir -r https://gitlab.mydomain.com/team/testapi.git
