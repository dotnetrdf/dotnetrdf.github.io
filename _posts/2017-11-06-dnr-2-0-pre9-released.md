---
layout: post
title: dotNetRDF 2.0.0 Pre-release 9 now available
tags: [dnr, releases]
---

A new pre-release of dotNetRDF 2.0 is now available via [NuGet](https://www.nuget.org/packages/dotNetRDF/2.0.0-pre0009) and [GitHub](https://github.com/dotnetrdf/dotnetrdf/releases/tag/v2.0.0-pre9)

This update fixes a couple of errors found in the previous pre-release.

The changelog for 2.0 so far is:

 * Tools and samples are now moved to their own independent GitHub repositories (https://github.com/dotnetrdf/dotNetRDF.Toolkit and https://github.com/dotnetrdf/dotNetRDF.Samples).
 * Support for .NET 3.5 and .NET 3.5 client profile has been removed.
 * Updated the solution and project files to .NET Core SDK 2.0
 * Added support for .NET Core 1.1 and 2.0
 * The build process has been simplified and no longer relies on NAnt - a build can be done from the command line as `dotnet restore` followed by `dotnet build`
 * Added support for JSON-LD. The implementation is tracking the in-development JSON-LD 1.1 specification.
 * Added support for enabling/disabling reasoning on SPARQL queries over the Stardog connector. Thanks to @charbull for the PR.
 * The SparqlRemoteEndpoint class now always honours an explicitly set HttpMode value. By default, the mode is set to AUTO which continues to implement pre-2.0 behaviour, 
   using GET unless the query string exceeds the internal query string length limit of 2048 characters or contains non-ASCII characters. From 2.0, if the user explicitly
   sets HttpMode to GET or to POST, that method will be used regardless of query parameter length or content. Thanks to @reeset for the report. (#128)
 * Fixed an error in the configuration of the Newtonsoft JSON parser that caused the RdfJSONParser to fail when the JSON file contained literal values formatted as ISO 8601 date/time strings. (#130)
