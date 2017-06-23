---
layout: post
title: dotNetRDF 2.0.0 prerelease
tags: [dnr, releases]
---

## TL;DR

A first pre-release of dotNetRDF 2.0 is now available for download from NuGet and from 
[GitHub](https://github.com/dotnetrdf/dotnetrdf/releases/tag/v2.0.0-pre7). 

This is the first in a cycle of pre-release versions which we will push out over the coming 
weeks to get [feedback and bug reports]().

For users of 1.0 the biggest changes are changes to the versions of .NET that we support and 
some reorganisation of the NuGet libraries. 

## Dropped Framework Support

We have decided to drop support for several older versions of the .NET Framework. This is 
to enable us to focus on the more modern frameworks and has allowed us to significantly 
clean up the code base by eliminating a lot of framework-specific code. It also reduces
our test matrix and makes it easier for us to ensure that dotNetRDF is properly tested
on the supported frameworks. The frameworks dropped are:


## NuGet Reorganisation


## Behind The Scenes

In addition to all this rearranging of stuff we have made a lot of changes to how the project
is hosted, built and deployed. The most significant of these is the addition of continuous integration
on Appveyor and the change to master-branch based development.

You may have noticed that this "first" pre-release has the pre-release tag 7. The first 6 pre-releases 
were sacrificial releases made to get the automatic deployment from Appveyor working properly - now that
this is in place we hope that we have a much more robust and streamlined deployment process which should
allow us to start pushing out new releases as the master branch is updated.

This change to the CI environment goes hand in hand with the change to our branching strategy to merge
features and PRs directly into master. This means that we can make much more responsive releases, especially
during the pre-release cycle. This isn't a change to a "rolling release" model however - we are still driving 
our releases off of manual tagging of the master branch; but what it should mean for those brave enough to build
from source is that our master branch always holds the latest "release-ready" code (for some value of "release-ready" ;-)

## New Stuff


## Going Forwards

