---
layout: essay
type: essay
title: "Meteor Gotchas"
date: 2017-03-09
labels:
  - Software Engineering
  - Meteor
---

# Growing Pains#

Using Meteor for the first time was an exciting experience because I never had the opportunity to develop web applications. However, this excitement didn't come without its difficulties. There was a lot of set up and involved and despite it being necessary, I wasn't the biggest fan of.

# Tell Me Whats Wrong#

One of the most significant issues that I ran into while developing in Meteor is that debugging is painful for me. Although IntelliJ highlights problem areas in a file, there isn't a really an error console that helpfully tells you whats wrong (at least not one that I have been made aware of).

When you write code in C or C++, the compiler will spit out error messages that help you debug your code and point out where the error is. When debugging in Meteor, I get blasted with a bunch of these error messages and not really too much of an idea where to start.

This isn't necessarily a problem with a "fix" so to speak. It is something that needs to be gotten used to. The way I solve it, is that I usually can revert to my last working build because of our use of version control with Git and GitHub. By committing code in working chunks, you can always revert backwards to a working state and attempt to implement whatever you were implementing again.

Without version control, I would have to attempt to remember the changes that I made that broke the build and try to remove them without removing something else that would further create problems. Overall, version control is necessary for working in any project. It saves a lot of headache and time.

# Bringing It All Together#

In this point in the semester we are starting to bring together all of the modules that we have been working on in hopes of working towards a final project. We are integrating JavaScript, Underscore library, Semantic UI, and now Meteor. I think its fair to say that we have covered a decent amount of material that no one has everything memorized if this is the first time they've seen it.

One common error I always end up making is that I try to implement code from memory typing something like:

```
<div class="ui text container" style="color: black"><p>Insert Text Here.</p></div>
```

When I want the container to turn black. However, the style we applied does not turn the background black, it turns the text inside the container black. This was a hard error for me to find because the text is defaulted to be black.

```
<div class="ui text container" style="background-color: black"><p>Insert Text Here.</p></div>
```

This would be the correct implementation and you can see that it was a small change in the code that really makes a large difference.

A solution is that there are many resources out there that have the proper documentation. More practice and experience will help catch these little bugs and make designing that much easier.
