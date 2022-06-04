# Static and Dynamic Libraries in C

## Background

Functions are blocks of code that are reusable throughout a program. Using them saves time, removing the need to rewrite code multiple times. Libraries, like functions also save time in that they make functiones reusable in multiple programs.

Static libraries, while reusable in multiple programs, are locked into a program at compile time. Dynamic, or shared libraries on the other hand, exist as separate files outside of the executable file.

A static library in C is a collection of objects files exposed for use and build another programs, so instead of re-write sections of code we bring back information that is already existing, this is where it comes the concept of library. In C exist two kinds of libraries the first ones are the static that allow us to linked to the program and are not relevant during the runtime, and the other ones are called dynamic libraries those are preferable use when you run a lot of programs at the same time who are using the same library and you want to be more efficient

## Tasks

Create a presentation with the following content:
- Static and dynamic libraries in C and their differences and advantages
- Linking of static and dynamic libraries in C\
- Workging of `ld` in linux (it's usage, common command flags) and the folders it uses for linking

Make sure to include images and command snippets in the presentation. \
Try out a simple static and dynamic linking example for this and explain the process in your presentation.

## Relevant Links

[https://medium.com/@StueyGK/static-libraries-vs-dynamic-libraries-af78f0b5f1e4](https://medium.com/@StueyGK/static-libraries-vs-dynamic-libraries-af78f0b5f1e4) \
[https://www.linkedin.com/pulse/what-static-library-how-use-them-juan-david-tuta-botero/?trackingId=9ogvYX7jTMyzl%2FL%2FJfWW1Q%3D%3D](https://www.linkedin.com/pulse/what-static-library-how-use-them-juan-david-tuta-botero/?trackingId=9ogvYX7jTMyzl%2FL%2FJfWW1Q%3D%3D) \
[https://www.linkedin.com/pulse/differences-between-static-dynamic-libraries-juan-david-tuta-botero/](https://www.linkedin.com/pulse/differences-between-static-dynamic-libraries-juan-david-tuta-botero/) \
[https://cu7ious.medium.com/how-to-use-dynamic-libraries-in-c-46a0f9b98270](https://cu7ious.medium.com/how-to-use-dynamic-libraries-in-c-46a0f9b98270)
