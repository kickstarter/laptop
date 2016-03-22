# Laptop

Laptop is a script to set up an OS X computer for web development.

It can be run multiple times on the same machine safely.
It installs, upgrades, or skips packages
based on what is already installed on the machine.

## Install

In a terminal window, run: 

```sh
curl -Ls https://raw.githubusercontent.com/kickstarter/laptop/master/mac | sh
```

## Debugging

Read through the output to see if you can debug the issue yourself.
If not, copy the lines where the script failed into a
[new GitHub Issue](https://github.com/kickstarter/laptop/issues/new) for us.
Or, cut & paste the entire output into the issue.

## OS X El Capitan (10.11)

You may have problems installing Homebrew for the first time on OS X El
Capitan due to permission changes to the /usr directory (within which the Homebrew
installation is typically located). See the [Homebrew El Capitan troubleshooting instructions](https://github.com/Homebrew/homebrew/blob/master/share/doc/homebrew/El_Capitan_and_Homebrew.md)
for steps to resolve the permissions issues that interfere with Homebrew's
installation.

## What it sets up

Mac OS X tools:

* [Homebrew] for managing operating system libraries.

[Homebrew]: http://brew.sh/

Unix tools:

* [Git] for version control
* [n] for managing versions of node JS
* [Rbenv] and [Ruby Build] for managing versions of Ruby
* [Pow] for running local web services


[Git]: https://git-scm.com
[n]: https://www.npmjs.com/package/n
[Rbenv]: https://github.com/sstephenson/rbenv
[Ruby Build]: https://github.com/sstephenson/ruby-build
[Pow]: http://pow.cx

It should take less than 15 minutes to install from scratch  (depends on your machine), and about 2 seconds for subsequent runs.

### Contributing

Edit the `mac` file.
Document in the `README.md` file.
Follow shell style guidelines by using [ShellCheck] and [Syntastic].

```sh
brew install shellcheck
```

[ShellCheck]: http://www.shellcheck.net/about.html
[Syntastic]: https://github.com/scrooloose/syntastic

### Credits

The Kickstarter laptop script is based on and inspired by
[thoughtbot's laptop](https://github.com/thoughtbot/laptop) script.

### License

Original Laptop script © 2011-2016 thoughtbot, inc.

Modifications © Kickstarter, PBC.
[LICENSE]: LICENSE
