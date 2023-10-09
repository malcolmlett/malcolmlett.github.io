# GitHub Pages Site
This is the repository for my [Personal website](https://malcolmlett.github.io/), hosted courtesy of GitHub Pages.

This site is built with [Jekyll](https://jekyllrb.com/) and the [Just the Docs](https://just-the-docs.com/) theme.

# Running locally

The first time you run this, you'll need to follow the "one time setup" steps below.

Then:

1. Run jekyll

    ```shell
    $ bundle exec jekyll serve --force_polling
    ```
	
1. Open in a browser at http://localhost:4000


## Running locally - one time setup

The following steps configure Jekyll to run within Windows System for Linux.

Prerequisites:
* make sure you are on Ubuntu 20.04.5 LTS or later

    ```shell
    $ lsb_release -a
    ```

* Identify exactly which version of Ruby and Bundler is used in the GitHub Pages Actions in order to replicate the same environment locally.

Steps:

1. Install ruby-install as per https://github.com/postmodern/ruby-install#readme
    * tip: you can download to a Downloads folder, it'll install as a globally available command when running make.

1. Install ruby:
	
    ```shell
    $ ruby-install
    $ sudo ruby-install --system ruby 3.1.4       # or whichever version is used on GitHub Pages
    $ ruby -v
    ```

1. Update your `.bashrc` to point to a local folders for gems to be installed to, as per https://jekyllrb.com/docs/troubleshooting/#no-sudo
	
1. Make sure you've got the correct version of bundler:

    ```shell
    $ gem install bundler --version "2.3.26"      # or whichever version is used on GitHub Pages
    ```

1. Install node.js (needed by execjs, used by Katex) as per https://learn.microsoft.com/en-us/windows/dev-environment/javascript/nodejs-on-wsl

1. Checkout and cd into the project

1. Do bundle install

    ```shell
    $ bundle install
    ```

