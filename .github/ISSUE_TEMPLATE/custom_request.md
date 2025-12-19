---
name: Feature Request
description: Suggest a new feature
title: "Feature: "
labels: ["enhancement"]
body:
  - type: input
    id: title
    attributes:
      label: Add a title
      description: What is your name?
      placeholder: ex. Sertha Taveewattana
    validations:
      required: true
  - type: markdown
    attributes:
      value: |
        Thanks for taking the time to fill out this bug report!
  - type: dropdown
    id: request-type
    attributes:
      label: Type of request?
      description: Select the type of your request
      options:
        - New Feature
        - Enhancement
        - Documentation
      default: 0
    validations:
      required: true
  - type: dropdown
    id: os
    attributes:
      label: What is the OS which you want to suggest?
      options:
        - Selection
        - Windows
        - macOS
        - Linux
      default: 0
    validations:
      required: true
  - type: textarea
    id: details
    attributes:
      label: What are the details of your suggestion?
      description: Explain what do you want
      placeholder: Feature details!
    validations:
      required: true