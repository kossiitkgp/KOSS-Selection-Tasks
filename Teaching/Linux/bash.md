# Generating Report from CSV file using Shell Scripting

## Background

Bash shell scripting is a powerful tool used by system administrators, developers, and data analysts to automate tasks, process data, and manage systems. Bash is a command-line shell that runs on Unix-based operating systems such as Linux and macOS. Shell scripts are essentially a series of commands written in a file that can be executed by the Bash shell.

Bash shell scripting is used in a wide range of applications, from automating system maintenance tasks to processing data and generating reports. It can be used to manage and monitor servers, automate software builds and deployments, and process and analyze large amounts of data.

Learning Bash shell scripting is a valuable skill for anyone working with Unix-based systems, as it can help improve productivity, automate repetitive tasks, and make systems more efficient. It is also a valuable skill for data analysts, as Bash can be used to process and analyze data from a variety of sources.

In this task, you will be required to demonstrate your knowledge of Bash shell scripting by showing how to create a script that processes a CSV file and generates a report. This task will help assess your ability to understand and apply key concepts related to file input, data parsing, and report generation using Bash shell scripting.

## Tasks
Research and gather information on the key concepts and commands needed to create a bash shell script that will process a CSV file and generate a report. This should include topics such as handling file input, parsing CSV files, and generating reports.

Create a presentation with the following content:
- Key concepts and commands in a clear and concise manner.
- Code snippets and examples to illustrate how the same are used to create the script.
- Prepare a sample CSV file that contains data that needs to be processed and analyzed.
- During the presentation, guide the panel through the process of creating the report script step by step.

## Relevant Links

[Bash Basics](https://linuxconfig.org/bash-scripting-tutorial-for-beginners/) \
[Shell Scripting Tutorial](https://www.guru99.com/introduction-to-shell-scripting.html/) \
[Parsing CSV files in Bash](https://www.baeldung.com/linux/csv-parsing/)

## Demo

csv file
```
Name,Email,Phone Number
John Doe,john.doe@email.com,555-1234
Jane Smith,jane.smith@email.com,555-5678
Bob Johnson,bob.johnson@email.com,555-9012
```

output
```
Report Generated On: Thu Apr 7 10:30:45 PDT 2023

----------------------------------------------------------
                     User Report
----------------------------------------------------------
Name: John Doe
Email: john.doe@email.com
Phone Number: 555-1234

Name: Jane Smith
Email: jane.smith@email.com
Phone Number: 555-5678

Name: Bob Johnson
Email: bob.johnson@email.com
Phone Number: 555-9012

----------------------------------------------------------
               End of User Report
----------------------------------------------------------
```
