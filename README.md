# Bath & NE Somerset Development team standards
Defining our standards for buildings and publishing software using public GitHub repositories.

## What is it?

This repository describes and gives templates for the general standards of documenting and licensing repositories held within the BathnesDevelopment organisational GitHub account.

It will also describe in very general terms coding standards and any other relevant guidelines for creating and maintaining code.

Anyone coming across a particular repository (internal or external) should be able to quickly understand what it is, why it was created, what skills are required to reproduce/maintain it, what the licensing terms are, and how to go about building and deploying the code.

## Documentation standards

All repositories should be documented to a uniform standard, primarily including a readme file taken from our template in this repository.

Installation should be covered in the readme file but more in depth installation details can be included as part of a documentation folder.  

User guides can also be included within this documentation folder.

In development...

## Licensing standards

The Council has an open data policy, and is working towards a code sharing policy, as encouraged by the Government Digital Service.

In development...

## Technology standards

There is a wide variety of technologies used in the Council so there are few obvious limitations when choosing technologies.  However, repositories should ideally avoid using technologies unlikely to be used elsewhere in the Council for development, or that have historically caused issues.

Deploying solutions that we'd rather avoid would likely cause further issues in future maintenance.  

- To avoid: Access databases, Oracle databases, VB, Classic ASP pages, PHP, Linux-only (unfortunately)
- Ideal options: ASP.Net, C#, Microsoft SQL Server, PostgreSQL/PostGIS, Powershell, HTML5, JavaScript, jQuery, Bootstrap

In general the set of technologies per project should be kept as minimal as possible.  Limit the requirements on server infrastructure setup/resources and the number of distinct technologies used.

## Security standards

While publicly making a lot of code available, there are some security considerations:

- Avoid publishing infrastructure details.  It is sensible to not publish too much about infrastructure such as server names or ports.   That may mean being more restricting within config/settings files, or not publishing areas of code dealing with publishing profiles (and holding these elsewhere). 
- Be extra careful about passwords.  It can be useful to explicitly restrict certain files (e.g. .config) using gitignore and then publish samples for these files.  This can take longer and be some exra effort but as long as the steps are explicitly listed in build/publish instructions then it can be an extra step in avoiding ever accidentally publishing sensitive information.

## Coding standards

There are no restrictive guidelines on coding styles, but for some general guidelines:

- Keep it simple. Prefer simple over heavily refined code, particularly for smaller projects.
- Name things appropriately (e.g. variables/classes).  Choose descriptive names, avoid non standard abbreviations.
- Comment and document.  Code should be commented throughout.  Some code will be self explanatory, other code may require a full description (e.g. above a method/class/page)