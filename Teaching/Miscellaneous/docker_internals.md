# Docker Internals!

## Background
Docker allows users to ship applications that are isolated from host systems, and agnostic of the host platform. This makes it super easy to reproduce issues, and you'll never have to say _But it works on my machine_ again!
Docker uses a lot of features from the Linux kernel, such as cgroups and namespaces. These features allow containers to run isolated from the host, without the need for spawing a virtual machine.

We want you to give us a brief overview of how Docker enables this isolation, by leveraging features such as cgroups and namespaces, which are part of the kernel

## What you need to do
We want you to cover the following topics:
- What in the world is a container even
- What cgroups and namespaces are, and how you can build _containers_ using them
- The Docker ecosystem - Docker today consists of multiple tools each doing their part: containerd, runc and many other tools that are part of the larger cloud native ecosystem. We would like to get a high level understanding of what they do, and what part they play
- (Optional) Show us some examples, using scripts, or tools of isolation achieved on a machine running Linux. You could show us how cgroups look like, how you can list namespaces and so on

We know that this task involves learning about a lot of concepts, so we do not except you to become masters in just a couple of days. We want to see what you've explored, and the effort you've put into the presentation

Please create a presentation, either using PPT, or using a tool such as Reveal.JS. The interviewee needs to keep in mind that the crowd he will be presenting to, will have mixed people of different knowledge levels, so it is advised that to keep the content balanced for all. Keep it short, to less than 20 slides or so, and you could include images, screenshots from commands run, and short snippets of code, to keep the audience interested

## Relevant Material
- https://docs.docker.com/get-started/overview
- https://docker-saigon.github.io/post/Docker-Internals/
- https://platform.sh/blog/2020/the-container-is-a-lie/
- https://jvns.ca/blog/2016/10/10/what-even-is-a-container/
- https://indradhanush.github.io/blog/life-of-a-container/
- https://www.youtube.com/watch?v=GwXLNAcHk-k
