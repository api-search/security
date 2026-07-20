---
api_key_in:
- environment
auth_types:
- apiKey
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Launchable Authentication
name_suffix: Authentication
oauth_flows: []
overview: Launchable secures its APIs with apiKey and openIdConnect across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Launchable
provider_slug: launchable
scheme_count: 2
schemes:
- description: Workspace API key issued from the Launchable web app and supplied to the CLI as an environment variable. The CLI presents it to the service on every request.
  docs: https://help.launchableinc.com/resources/cli-reference/
  example_usage: export LAUNCHABLE_TOKEN=your_API_key
  in: environment
  name: LAUNCHABLE_TOKEN
  parameter_name: LAUNCHABLE_TOKEN
  scope: workspace
  type: apiKey
- description: Keyless authentication for GitHub Actions workflows using GitHub's OIDC identity token in place of a long-lived LAUNCHABLE_TOKEN.
  docs: https://help.launchableinc.com/sending-data-to-launchable/using-the-launchable-cli/getting-started/migration-to-github-oidc-auth/
  name: GitHub OIDC
  status: recommended
  type: openIdConnect
slug: launchable-authentication
source_filename: launchable-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://help.launchableinc.com/resources/cli-reference/\ndocs: https://help.launchableinc.com/sending-data-to-launchable/using-the-launchable-cli/getting-started/\nnote: Launchable publishes no OpenAPI, so this profile is searched from the CLI/getting-started\n  documentation rather than derived from securitySchemes.\nsummary:\n  types:\n  - apiKey\n  - openIdConnect\n  api_key_in:\n  - environment\n  oauth2_flows: []\nschemes:\n- name: LAUNCHABLE_TOKEN\n  type: apiKey\n  in: environment\n  parameter_name: LAUNCHABLE_TOKEN\n  description: Workspace API key issued from the Launchable web app and supplied to the CLI as an\n    environment variable. The CLI presents it to the service on every request.\n  example_usage: export LAUNCHABLE_TOKEN=your_API_key\n  scope: workspace\n  docs: https://help.launchableinc.com/resources/cli-reference/\n- name: GitHub OIDC\n  type: openIdConnect\n  description: Keyless authentication for GitHub\
  \ Actions workflows using GitHub's OIDC identity\n    token in place of a long-lived LAUNCHABLE_TOKEN.\n  docs: https://help.launchableinc.com/sending-data-to-launchable/using-the-launchable-cli/getting-started/migration-to-github-oidc-auth/\n  status: recommended\nverification:\n  command: launchable verify\n  description: Confirms CLI authentication and connectivity to the Launchable service.\nscopes:\n  documented: false\n  note: No OAuth scope surface is published; authorization is workspace-bound by the API key or\n    OIDC subject. scopes/ is intentionally not produced.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/launchable/refs/heads/main/authentication/launchable-authentication.yml
summary_line: apiKey/openIdConnect · 2 schemes
tags:
- Company
- Continuous Integration
- Testing
- Test Automation
- Developer Tools
- DevOps
- Machine Learning
- Software Delivery
- Predictive Test Selection
- CI/CD
---
