# Eudyptula Challenge - Task 1

## Background
Linux allows users to extend the functionality of the kernel with modules, which are pieces of code that can be loaded/unloaded on demand. You can load a module, and use the functionality without having to reboot, or re-compile the kernel. To list all modules loaded currently, we can use the `lsmod` command. 

The Eudyptula Challenge is a series of challenges, meant to introduce new people to the workflow of Linux Kernel developement. We want you to try out the first challenge, explain to us your understanding of kernel modules, and show us the code you've written.

## Problem Statement
**Copied verbatim from the challenge**

Write a Linux kernel module, and stand-alone Makefile, that when loaded
prints to the kernel debug log level, "Hello World!"  Be sure to make
the module be able to be unloaded as well.

The Makefile should build the kernel module against the source for the
currently running kernel, or, use an environment variable to specify
what kernel tree to build it against.

Please show proof of this module being built, and running, in your
kernel.  What this proof is is up to you, I'm sure you can come up with
something.  Also be sure to send the kernel module you wrote, along with
the Makefile you created to build the module.

We know that this task involves learning about a lot of concepts, so we do not except you to become masters in just a couple of days. We want to see what you've explored, and the effort you've put into the presentation

Please create a presentation, either using PPT, or using a tool such as Reveal.JS. The interviewee needs to keep in mind that the crowd he will be presenting to, will have mixed people of different knowledge levels, so it is advised that to keep the content balanced for all. Keep it short, to less than 20 slides or so, and you could include images, screenshots from commands run, and short snippets of code, to keep the audience interested

## Relevant Material
- https://linux.die.net/lkmpg/x40.html
- https://wiki.archlinux.org/title/Kernel_module
- https://linux-kernel-labs.github.io/refs/heads/master/labs/kernel_modules.html
- https://sebastianfricke.me/eudyptula-challenge-Part-1/ (This contains code as well, but we expect you to be honest)
