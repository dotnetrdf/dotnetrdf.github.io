---
layout: post
title: dotNetRDF 2.4.0 now available
tags: [dnr, releases]
---

We are pleased to announce a new dotNetRDF release today.

dotNetRDF 2.4 has been focussed on eliminating some of the API differences between the .NET Standard and .NET Framework targets of the library. This change means that dotNetRDF now requires a minimum of .NET Standard 2.0 for .NET Core applications, but this allows us to enable support for a whole host of features that were previously missing from the API for .NET core applications, including:
  * The option to use PLINQ evaluation for joins
  * Parallel and asynchronous query evaluation in Leviathan
  * SPARQLView invalidation
  * Multi-threaded writing in store writers
  
This release also fixes a small number of bugs reported by the community.

For full details please refer to the [change log](https://github.com/dotnetrdf/dotnetrdf/blob/master/ChangeLog.txt)

dotNetRDF 2.4 can be found [here on NuGet](https://www.nuget.org/packages/dotNetRDF/2.4.0) and also on [GitHub](https://github.com/dotnetrdf/dotnetrdf/releases/tag/v2.4.0).
