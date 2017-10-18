---
layout: post
title: dotNetRDF 2.0.0 Pre-release 8 now available
tags: [dnr, releases]
---

A new pre-release of dotNetRDF 2.0 is now available via [NuGet](https://www.nuget.org/packages/dotNetRDF/2.0.0-pre0008) and [GitHub](https://github.com/dotnetrdf/dotnetrdf/releases/tag/v2.0.0-pre8)

This update adds .NET Core 2.0 as a target, so these new NuGet packages can now be used in your .NET Core 2.0 applications.

The changelog for 2.0 so far is:

 * Tools and samples are now moved to their own independent GitHub repositories (https://github.com/dotnetrdf/dotNetRDF.Toolkit and https://github.com/dotnetrdf/dotNetRDF.Samples).
 * Support for .NET 3.5 and .NET 3.5 client profile has been removed.
 * Updated the solution and project files to .NET Core SDK 2.0
 * Added support for .NET Core 1.1 and 2.0
 * The build process has been simplified and no longer relies on NAnt - a build can be done from the command line as `dotnet restore` followed by `dotnet build`
 * Added support for JSON-LD. The implementation is tracking the in-development JSON-LD 1.1 specification.
 * Added support for enabling/disabling reasoning on SPARQL queries over the Stardog connector. Thanks to @charbull for the PR.
