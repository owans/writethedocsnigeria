# WriteTheDocsNigeria
This is an example tutorial to show how to build a static site with markdown and jekyll in Write the Docs Nigeria Meetup on 3rd April, 2021

This repo contains the Sample Tutorial for: [how to build a static site with markdown and jekyll]()

## Requirements

- ***Ruby*** version 2.6.3, including all development headers
  (ruby version can be checked by running `ruby -v`)
  - [RVM](https://rvm.io/) is recommended to install and
    switch between multiple Ruby versions.
- ***RubyGems*** (which you can check by running `gem -v`)
- ***GCC and Make*** (in case your system doesn’t have them installed,
  which you can check by running `gcc -v`,`g++ -v` and
  `make -v` in your system’s command line interface)

## Set up

Clone this repository, and run the following commands in its directory:

```shell
sudo gem install bundler
bundle update
bundle install
```

Verify your installation:

```shell
ruby -v
bundler -v
bundle exec jekyll -v
```

None of these three commands should error,
and they should all print out their version numbers.

## Usage

### Development mode

```bash
bundle exec jekyll serve
```

You will now find a site ready for production in `./_site`.

You will now find a site located in `./_site`,
and this will be served at [`http://localhost:4000/`](http://localhost:4000/).

Pass the `--livereload` option to serve to automatically refresh the page with each change you make to the source files: `bundle exec jekyll serve --livereload`

Each time you save a file, the site will get regenerated.