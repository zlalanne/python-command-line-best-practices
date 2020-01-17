# python-command-line-best-practices

Repo for talk on Python command line best practices

## Planning

Outline

* About me
* Why we need tools
  * Make developers efficient
  * Make things more consistent
* Problem statement
  * Your CTO has heard about this awesome thing called Markdown. And they want everyone to use it to write documentation
  * Your developers need a tool to convert Markdown to HTML
  * You want to use your companies branding along the way
* So let's design a new tool
  * We want to read command line arguments
    * argparse
    * click
    * docopt
  * Add some arguments
    * --dark_mode
    * --table\_of\_contents
* Notes about command line arguments
  * Treat it like your API
    * Don't remove flags
  * Use unique error codes when it makes sense
* Be consistent with your flags
  * --version / --help
  * short and long form arguments are nice, most libraries will support this
  * use '-' for STDIN
* Adding feature flags
  * --experimental__new__theme
* Don't be too chatty
  * Add a verbose flag
* Making them easy to use
  * People have lots of different ways they like to use their tools.
  * make man pages
  * bash completion
* Make them easy to use with other tools
  * If you're in a Linux shop. Make things work with STDOUT/STDERR/STDIN
* Make them well tested
  * Import functions from your tools
  * call your tools, do "system-level" testing
  * pytest-datadir
  * pytest-tempdir
  * check exit codes
* Other stdlib/features to check out
  * tempfile / atexit
* Other references
  * [Exploring CLI Best Practices](https://eng.localytics.com/exploring-cli-best-practices/)
