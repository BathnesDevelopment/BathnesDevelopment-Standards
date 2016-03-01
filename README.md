# Bath and North East Somerset Council development team standards
Defining our standards for buildings and publishing software using public GitHub repositories.

## What is it?

This repository describes and gives templates for the general standards of documenting and licensing repositories held within the BathnesDevelopment organisational GitHub account.

It will also describe in very general terms coding standards and any other relevant guidelines for creating and maintaining code.

Anyone coming across a particular repository (internal or external) should understand what it is, why it was created, what skills are required to reproduce/maintain it, and how to go about building and deploying the code.

## Readme standards

All repositories should be documented to a uniform standard.

In development...

## Licensing standards

The Council has an open data policy, and is working towards a policy, encouraged in government towards a 'code sharing' policy.

In development...

## Technology standards

There is a wide variety of technologies used in the Council so there are few obvious limitations when choosing technologies.  However, repositories should ideally avoid using technologies that are unlikely to be used elsewhere in the Council for development, or that have historically caused issues.

These would be likely to cause further issues in being maintained in future.  

Ideal options: ASP.Net, C#, Microsoft SQL Server, PostgreSQL/PostGIS, 
To avoid: Access databases, Oracle databases, VB, Classic ASP pages, PHP

In general the set of technologies per project should be kept as simple as possible.  Limit the requirements on server infrastructure setup and the number of distinct tecnnologies used.

## Coding standards

There are no restrictive guidelines on coding styles, but for some general guidelines:

- Keep it simple. Prefer simple over heavily refined code, particularly for smaller projects.
- Name things appropriately (e.g. variables/classes).  Choose descriptive names, avoid non standard abbreviations.
- Comment and document.  Code should be commented throughout.  Some code will be self explanatory, other code may just require a full description (e.g. above a method/class/page)