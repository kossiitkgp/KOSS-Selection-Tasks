# Understanding memory management and garbage collection 


## Background

The manual memory management that you did (or are doing)
in your PDS lab, using `malloc` and `free`,
are OK upto a certain level of application complexity.
Beyond that, unless you are a very meticulous programmer,
managing memory can easily become a nightmare.
To help you with that, different programming languages come packed with
different memory management systems.

Garbage collection is a technique (or a broad category of techniques)
that is used for memory management is some high level languages like
Java, Python, Go etc.
However, there is another approach to memory management called the Ownership model,
made famous in recent times by Rust.

## What you need to do

1. Talk about what garbage collection is in general, its pros and cons.

2. Talk briefly about different techniques of garbage collection (eg reference counting),
giving examples about which languages they are used in.

3. Talk briefly about the memory model in Rust, specifically the Ownership model.

4. (Optional) Show running code snippets where garbage collection produces significant differences
in performance (both improvement and degradation, in time and memory).

We know it is a lot to take in, in this much limited time.
These are research topics in systems.
However, we expect the best effort from your side in completing as much as possible.
We will judge you on the basis of your depth of conceptual understanding
and not by your coverage.

Prepare no more than 20 slides.
You can use your favorite presentation tool.
But FYI, there are great open source projects out there, eg,
Libreoffice Impress, Reveal.js, Beamer (LaTex) etc.

## Reading materials

1. https://en.m.wikipedia.org/wiki/Garbage_collection_(computer_science)
2. https://speice.io/2019/02/understanding-allocations-in-rust.html

#### For any questions, please reach out to [Mukul Mehta](mailto:mukul.csiitkgp@gmail.com)
