---
title: "Certified Kubernetes Administrator Study Guide"
linkTitle: "CKA Study Guide"
weight: 20
menu:
  main:
    weight: 20
---

- [About the Learning Guide Template](#about-the-learning-guide-template)
- [Formatting Reference](#formatting-reference)
  - [Reference Guide](#reference-guide)
  - [Source Template Documentation](#source-template-documentation)
  - [Template Framework Documentation](#template-framework-documentation)
- [How to create a new Learning Guide](#how-to-create-a-new-learning-guide)
  - [Prerequisites](#prerequisites)
  - [Instructions](#instructions)

## About the Learning Guide Template

This template is a simple, single page template based on [Google's Open Source Docsy theme](https://docsy.dev) for the [Hugo Static Site generator](https://gohugo.io), that includes custom styling and feature enhancements for the ModernApps community. 

In addition to the static content present in the template, the template itself includes a number of key workflow automations based on github actions. This repository includes an automated workflow that allows members with contributor or greater privileges to automatically create a new lab guide template repository which they can use to create a custom lab guide. 

This workflow automates the setup of the new lab guide including: 
- Creates a new repository
- Scaffolds many of the lab guide settings files with the new guide title, url and other variables
- Creates the full set of standard ModernApps by Tanzu github labels on the new repository
- Implements the ModernApps by Tanzu Github Teams-based IAM and Policy Model on the new repository
- Adds the guide creator to the Maintainers team for the ModernApps Ninja github org and the new repository, empowering the content developer to customize the settings for their repository if desired

Once the new repository is created, it is pre-loaded with several other key workflow automations, the most important of which is the hugo build action, which automatically triggers a hugo build to generate updated html files each time you update a source markdown file on this repository. 

There is no specific formatting requirement for what constitutes a "Learning Guide", this repository is intended to be used for anyone who wants to create a one or more page site, where the content creator is free to utilize the full range of capabilities possible within the robust Docsy and Hugo frameworks.

The docsy template was chosen because of its in-page navigation features that empower content creators to create long single page documents utilizing in-page navigation, and also to support complex multi-page and multi-section navigational structures. Accordingly content developers can also start a guide with a simple single page, and can choose to grow the site over time to a more complex multi-page or multi-section structure, or grow a guide into a full ModernApps Course over time, as the ModernApps Course template is a multi-section implementation based on the same exact baseline docsy template. 

## Formatting Reference

### Reference Guide

As there is already extensive documentation available for the docsy template, we would like to rely on the docsy documentation except in cases where the ModernApps template has a unique customization that requires instructions not present in the source docsy template instructions. 

Perhaps the simplest method to get started creating a ModernApps by Tanzu learning guide is to see if another guide is already published that is similar in style to how you would like your guide to look, to use that guide as a reference or even copy content from that guide into this repository and customize the content to your desire. If you arent familiar with markdown, perhaps the easiest way to get started is this method of copying from and modifying an existing guide with your content. 

You can browse other ModernApps by Tanzu guides to use for reference here: [https://modernapps.ninja/guide/](https://modernapps.ninja/guide/)

If you desire to create content that is formatted very differently from the existing guides, that is perfectly fine, you are free to reference the docsy template documentation and utilize the full range of features available in the docsy template. 

### Source Template Documentation

This repository is based on Google's docsy theme, which has excellent reference documentation for everything on basic Markdown formatting reference to detailed instructions for taking advantage of a wide variety of content and features that can be enabled within the docsy template. 

The docsy documentation can be found at [https://docsy.dev](https://docsy.dev).

### Template Framework Documentation

The Docsy theme is implemented by the Hugo static site generator. Hugo offers an even greater array of customizations that guide developers can leverage to be able to offer an incredibly robust range of options that make it possible to leverage virtually any feature available in modern web frameworks within your learning guide. 

The Hugo documentation can be found at [https://gohugo.io](https://gohugo.io)

## How to create a new Learning Guide

### Prerequisites

To create a new learning guide, you must first have contributor or highter level priviliges in the ModernApps community. If you do not yet have contributor priviliges, you can open a support request ticket for assistance here: [https://github.com/ModernAppsNinja/modernappsninja.github.io/issues/new/choose](https://github.com/ModernAppsNinja/modernappsninja.github.io/issues/new/choose)

### Instructions

1. Navigate to the actions tab on the github repository for this page
2. Select the `Create New Learning Guide` Workflow
3. Select the `Run Workflow` pulldown to expose the form you need to fill in to run the workflow
4. Fill in the form fields including title, description etc, and then click `Run Workflow`

After you click run workflow, the workflow will build a new repository for your learning guide, and will post a message to the new repository to provide instructions and alert the github user account that initiated the Create New Learning guide workflow that the new repository is now available.

Once the new guide is provisioned, the content author can then customize the content in the template until it provides the information and user experience desired. Once the new guide is prepared, you can open a trouble ticket on the modernapps.github.io repo requesting that the guide be published on the ModernApps.ninja homepage. 

Thanks for participating in the ModernApps by VMware Tanzu Community!

