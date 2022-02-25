# Converting Word documents to Markdown using Pandoc.

## Table Of Contents
1. [Introduction](#introduction)
2. [Instructions](#instructions)
3. [Common Errors](#common-errors)

## Introduction
Markdown has slowly become the standard for creating websites due to being far easier than its competitions for basic level website posts. In this guide we will go over how to convert your word documents to markdown files automatically using Pandoc. The reason we use Pandoc is that it supports multiple flavors of markdown, the most reputable being the [Github Flavor Markdown spec](https://github.github.com/gfm/) which is what we will be using in this class.

## Instructions
1. The first step is to install [Pandoc](https://pandoc.org/installing.html) if you have not already.
    - Download the installer and follow the steps to setup.
3. Ensure that your document is in the .docx format.
    - If you have a word version from 2007 to present then your document is automatically save in the .docx format.
4. Open command prompt.
    - You can do so by clicking Windows icon>Searching up Command Prompt.
5. Enter into the folder that your word document is stored on Command Prompt.
    1. Open file explorer and navigate to where you saved your word document.
    2. In the bar at the top of you explorer click and copy the C:\path\to\file\
    3. Return to Command Prompt and use the command ```cd C:\path\to\file```
6. Once you have entered into the folder where your file is stored in Command Prompt, use the command \

    ```
    pandoc -t gfm --extract-media . -o [file].md [file].docx
    ```
    - The ```--extract-media``` option ensures that all images in your document are properly stored to be shown in your markdown file.

## Common Errors
If you run into any errors converting your files, check to make sure that you have followed all the guidelines included below.
- Ensure that you're word document is in the .docx format.
- Ensure that you're are in the appropriate folder where your file is stored.

[Back](sidpoth.github.io)
