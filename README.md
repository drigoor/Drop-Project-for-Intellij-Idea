# Drop Project Plugin for Intellij Idea

![[Static Badge](https://img.shields.io/badge/version-v0.9.4-blue)](https://img.shields.io/badge/version-v0.9.6-blue)
[![JetBrains plugins](https://img.shields.io/jetbrains/plugin/d/21870-drop-project)](https://img.shields.io/jetbrains/plugin/d/21870-drop-project)

<!-- Plugin description -->
[Drop Project](https://dropproject.org) is an open-source automated assessment tool that checks student programming projects for correctness and
quality. Currently, it supports Java and Kotlin projects.

This plugin allows students to submit their projects directly from Intellij IDEA. They can also review the submission build results.
<!-- Plugin description end -->

## Features

    Add assignments
    Check assignments details
    Submit assignments
    Review assignments results

## Requirements

* IntelliJ IDEA installed
* Access to Drop Project Website

## How to get it

* Access the IDE settings in File > Settings, or access directly through the settings icon in the upper right corner
* Go to the Plugins section
* Go to the Marketplace section in plugins and search for Drop Project
* Select Install

## How to use

* This plugin is mainly concentrated in a toolwindow, which is probably in the right panel of your IDE
* Login with your credentials (Your name; Your Drop Project Token)
* First icon in the toolbar is to add an assignment
* Second icon is to submit your code
* Third icon is to refresh the assignment list
* The last icon is to log out
* If you submit an assignment, a forth icon will appear which is used to check the buid report of your last submission
* You can access some aditional plugin settings in the settings icon on the toolwindow top title

## How to create a new version

* Update CHANGELOG.md - move all unreleased changes to the current version
* Change the `pluginVersion` property on `gradle.properties`
* Update, if necessary, the `pluginUntilBuild` property
    * In this case, make sure to test the plugin in that Intellij version. Change the platformVersion property and execute `Run Plugin`.
* Execute `Run Verifications`
* In github, create a release - this will trigger a github action to publish the plugin
