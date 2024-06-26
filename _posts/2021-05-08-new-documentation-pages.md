---
layout: post
title: New Documentation Pages
tags: [dnr, documentation, rtfm]
---

As we start to make more progress towards a 3.0 release I realized that there was a challenge looming for our documentation.
Up to now the docs have been managed as a GitHub wiki in the main dotNetRDF repository. This has the advantage of being 
really easy to locate and to update and has served us pretty well for the last few years. However there are a couple of problems
with using a wiki for the user docs.

The first problem is that  there is not really a neat way to have the documentation for the 3.0 API properly separated from
that for 2.x releases. As we are planning a number of breaking API changes for the next major release, this could
end up being a problem. Either we would end up with a lot of conditional sections ("If you are on 2.x do this, but 
on 3.x you need to do that") or else a whole additional parallel structure in the wiki.

The other problem that we have always had with the wiki is that the API documentation (generated by Sandcastle Help 
File Builder) has had to be hosted separately on the dotNetRDF.org website. 

Having looked around for a suitable replacement I finally settled on using DocFX to build an integrated set of user and API docs.
With this new system I am able to generate a complete documentation set (both user docs and API docs) for a given release and
then copy those over to the GitHub Pages repo that runs the dotNetRDF.org website. With a little bit of creative copying I can
also have persistent locations for the "latest stable" and "bleeding edge" docs as well as being able to keep older versions
of the documentation around for those who need it. With the API docs better integrated it is also now possible to reference
API documentation a lot more easily from the user docs - which will hopefully make life a lot easier for those working through
pages like our [tutorial](/docs/stable/user_guide/Getting-Started.html) to hop over to the API docs as needed.

You can [check out the brand new docs here](https://www.dotnetrdf.org/docs/stable/)

There's still a bit of work to do on making it a bit better integrated into the site overall (there is no easy way back from 
the docs to the homepage of the site right now, for example), but hopefully you will find the new docs at least as useful
(hopefully more useful!) than the old wiki.