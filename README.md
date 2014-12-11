AOSL
====

**Universal Format for Digital Story-Telling**

*AOSL Specification:* **2.0 (work in progress)**
*XAOSL Specification:* **(not started yet)**

**AOSL** is a data format to represent digital stories. 
It is designed as a pivot language, that is, tools can use the abstract digital story representation to generate different other specialized products: web pages, applications, packages, etc. to be read by
players.

**XAOSL** is a file format that is based on AOSL which embedd all resources into one archive file
and constrain the possible content so that it is usable as a universally readable package. 

See the [docs directory for specifications sources](./docs/).


AOSL and XAOSL are part of the [Art Of Sequence](http//artofsequence.org) project. 

 - Development info: http://dev.artofsequence.org/
 - Discussions: http://forum.artofsequence.org/
 - Report technical issues: https://github.com/artofsequence/aosl/issues
 - Tasks in progress and future plans: https://trello.com/b/3qeC6jcG/aosl-xaosl

## AOSL Specification


AOSL is specified using XML for inter-operability (to help building tools around it) and it can be used either for:

 - direct use: reading and edition of digital media stories directly by interpreting an AOSL file;
 - export: convert the AOSL information to a more efficient format for the target interpreter;
 - create a new file format: you can create new format files including AOSL representations to help describing a digital story;

AOSL is not explicitly designed to be read by humans (even if it is possible) because it's main target is helping tools process a digital story representation.
It is media-agnostic by default and interpreter-agnostic. It is extensible and can also be constrained for specific usage.

AOSL describe digital stories, which can exploit the procedural nature of the digital platforms.
It actually don't describe the story, but how to change the objects that compose the story to tell that story.
This imply that:

 - it can use any kind of resources (graphics, audio, video, games) inside the story (limited by what the interpreter can manage);
 - it can generate loops in the story;
 - it can generate branches (choice or other kinds of branching) in the story.

These are the specific features of digital platforms compared to other media supports.
AOSL aim to allow creative people to exploit (with moderation) and explore the possibilities
given by the digital platforms features.

Another goal of AOSL's design is to allow the author to specify in one place how the content of the story
should be modified depending on the capabilities of the interpreter.


