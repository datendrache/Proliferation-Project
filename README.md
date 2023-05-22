# The Proliferation Project

# Status MOTD

TL;DR

For those people stopping by, as of 5/22/2023 and expected for the remaining month or more, everything in is the state of being set up for GitHub and NuGet, as well as being converted from .NET Framework to .NET Core.

SS

Roughly 22 repositories are being converted from the original source started back in 2003.  This breaks a lot of functionality that will need to be fixed one project at a time.  The conversions of the code to .NET Core break all the Framework only functionality, including the API and the Web Forms applications.  I'm expecting these to be rewritten from the ground up.  The final number of projects that will be added to the Proliferation Project is an unknown at this point as several of these may be refactored into multiple NuGet packages.

Refactoring expections:

- Previous packages expected a Windows VM to host, the conversion to .NET Core frees up for the use of containers, webjobs, VM, desktop, etc.
- Tools like IntelliSense, SonarLint, and ReSharper are being used to clean up the code as refactoring is done.  Adherance to modern coding practices are now being observed.
- Unit Testing is now entering the picture, especially in the core libaries.  
- I'm also expecting to use DotNetBenchmark to help optimize, noting that sealing various classes and using improved performance on Linq may go a long way to improve performance.

When can people get started using these libaries for our own code?

The Libraries build on each other, and as I go through each interface and update their standards, it causes all the downstream libraries to need to be updated with new method casing, etc.  When I'm satisfied with all the changes to the project, I'll update the version numbers to 2.0.0.  (Keep in mind that this is probably closer to 10.0.0, as the original Proliferation Project code was written in Microsoft Java, then converted to J#, then converted to C# .NET Framework, then to where it is now at .NET Core 7.  This will be the signal that the code is ready for outside project use.

# Description

This is the home of the Proliferation Project, a personal vision for a data network of continuous discovery, data manipulation and event driven technologies.  This ia a conceptual ecosystem of automation rather than a specific product, made up of many smaller projects.

2023 Components:

1) Filesystem/File Data forensics
2) Data In Motion collection, processing, storage, and forwarding
3) Prototype data-in-motion processing, metadata manipulation, and interpreted language
4) Web based visualization tools
5) No-limit scalability
6) Metadata manipulation tools
7) Database/Datastore adapters

Why use the term "Proliferation"?  Because many of the technologies that entered into the mainstream reached the point where they were satisfactory for driving business sales, but not satisfactory for achieving the ideal state for solving the domain(s) problems:

1) Require extreme amounts of hardware, extremely slow performing
2) Limited to a specific types of data
3) Not well thought out, have artificial limitations, or limited by institutional use
4) Lack of modularity
5) No class, style, and/or makes everything too difficult
6) Lacks depth or breadth

Also, on a personal note, I have my own wonderment to pursue (i.e., nasty hacker mindset) and personal growth is very important to me (i.e., achieving entirely new technologies that matter to me and my personal life.)  The Proliferation Project is meant to grow my mastery of knowledge ecosystems, helping me improve the signal to noise ratio while extracting the meanings behind both.
