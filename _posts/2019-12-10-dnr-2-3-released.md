---
layout: post
title: dotNetRDF 2.3.0 now available
tags: [dnr, releases]
---

We are pleased to announce a new dotNetRDF release today.

dotNetRDF 2.3 adds support for SHACL validation and a new Dynamic API for accessing RDF graphs using .NET dynamics (both thanks to contributor Samu Lang). 

With this release we have also removed support for the .NET Standard 1.0 API and .NET Core 1.0. Moving to .NET Standard 2.0 will enable us to support a lot more of the dotNetRDF API for .NET Core applications while at the same time reducing the amount of platform-specific code, making the project easier to develop and maintain going forwards.

As usual this release also fixes a number of bugs reported by the community.

For full details please refer to the [change log](https://github.com/dotnetrdf/dotnetrdf/blob/master/ChangeLog.txt)

dotNetRDF 2.3 can be found [here on NuGet](https://www.nuget.org/packages/dotNetRDF/2.3.0) and also on [GitHub](https://github.com/dotnetrdf/dotnetrdf/releases/tag/v2.3.0).
