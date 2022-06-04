# Inter Process Communication and DBus

## Background

An independent process is not affected by the execution of other processes while a co-operating process can be affected by other executing processes. Though one can think that those processes, which are running independently, will execute very efficiently, in reality, there are many situations when co-operative nature can be utilized for increasing computational speed, convenience, and modularity. Inter-process communication (IPC) is a mechanism that allows processes to communicate with each other and synchronize their actions.

D-Bus is a message bus system, a simple way for applications to talk to one another. In addition to interprocess communication, D-Bus helps coordinate process lifecycle; it makes it simple and reliable to code a "single instance" application or daemon, and to launch applications and daemons on demand when their services are needed. D-Bus has a structured view of the data it carries, and deals with data in binary form: integral numbers of various widths, floating-point numbers, strings, compound types, and so on. Because data is not just "raw bytes" to D-Bus, messages can be validated and ill-formed messages rejected.

## Task

Create a short presentation and teach the audience about the following:
- Interprocess communication(IPC) on Unix-like systems  ( or Linux specifically ) and various methods of IPC available in Unix-like systems ( or Linux specifically )
- DBus overview and how it works. Don't explain the API, just the basic concepts and the bus architecture.
- Features provided by DBus

## Relevant Materials

[https://en.wikipedia.org/wiki/Inter-process_communication](https://en.wikipedia.org/wiki/Inter-process_communication) \
[https://en.wikipedia.org/wiki/D-Bus](https://en.wikipedia.org/wiki/D-Bus) \
[https://www.freedesktop.org/wiki/IntroductionToDBus/](https://www.freedesktop.org/wiki/IntroductionToDBus/) \
[https://dbus.freedesktop.org/doc/dbus-tutorial.html](https://dbus.freedesktop.org/doc/dbus-tutorial.html) \
[https://dbus.freedesktop.org/doc/diagram.png](https://dbus.freedesktop.org/doc/diagram.png)