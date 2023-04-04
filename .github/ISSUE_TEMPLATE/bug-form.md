name: Bug report
description: Help us diagnose and fix bugs in Official AWS Provider
title: ''
labels:
  - bug
  - needs:triage
body:
  - type: markdown
    attributes:
      value: >-
        Thank you for helping to improve Official AWS Provider!
        Please be sure to search for open issues before raising a new one. We
        use issues for both bug reports and feature requests.
  - type: textarea
    attributes:
      label: What happened?
      description: >-
        Please let us know what behavior you expected and how Official AWS
        Provider diverged from that expectation.
      placeholder: >-
        The more context you provide the easier it is for us to triage and
        prioritize your issue. Screenshots and logs help us contextualize the
        issue.
    validations:
      required: true
  - type: textarea
    attributes:
      label: How can we reproduce it?
      description: >-
        Help us to reproduce your bug as succinctly and precisely as possible.
        Artifacts such as example manifests or a script that triggers the issue
        are highly appreciated!
      placeholder: >-
        This is the most valuable information you can provide us to help us
        resolve this bug. Feel free to include a link to publicly accessible
        code or a GitHub Gist. 
    validations:
      required: true
  - type: dropdown
    attributes:
      label: Crossplane Version
      description: Which version of Crossplane or UXP are you using?
      options:
        - 1.11.3
        - 1.11.2
        - 1.11.1
        - 1.10.x
        - 1.9.x
        - Older than 1.9.x
        - Other
    validations:
      required: true
  - type: dropdown
    attributes:
      label: Provider Version
      options:
        - 0.32.1
        - 0.32.0
        - 0.31.0
        - 0.30.0
        - Older than 0.30.0
    validations:
      required: true
  - type: dropdown
    attributes:
      label: Kubernetes Distribution
      options:
        - Kind
        - EKS
        - AKS
        - GKE
        - OpenShift
  - type: input
    attributes:
      label: Kubernetes Version
      description: Specify the Server Version from the `kubectl version --short` output.
