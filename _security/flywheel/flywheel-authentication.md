---
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Flywheel Authentication
name_suffix: Authentication
oauth_flows: []
overview: Flywheel secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Flywheel
provider_slug: flywheel
scheme_count: 1
schemes:
- format: <hostname>:<key>
  in: header
  key_name: Authorization
  name: FlywheelApiKey
  obtained_from: User profile in the Flywheel web application
  sources:
  - docs.flywheel.io/Developer_Guides/api_sdk/
  type: apiKey
  used_by:
  - flywheel-sdk (Python) — flywheel.Client('<api-key>')
  - flywheel-cli — fw login <api-key>
  - fw-client HTTP client
slug: flywheel-authentication
source_filename: flywheel-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://docs.flywheel.io/Developer_Guides/api_sdk/\ndocs: https://docs.flywheel.io/Developer_Guides/api_sdk/\nnotes: >-\n  Flywheel authenticates API/SDK/CLI access with a per-user API key. The key is\n  of the form <hostname>:<key> and is generated from the user profile in the\n  Flywheel web UI. No public OpenAPI is available (the API is per-instance), so\n  this profile is captured from the developer documentation rather than derived.\nsummary:\n  types: [apiKey]\n  api_key_in: [header]\n  oauth2_flows: []\nschemes:\n  - name: FlywheelApiKey\n    type: apiKey\n    in: header\n    key_name: Authorization\n    format: '<hostname>:<key>'\n    obtained_from: User profile in the Flywheel web application\n    used_by:\n      - flywheel-sdk (Python) — flywheel.Client('<api-key>')\n      - flywheel-cli — fw login <api-key>\n      - fw-client HTTP client\n    sources: [docs.flywheel.io/Developer_Guides/api_sdk/]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/flywheel/refs/heads/main/authentication/flywheel-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Medical Imaging
- Healthcare
- Data Management
- Machine Learning
- Research
- DICOM
- Life Sciences
---
