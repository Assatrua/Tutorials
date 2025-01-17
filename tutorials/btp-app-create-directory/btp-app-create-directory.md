---
author_name: Iwona Hahn
author_profile: https://github.com/iwonahahn
title: Create a Directory for Development
description: This tutorial shows you how to start building your application with CAP and VS Code.
auto_validation: true
time: 10
tags: [ tutorial>beginner, software-product-function>sap-cloud-application-programming-model, topic>node-js, products>sap-business-technology-platform]
primary_tag: software-product-function>sap-cloud-application-programming-model
---

## Prerequisites
 - [Set Up Local Development using VS Code](btp-app-set-up-local-development)

## Details
### You will learn
 - How to develop the app
 - How to download the complete tutorial
 - How to create a GitHub repository
 - How to clone your GitHub repository

---

[ACCORDION-BEGIN [Step 1: ](Develop the App)]

If a tutorial has prerequisites, they're listed at the beginning of the tutorial.

For the tutorial, you need a directory to develop the app and you need access to the template files. We recommend choosing one root directory (that is the tutorial root directory) for both the directory for your app (`cpapp`) and the tutorial directory (`tutorial`) with the template files. See the table below:

| Directory | Contents |
|-|-|
| tutorial root directory | the directory containing `cpapp` and `tutorial` |
| `tutorial` | the directory containing the clone of the tutorial repository |
| `tutorial/templates` | templates provided by the tutorial repository |
| `cpapp` | the directory that will contain your application |

[DONE]
[ACCORDION-END]
---
[ACCORDION-BEGIN [Step 2: ](Download the Tutorial)]

Downloading the tutorial gives you easy access to template files that are required for some tutorials.

1. Open a terminal.

2. Navigate to the previously decided tutorial root directory:

    ```Shell/Bash
    cd <tutorial root directory>
    ```

3. Clone the tutorial:

    ```Shell/Bash
    git clone https://github.com/SAP-samples/cloud-cap-risk-management tutorial
    ```


[DONE]
[ACCORDION-END]
---
[ACCORDION-BEGIN [Step 3: ](Create a GitHub Repository for Your Project)]

We recommend creating a public [GitHub](https://github.com) repository to save your tutorial application. This way, if you have issues with your tutorial application, you can refer to it.

For real application development, you need to consider the right place for your repository, of course.

Go to [GitHub](https://github.com/) and create a new GitHub repository.

<!--
    Currently, SAP Continuous Integration and Delivery supports only [GitHub](https://github.com/) repositories.
    To be able to connect SAP Continuous Integration and Delivery with your repository, create a new repository on [GitHub](https://github.com/).
-->


[DONE]
[ACCORDION-END]
---
[ACCORDION-BEGIN [Step 4: ](Clone Your GitHub Repository)]

1. Copy the repository's URL you have created before.

2. Open a terminal.

3. Navigate to the tutorial root directory:

    ```Shell/Bash
    cd <tutorial root directory>
    ```

4. Clone your new repository:

    ```Shell/Bash
    git clone <git-repository-url> cpapp
    ```

    > Replace `<git-repository-url>` with your GitHub repository's URL.



[DONE]
[ACCORDION-END]
---
[ACCORDION-BEGIN [Step 5: ]((Optional) Copy the Files to Start from an Example)]

   > ### To earn your badge for the whole mission, you'll need to mark all steps in a tutorial as done, including any optional ones that you may have skipped because they are not relevant for you.

If you don't want to start from scratch, but from a specific example of the tutorial, you can copy the required files in your project. Alternatively, you can fork the project and work on the fork.

> The name of the prerequisite branch is given on the top of each tutorial that requires code changes.

1. Look-up the branch in the tutorial.

2. Open a terminal.

3. Navigate to the tutorial root directory:

    ```Shell/Bash
    cd <tutorial root directory>
    ```

4. Check out the example's branch:

    ``` bash
    cd tutorial
    git checkout <branch>
    ```

    > Replace `<branch>` with the name of the branch of the example that you want to start with.

5. Copy all files from the example to a local directory `<project-dir>`, except the `.git` directory.

    ```Shell/Bash
    cp -r .gitignore $(ls -1A | grep -v .git) ../cpapp
    ```

6. Check out the `master` branch to get access to the template files again:

    ```Shell/Bash
    git checkout master
    ```

7. Switch to your app directory:

    ```Shell/Bash
    cd ../cpapp
    ```

[VALIDATE_1]

[ACCORDION-END]
---