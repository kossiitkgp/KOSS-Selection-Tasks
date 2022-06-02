# NixOS

## Background

NixOS is both a Linux distro and a package manager, but unlike other disros (Ubuntu, Fedora, Arch Linux, etc.) it is a _declarative_ OS/package manager. It means, the packages and dependencies are always mentioned before-hand (in a configuration file), which avoids [dependency hell](https://en.wikipedia.org/wiki/Dependency_hell). It has it's own language (albeit a very simple one), Nix, which is used in its configuration files.

You don't have to install NixOS on your system (although you can if you want to). You can [directly install](https://nixos.org/download.html) the Nix package manager onto an existing Linux distro and it will work.

We want you to learn how Nix works and then present it. You should explain the Nix language and features of NixOS.

## What you need to do

At the minimum, you should cover the following topics:
- What exactly is NixOS and how it is different from other distros or package managers
- What is the Nix langauge (it's a functional language, so you can add 1-2 slides on that too)
- How to create your own package in Nix

You can even go into the following topics if you have the time:
- How it works under the hood
- Nix flakes

Please create a presentation, either using PPT or preferably a tool such as [RevealJS](https://revealjs.com/). The interviewee needs to keep in mind that the crowd he will be presenting to, will have mixed people of different knowledge levels, so it is advised that to keep the content balanced for all. Keep it short, to less than 20 slides or so, and you could include images, screenshots from commands run, and short snippets of code, to keep the audience interested.

## Relevant Material

1. https://nixos.org/
2. https://nixos.org/guides/nix-pills/
3. https://nixos.org/manual/nix/stable/
4. https://notes.yukiisbo.red/posts/2021/07/Spice_up_with_Nix_Scripts.html, https://notes.yukiisbo.red/posts/2021/08/Spice_up_with_Nix_Shells.html, https://notes.yukiisbo.red/posts/2021/09/Spice_up_with_Nix_Traditional_Software_Deployment.html, https://notes.yukiisbo.red/posts/2022/01/Spice_up_with_Nix_Functional_Software_Deployment.html
5. https://nixos.org/manual/nixpkgs/stable/ and https://nixos.org/manual/nixos/stable/

#### In case you have any questions, feel free to reach out to [Soham Sen](mailto:hello@sohamsen.me)
