# Contributing to Analysis Documents for WildFly

Welcome to the Analysis Documents for WildFly project! We welcome contributions from the community. This guide will walk you through the steps for getting started on our project.

- [Legal](#legal)
- [Issues](#issues)
  - [Good First Issues](#good-first-issues)
- [Forking the Project](#forking-the-project)
- [Setting up your Developer Environment](#setting-up-your-developer-environment)
- [Contributing Guidelines](#contributing-guidelines)

## Legal

All contributions to this repository are licensed under the [Apache License](https://www.apache.org/licenses/LICENSE-2.0), version 2.0 or later, or, if another license is specified as governing the file or directory being modified, such other license.

All contributions are subject to the [Developer Certificate of Origin (DCO)](https://developercertificate.org/).
The DCO text is also included verbatim in the [dco.txt](dco.txt) file in the root directory of the repository.

### Compliance with Laws and Regulations

All contributions must comply with applicable laws and regulations, including U.S. export control and sanctions restrictions.
For background, see the Linux Foundation’s guidance:
[Navigating Global Regulations and Open Source: US OFAC Sanctions](https://www.linuxfoundation.org/blog/navigating-global-regulations-and-open-source-us-ofac-sanctions).


## Forking the Project
To contribute, you will first need to fork the [wildfly-proposals](https://github.com/wildfly/wildfly-proposals) repository.

This can be done by looking in the top-right corner of the repository page and clicking "Fork".

The next step is to clone your newly forked repository onto your local workspace. This can be done by going to your newly forked repository, which should be at `https://github.com/USERNAME/wildfly-proposals`.

Then, there will be a green button that says "Code". Click on that and copy the URL.

Then, in your terminal, paste the following command:
```bash
git clone [URL]
```
Be sure to replace [URL] with the URL that you copied.

Now you have the repository on your computer!

## Issues
The Analysis Documents for WildFly project uses GitHub Issues to manage issues. All issues can be found [here](https://github.com/wildfly/wildfly-proposals/issues).

To create a new issue, comment on an existing issue, or assign an issue to yourself, you'll need to first [create a GitHub account](https://github.com/signup).

There are two basic categories of changes to this repository, with different procedures to follow for each.

### New Feature Analyses

Most changes to this repository come in the form of analysis documents for new WildFly features. Such documents are just one part of the set of work that is needed to contribute a new WildFly feature.
Please familiarize yourself with the [WildFly Feature Development Process](https://docs.wildfly.org/wildfly-proposals/FEATURE_PROCESS.html) guide and follow the steps there.

### Miscellaneous Changes

Of course there can be other changes to this repository besides new feature analyses, e.g. changes to how the GitHub Pages publishing of the analyses works, changes to documents like this one, 
or even corrections to existing analyses.

To create a new issue miscellaneous issue, go to the [issues page](https://github.com/wildfly/wildfly-proposals/issues), click the "New Issue"" button, and choose the "Blank issue" option".

Once you have selected an issue you'd like to work on, make sure it's not already assigned to someone else.
Before beginning work on an issue, it's good to start a thread in the [wildfly-developers channel in Zulip](https://wildfly.zulipchat.com/#narrow/channel/174184-wildfly-developers) to let others know what you'll be doing.


### Good First Issues
Want to contribute to the Analysis Documents for WildFly project but aren't quite sure where to start? Look for issues with the `good first issue` label. These are a triaged set of issues that are great for getting started on our project. These can be found [here](https://github.com/wildfly/wildfly-proposals/pulls?q=is%3Aopen+is%3Apr+label%3A%22good+first+issue%22).


## Setting up your Developer Environment
You will need:

* JDK (SE 21 or later)
* Git
* Maven
* An [IDE](https://en.wikipedia.org/wiki/Comparison_of_integrated_development_environments#Java)
  (e.g., [IntelliJ IDEA](https://www.jetbrains.com/idea/download/), [Eclipse](https://www.eclipse.org/downloads/), [VS Code](https://code.visualstudio.com/), etc.)
  or a good text editor.


First `cd` to the directory where you cloned the project (eg: `cd wildfly-proposals`)

Add a remote ref to upstream, for pulling future updates.
For example:

```
git remote add upstream https://github.com/wildfly/wildfly-proposals
```

It is recommended that you use a separate branch for every issue you work on. To keep things straightforward and memorable, you can name each branch using the GitHub issue number. This way, you can have multiple PRs open for different issues.
```bash
git checkout -b Issue_9999
```

## Contributing Guidelines

When submitting a PR, please keep the following guidelines in mind:

1. In general, it's good practice to squash all of your commits into a single commit. For larger changes, it's ok to have multiple meaningful commits. If you need help with squashing your commits, feel free to ask us how to do this on your pull request. We're more than happy to help!

  1. Please include the GitHub issue you worked on in the title of your pull request and in your commit message. For example, for issue [999](https://github.com/wildfly/wildfly-proposals/issues/999), the PR title and commit message should be `[Issue_999] Create a testcase which verifies behaviour of the foo`.

2. Please include the link to the GitHub issue you worked on in the description of the pull request. For example, if your PR adds a fix for [999](https://github.com/wildfly/wildfly-proposals/issues/999), the PR description should contain a link to https://github.com/wildfly/wildfly-proposals/issues/999.
