---
title: "How many tools do I need?"
date: 2019-1-4
authors:
  - author:
      name: "Guy Korland"
      link: "https://github.com/gkorland"
tags: ["CI", "buid"]
---

I have this fetish of finding new tools static-analysis/verification-tools/automation/code-coverage tools, I really can't stand the thought of bugs that we could have found by automatic tools before we merge a pull request.

Let me list some of the tools we're using at Redis Labs across our projects, I promise to cover some of them better in the future.

Obviously we start every project with a *CI* (continuous integration) platform, not all our projects are using the same CI tool, it’s a matter of taste and some legacy projects:
* [Circle CI](https://circleci.com/) - most of our projects are using CircleCI
* [Jenkins](https://www.jenkins.io/) - Redis Enterprise with its many flavours and vast automation is heavily invested in Jenkins.
* [Travis](https://travis-ci.org/) - Slowly fading out as we felt it doesn’t keep up with CircleCI.
* [Github Actions](https://github.com/features/actions) - the new kid on the block, it has its own advantages but it’s still not mature as the other tools.

On top of that the first thing we usually add is a *Code coverage* tool:
* [codecov](https://codecov.io/) 
* [coveralls](https://coveralls.io/) - we tried it but decided to stay with codecov

Next, comes the static *Code analysis* tools:
* [lgtm](https://lgtm.com/) - Still missing some of the 
* [Go Report Card](https://goreportcard.com/)
* [PMD](https://pmd.github.io/)
* [FindBugs](http://findbugs.sourceforge.net/)
* [SonarLint](https://www.sonarlint.org/)

And then a *Security* tool:
* [snyk](https://snyk.io)
* [Whitesource](https://www.whitesourcesoftware.com/)

Last, we want to make sure everything we develop is distributed and can be easily used by developers.

Docs:
* [GoDoc](https://godoc.org)
* [JavaDoc](https://www.javadoc.io)

Package manager:
* [Docker hub](https://hub.docker.com/)
* [pypi](https://pypi.org)
* [NPM](https://npmjs.org)
* [Maven Repository](https://mvnrepository.com/)
* [RubyGems](https://rubygems.org)

 


