---
layout: post
title:  "Getting going again"
date:   2021-03-07 17:39:46 +0000 
categories: jekyll bundle
---
Bundle is a Ruby package manager.

It installs Ruby packages (called Gems) in a library folder, which I have set in .bundle/config to ~/.gem, and while it makes the project slightly less self contained it saves time downloading by sharing packages between projects.

To update a package change the version in the Gemfile and run

    $ bundle update <package>

The Gemfile.lock file contains the current version and dependency versions and allows tracking of the dependency versions so they don't get updated unexpectedly.
