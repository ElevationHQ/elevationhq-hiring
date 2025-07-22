# elevationhq-hiring
-----------

name: Walk-In Applicant
description: Log a new walk-in job applicant for Elevation HQ
title: "[Applicant] Full Name Here"
labels: ["applicant", "walk-in"]
assignees: []

body:
  - type: input
    id: full-name
    attributes:
      label: Full Name
      placeholder: e.g. John Doe
    validations:
      required: true

  - type: input
    id: phone
    attributes:
      label: Phone Number
      placeholder: e.g. (123) 456-7890
    validations:
      required: true

  - type: input
    id: email
    attributes:
      label: Email
      placeholder: e.g. john@example.com
    validations:
      required: true

  - type: dropdown
    id: availability
    attributes:
      label: Availability
      options:
        - Morning
        - Night
        - Any
    validations:
      required: true

  - type: dropdown
    id: role
    attributes:
      label: Interested Role
      multiple: true
      options:
        - Budtending
        - Inventory
        - Security
        - Floor
        - Cleaning
        - Management
    validations:
      required: true

  - type: dropdown
    id: resume
    attributes:
      label: Resume Provided?
      options:
        - Yes - attached to this issue
        - No - will email to elevationhq701@gmail.com
    validations:
      required: true

