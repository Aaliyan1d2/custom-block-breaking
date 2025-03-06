name: "Bug Report"
description: "Report an issue with the mod."
title: "[Bug] "
labels: ["bug"]
assignees: []

body:
  - type: markdown
    attributes:
      value: "## 🛠️ Thanks for reporting a bug! Please fill out the details below."

  - type: textarea
    id: bug_description
    attributes:
      label: "Describe the Bug"
      description: "A clear and concise description of what the bug is."
      placeholder: "Describe the issue here..."
    validations:
      required: true

  - type: textarea
    id: steps
    attributes:
      label: "Steps to Reproduce"
      description: "How can we reproduce this bug?"
      placeholder: |
        1. Load the mod in Minecraft
        2. Perform [specific action]
        3. Observe the bug
    validations:
      required: true

  - type: textarea
    id: expected_behavior
    attributes:
      label: "Expected Behavior"
      description: "What should have happened instead?"
      placeholder: "The expected outcome..."
    validations:
      required: true

  - type: textarea
    id: logs
    attributes:
      label: "Crash Report or Logs (if applicable)"
      description: "Paste any relevant logs or crash reports here."
      render: shell

  - type: input
    id: mod_version
    attributes:
      label: "Mod Version"
      placeholder: "e.g., 1.0.0"

  - type: dropdown
    id: minecraft_version
    attributes:
      label: "Minecraft Version"
      options:
        - "1.20.1"
        - "1.19.4"
        - "1.18.2"
        - "Other"

  - type: checkboxes
    id: other_mods
    attributes:
      label: "Other Mods Installed?"
      options:
        - label: "Yes"
        - label: "No"

  - type: textarea
    id: additional_context
    attributes:
      label: "Additional Context"
      description: "Anything else we should know?"
      placeholder: "Other details about the issue..."
