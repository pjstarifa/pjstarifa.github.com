---
layout: post
title: "Getting Started With Octopress"
date: 2013-05-29 11 
categories: blog
---

## Creating, Previewing, and Deploying 

### Create

    rake new_post["title"]

    rake new_page[super-awesome]
    # creates /source/super-awesome/index.markdown

    rake new_page[super-awesome/page.html]
    # creates /source/super-awesome/page.html

### Preview

    bundle exec rake generate   # Generates posts and pages into the public directory
    bundle exec rake watch      # Watches source/ and sass/ for changes and regenerates
    bundle exec rake preview    # Watches, and mounts a webserver at http://localhost:4000

### Deploy

    bundle exec rake generate
    bundle exec rake deploy

### Update Source Control

    git status
    git add -A
    git commit -m "message"    
    git push origin master