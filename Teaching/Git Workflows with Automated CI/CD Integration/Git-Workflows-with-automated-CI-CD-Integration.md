# Git Workflows with Automated CI/CD Integration

## Story

In software development, it's essential to maintain a structured workflow to manage changes efficiently and ensure code quality. Git workflows like GitFlow,GitHub Flow,Forking Workflow and Centralised workflow provide guidelines for managing branching strategies and integrating changes smoothly.

CI/CD practices aim to automate and streamline the software development lifecycle, from code integration and testing to deployment and delivery.

* Continuous Integration (CI): Involves automatically integrating code changes into a shared repository multiple times a day. CI pipelines typically include automated tests to ensure code quality and detect issues early in the development process.

* Continuous Delivery (CD): Focuses on automating the delivery of code changes to production-like environments, enabling teams to release software updates at any time. CD pipelines involve automated deployment and validation steps, ensuring that code changes are production-ready.

* Continuous Deployment (CD): Takes automation a step further by automatically deploying every code change that passes through the CI/CD pipeline directly to production environments. This approach enables rapid delivery of features and fixes while maintaining a high level of confidence in the stability and reliability of the software.

GitHub Actions is a continuous integration and continuous delivery (CI/CD) platform that allows you to automate your build, test, and deployment pipeline. You can create workflows that build and test every pull request to your repository, or deploy merged pull requests to production.
In GitHub Actions a workflow is a series of actions initiated once a triggering event occurs. For example, the triggering event can be some commit pushed to a GitHub repository, the creation of a pull request, or another workflow completed successfully. 
The workflow is divided into jobs, and each job performs a set of steps. Each step runs one or more commands and can also call self-contained units of commands called actions. Each step runs on computational resources called runners, and the default settings can specify it to be Windows or Linux.

## Materials

https://www.atlassian.com/git/tutorials/comparing-workflows
https://www.redhat.com/sysadmin/git-hooks
https://docs.github.com/en/actions/using-workflows/about-workflows
https://codefresh.io/learn/github-actions/github-actions-tutorial-and-examples/

## What you need to do

* Create a presentation explaining all of the concepts mentioned and how you implemented them, make sure the explanations are comprehensive.

* Choose a Git workflow model (e.g., GitFlow, GitHub Flow, Forking Workflow or your custom workflow).
* Set up a new project repository following the chosen workflow model.
  * Create a new project repository, it can be a Node.js project or you can create your own project on GitHub.
  * Define the repository structure
  * Establish branch naming conventions (e.g., main,develop,feature branches,hotfix branches, release branches)
  * Establish guidelines for branch naming conventions and versioning schemes.
* Implement a feature by creating a new feature branch, making changes, and merging the branch back into the main branch.
  * Create feature branches for new developments and bug fixes.
  * Demonstrate the process of making changes, staging commits, and merging branches.
  * Highlight best practices for resolving merge conflicts and ensuring branch consistency.
* Configure a continuous integration (CI) system (e.g., GitHub Actions, Jenkins, Travis CI) to automate testing and code quality checks.
  * Integrate CI tools such as GitHub Actions into the project workflow.
  * Define CI pipelines to automate testing, code analysis, and deployment processes.
  * You should write your own pipeline configuration
* Test your CI/CD pipeline
  * Implement a feature from start to deployment testing the pipeline with various errors during the process (Incorrect syntax, code styling using linters)
  * Push these changes to feature branches.
  * Ensure the pipeline handles various scenarios like feature releases and syntax errors appropriately.
  
* Document your workflow process, including branching strategies, pull request guidelines, and CI configuration.

* Bonus Task 1: Implement automatic deployment of the project to a staging environment after successful CI checks.
* Bonus Task 2: Experiment with Git hooks to enforce coding standards and prevent committing code that doesn't meet quality criteria.
  * Dive deeper into Git hooks by experimenting with post-receive hooks for server-side actions.
  * Explore advanced hook scripts to enforce stricter code quality criteria and prevent committing substandard code.

**Please remember to keep the presentation short and concise. Long presentation bores the audience and you will also get tired in presenting. It has also been observed that images, quotes, interactive programming sessions tend to keep the audience interested in the content. (Recommended: Keep he presentation with 20 slides). Interview should be also prepared for questions regarding the topics being presented by him/her.** 

## Tech Stack

Git, CI/CD tools (e.g., GitHub Actions, Jenkins).

## Learning from the task

Understand Git workflows and their applications in real-world projects.
Learn about integrating Git with CI/CD pipelines to automate testing and deployment processes.
Gain experience in setting up and managing complex development workflows.
