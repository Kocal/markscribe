# markscribe

[![Build Status](https://travis-ci.org/muesli/markscribe.svg?branch=master)](https://travis-ci.org/muesli/markscribe)
[![GoDoc](https://godoc.org/github.com/golang/gddo?status.svg)](https://godoc.org/github.com/muesli/markscribe)
[![Coverage Status](https://coveralls.io/repos/github/muesli/markscribe/badge.svg?branch=master)](https://coveralls.io/github/muesli/markscribe?branch=master)
[![Go ReportCard](http://goreportcard.com/badge/muesli/markscribe)](http://goreportcard.com/report/muesli/markscribe)

Your personal markdown scribe with template-engine and Git(Hub) & RSS powers 📜

In order to access GitHub's API, markscribe expects you to provide a valid
GitHub token as an environment variable called `GITHUB_TOKEN`.

## Usage

Render a template to stdout:

    markscribe file.tpl

Render to a file:

    markscribe -write /tmp/output.md file.tpl

## Templates

You can find an example template to generate a GitHub profile README under
`templates/github-profile.tpl`. Make sure to fill in the placeholders, like
the RSS-feed or social media URLs.

Rendered it looks a little like my own profile page: https://github.com/muesli

## Template Engine

markscribe uses Go's powerful template engine. You can find its documentation
here: https://golang.org/pkg/text/template/

## FAQ

Q: "That's awesome, but can you expose more APIs and data?"  
A: Of course, just let me know what you'd like to do with markscribe and open a new issue!
