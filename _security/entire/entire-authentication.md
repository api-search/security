---
api_key_in: []
auth_types:
- oauth2-device
- bearer-token
description: ''
kind: authentication
layout: security
method: searched
name: Entire Authentication
name_suffix: Authentication
oauth_flows:
- deviceAuthorization
overview: Entire secures its APIs with oauth2-device and bearer-token across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the deviceAuthorization flow(s).
provider_name: Entire
provider_slug: entire
scheme_count: 2
schemes:
- command: entire login
  description: The Entire CLI authenticates with the platform via a device authorization flow (`entire login`), which mints a token used for subsequent Checkpoint/session sync.
  flow: deviceAuthorization
  name: EntireDeviceAuth
  sources:
  - https://github.com/entireio/cli
  type: oauth2
- description: Access token issued by device auth. Stored in the OS keyring by default, with file-backed and ENTIRE_TOKEN environment-variable fallbacks for CI/headless use.
  name: EntireToken
  scheme: bearer
  sources:
  - https://github.com/entireio/cli
  token_env: ENTIRE_TOKEN
  token_storage:
  - os-keyring
  - file-backed store
  - environment variable
  type: http
slug: entire-authentication
source_filename: entire-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://github.com/entireio/cli + https://docs.entire.io/ (Security and privacy)\nnote: >-\n  Entire exposes no public REST API, so this profile is derived from the platform's\n  documented CLI/client authentication rather than from an OpenAPI securityScheme.\nsummary:\n  types: [oauth2-device, bearer-token]\n  api_key_in: []\n  oauth2_flows: [deviceAuthorization]\nschemes:\n- name: EntireDeviceAuth\n  type: oauth2\n  flow: deviceAuthorization\n  command: entire login\n  description: >-\n    The Entire CLI authenticates with the platform via a device authorization flow\n    (`entire login`), which mints a token used for subsequent Checkpoint/session sync.\n  sources: [https://github.com/entireio/cli]\n- name: EntireToken\n  type: http\n  scheme: bearer\n  token_env: ENTIRE_TOKEN\n  token_storage: [os-keyring, file-backed store, environment variable]\n  description: >-\n    Access token issued by device auth. Stored in the OS\
  \ keyring by default, with\n    file-backed and ENTIRE_TOKEN environment-variable fallbacks for CI/headless use.\n  sources: [https://github.com/entireio/cli]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/entire/refs/heads/main/authentication/entire-authentication.yml
summary_line: oauth2-device/bearer-token · 2 schemes
tags:
- Company
- Developer Tools
- Developer Platform
- Git
- Git Hosting
- Version Control
- Source Control
- AI Agents
- Agent Infrastructure
- CLI
---
