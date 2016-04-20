# Bath & NE Somerset Development team standards
Defining our standards for buildings and publishing software using public GitHub repositories.

## What is it?

This repository describes and gives templates for the general standards of documenting and licensing code held within the BathnesDevelopment organisational GitHub account.

It will also describe in very general terms coding standards and any other relevant guidelines for creating and maintaining code.

Anyone (internal or external) coming across a particular repository should be able to quickly understand what it is, why it was created, what skills are required to deploy/maintain it, what the licensing terms are, and how to go about building and deploying the code.

## Documentation standards

All repositories should be documented to a uniform standard, primarily including a readme file taken from the [README template](README-template.md) in this repository.

Installation should be covered in the readme file but more in depth installation details can be included as part of a documentation folder or documentation indicated to be elsewhere.

User guides can also be included within this documentation folder.

## Open source licensing

The Council has an open data policy, and is working towards a code sharing policy, as encouraged by the Government Digital Service in their [Coding in the Open](https://gds.blog.gov.uk/2012/10/12/coding-in-the-open/) blogs.

The Council also does not have many licensed software development tools, other than free versions of integrated development environments (IDEs), such as Visual Studio (VS) Community edition.

VS Community edition is free for individuals and organisations of under 250 employees, but other users must only use it for 'applications released under Open Source Initiative (OSI) approved open source software licenses'.  For this we have chosen the MIT licence.

[Microsoft: Visual Studio Community license terms](https://www.visualstudio.com/support/legal/mt171547)

## Technology standards

There is a wide variety of technologies used in the Council so there are few obvious limitations when choosing technologies.  However, repositories should ideally avoid using technologies unlikely to be used elsewhere for development, or that have historically caused issues, or that are going to be difficult to maintain.

Deploying solutions that we'd rather avoid is likely to cause further issues in future maintenance.  

- To avoid: Access databases, Oracle databases, VB, VB.Net, Classic ASP pages, PHP, Linux deployment
- Ideal: ASP.Net (MVC), C#, Microsoft SQL Server, PostgreSQL/PostGIS, Powershell, HTML5, JavaScript, jQuery, Bootstrap, Windows deployment

In general the set of technologies per project should be kept as minimal as possible.  Limit the requirements on server infrastructure setup/resources and the number of distinct technologies used.

## Security standards

While publicly making a lot of code available, there are some security considerations:

- Avoid publishing infrastructure details.  It is sensible to not publish too much about infrastructure such as server names or ports.   That may mean redacting within config/settings files, or not publishing areas of code dealing with publishing profiles (and holding these elsewhere). 
- Be extra careful about passwords.  It can be useful to explicitly restrict certain files (e.g. web.config) using ignore files and then publish samples for these files under different names.  This can take longer to setup and be some exra effort but it can be an extra step in avoiding ever accidentally publishing sensitive information.  Any extra steps required can be documented in the build/deployment README instructions.

## Coding standards

There are no restrictive guidelines on coding styles, but for some general info:

- Keep it simple. Prefer simple over heavily-refined code, particularly for smaller projects.
- Name things appropriately (e.g. variables/classes).  Choose descriptive names, avoid non standard abbreviations.
- Comment and document.  Code should be commented throughout (e.g. method/class commenting).  Some code will be self explanatory, other code may require a full description.