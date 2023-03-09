# Laptop

Laptop is a script to set up a macOS laptop for web and mobile development.

It can be run multiple times on the same machine safely.
It installs, upgrades, or skips packages
based on what is already installed on the machine.

This project is forked & derived from the [thoughtbot/laptop](https://github.com/thoughtbot/laptop) project, but customized for my own use.


## Install

Download the script:

```sh
curl --remote-name https://raw.githubusercontent.com/mutukrish/laptop_m1/main/mac
```

Review the script (avoid running scripts you haven’t read!):

```sh
less mac
```

Execute the downloaded script:

```sh
sh mac 2>&1 | tee ~/laptop.log
```

Optionally, review the log:

```sh
less ~/laptop.log
```

Your last Laptop run will be saved to `~/laptop.log`.

## What it sets up

First, it shows hidden (dot)files on your Mac.

macOS tools:

- [Homebrew] for managing operating system libraries.

[homebrew]: http://brew.sh/

Unix tools:

- [Universal Ctags] for indexing files for vim tab completion
- [Git] for version control
- [OpenSSL] for Transport Layer Security (TLS)
- [RCM] for managing company and personal dotfiles
- [The Silver Searcher] for finding things in files
- [Tmux] for saving project state and switching between projects
- [Watchman] for watching for filesystem events
- [Zsh] as your shell

[universal ctags]: https://ctags.io/
[git]: https://git-scm.com/
[openssl]: https://www.openssl.org/
[rcm]: https://github.com/thoughtbot/rcm
[the silver searcher]: https://github.com/ggreer/the_silver_searcher
[tmux]: http://tmux.github.io/
[watchman]: https://facebook.github.io/watchman/
[zsh]: http://www.zsh.org/

Heroku tools:

- [Heroku CLI] and [Parity] for interacting with the Heroku API

[heroku cli]: https://devcenter.heroku.com/articles/heroku-cli
[parity]: https://github.com/thoughtbot/parity

GitHub tools:

- [GitHub CLI] for interacting with the GitHub API

[github cli]: https://cli.github.com/

Image tools:

- [ImageMagick] for cropping and resizing images
- [Guetzli] for optimizing images

Programming languages, package managers, and configuration:

- [Bundler] for managing Ruby libraries
- [Node.js] (latest LTS version) & [npm], for running apps and installing JavaScript packages, via [tj/n]
- [Ruby] (latest stable version) via [rbenv]
- [Yarn] for managing JavaScript packages
- [NVM] Managing node version locally

[bundler]: http://bundler.io/
[imagemagick]: http://www.imagemagick.org/
[guetzli]: https://github.com/google/guetzli
[node.js]: http://nodejs.org/
[npm]: https://www.npmjs.org/
[tj/n]: https://github.com/tj/n
[ruby]: https://www.ruby-lang.org/en/
[rbenv]: https://rbenv.org
[yarn]: https://yarnpkg.com/en/
[nvm]: https://github.com/nvm-sh/nvm

Databases:

- [MongoDB] for storing data

[MongoDB]: https://www.mongodb.com/docs/manual/tutorial/install-mongodb-on-os-x/
[MongoDB Database Tools]: https://www.mongodb.com/docs/database-tools/installation/installation-macos/


## License

Laptop is © 2011-2020 thoughtbot, inc.
It is free software,
and may be redistributed under the terms specified in the [LICENSE] file.

[license]: LICENSE