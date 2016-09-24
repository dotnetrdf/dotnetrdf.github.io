---
layout: post
title: Migrations and Transitions
tags: [dnr, dnr2]
excerpt: Change is the only constant - for this project as everything else!
---

First post on our new site infrastructure. How exciting!

This post marks the end of the beginning of our migration of the dotNetRDF project from its older homes of SourceForge and BitBucket over to GitHub. 
The source code is now all migrated, and the recent 1.0.12 release was built from the new source code infrastructure. The documentation is now
managed as a [GitHub wiki](http://github.com/dotnetrdf/dotnetrdf/wiki). Right now the documentation has a number of formatting issues that result from
the migration from the BitBucket wiki which used a different wiki syntax but we are working through the pages fixing this bit by bit - please bear with us
while this dull, but important work gets finished off!

The source code for VDS.Common (a library of useful data-structures for .NET and one of our core dependencies) is also now managed under the [dotNetRDF
organization at GitHub](http://github.com/dotnetrdf/). 

A sadder transition has also taken place as the creator and long-time sole maintainer of dotNetRDF, Rob Vesse has stepped down 
from that position. We have to thank Rob for all of his hard work and dedication that has brought the project to where it is today. To ensure that the project continues, 
I have taken up the maintainer role. To introduce myself, I'm [Kal](http://twitter.com/kal_ahmed) and among other things I am the lead developer and maintainer of 
[BrightstarDB](http://brightstardb.com/) an open-source RDF triple store for .NET. Unsurprisingly, dotNetRDF is a major dependency for that project; and I use
dotNetRDF in a lot of my work with [NetworkedPlanet](http://www.networkedplanet.com/) - so I have a strong personal incentive to keep this project going.

The .NET landscape is undergoing many transitions of its own, with .NET Core and the open-sourcing of the .NET libraries. We are 
working right now on porting the existing codebase over to .NET Core. The next release (1.0.13) will see the addition of a .NET Core library to our distribution
and the NuGet package. 

Finally, I have also migrated the work Rob had started on dotNetRDF 2.0. This is an ambitious, complete re-write of dotNetRDF so it is something of a longer
and more major transition but one which I hope we can move forwards on. If you are interested in what is planned with this new version of the library or are 
considering contributing please take a look at [the new design documentation](https://github.com/dotnetrdf/dotnetrdf/wiki/DeveloperGuide-Architecture-Design) that Rob wrote describing the 2.0 motivation and design notes.

