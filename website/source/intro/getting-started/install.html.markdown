---
layout: "intro"
page_title: "Installing Serf"
sidebar_current: "gettingstarted-install"
---

# Install Serf

Serf must first be installed on every node that will be a member of a
Serf cluster. To make installation easy, Serf is distributed as a
[binary package](/downloads.html) for all supported platforms and
architectures. This page will not cover how to compile Serf from
source.

## Installing Serf

To install Serf, find the [appropriate package](/downloads.html) for
your system and download it. Serf is packaged as a "zip" archive.

After downloading Serf, unzip the package. Copy the `serf` binary to
somewhere on the PATH so that it can be executed. On Unix systems,
`~/bin` and `/usr/local/bin` are common installation directories,
depending on if you want to restrict the install to a single user or
expose it to the entire system. On Windows systems, you can put it wherever
you would like.

## Verifying the Installation

After installing Serf, verify the installation worked by opening a new
terminal session and checking that `serf` is available. By executing
`serf` you should see help output similar to that below:

```
$ serf
usage: serf [--version] [--help] <command> [<args>]

Available commands are:
    agent      Runs a Serf agent
    event      Send a custom event through the Serf cluster
    join       Tell Serf agent to join cluster
    members    Lists the members of a Serf cluster
    monitor    Stream logs from a Serf agent
    version    Prints the Serf version
```

If you get an error that `serf` could not be found, then your PATH
environmental variable was not setup properly. Please go back and ensure
that your PATH variable contains the directory where Serf was installed.

Otherwise, Serf is installed and ready to go!
