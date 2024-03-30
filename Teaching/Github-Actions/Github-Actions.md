# New Git Concepts

## Story

In software development, it's essential to maintain a structured workflow to manage changes efficiently and ensure code quality. Git workflows like GitFlow and GitHub Flow provide guidelines for managing branching strategies and integrating changes smoothly.

## Materials

https://www.atlassian.com/git/tutorials/comparing-workflows
https://www.redhat.com/sysadmin/git-hooks
https://docs.github.com/en/actions/using-workflows/about-workflows

## What you need to do

* Choose a Git workflow model (e.g., GitFlow, GitHub Flow, or your custom workflow).
* Set up a new project repository following the chosen workflow model.
  * Create a new project repository on a GitHub.
  * Define the repository structure, including main, feature, and release branches.
  * Establish guidelines for branch naming conventions and versioning schemes.
* Implement a feature by creating a new feature branch, making changes, and merging the branch back into the main branch.
  * Create feature branches for new developments and bug fixes.
  * Demonstrate the process of making changes, staging commits, and merging branches.
  * Highlight best practices for resolving merge conflicts and ensuring branch consistency.
* Configure a continuous integration (CI) system (e.g., GitHub Actions) to automate testing and code quality checks.
  * Integrate CI tools such as GitHub Actions into the project workflow.
  * Define CI pipelines to automate testing, code analysis, and deployment processes.
  * Customize CI configurations to suit project requirements and ensure seamless integration with Git branches.
  
* Document your workflow process, including branching strategies, pull request guidelines, and CI configuration.

* Bonus Task 1: Implement automatic deployment of the project to a staging environment after successful CI checks.
* Bonus Task 2: Experiment with Git hooks to enforce coding standards and prevent committing code that doesn't meet quality criteria.
  * Dive deeper into Git hooks by experimenting with post-receive hooks for server-side actions.
  * Explore advanced hook scripts to enforce stricter code quality criteria and prevent committing substandard code.

**Please remember to keep the presentation short and concise. Long presentation bores the audience and you will also get tired in presenting. It has also been observed that images, quotes, interactive programming sessions tend to keep the audience interested in the content. (Recommended: Keep he presentation with 20 slides). Interview should be also prepared for questions regarding the topics being presented by him/her.** 

## Tech Stack

Git, CI/CD tools (e.g., GitHub Actions).

## Learning from the task

Understand Git workflows and their applications in real-world projects.
Learn about integrating Git with CI/CD pipelines to automate testing and deployment processes.
Gain experience in setting up and managing complex development workflows.
