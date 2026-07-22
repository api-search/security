---
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Cluely Authentication
name_suffix: Authentication
oauth_flows:
- browser-interactive
overview: Cluely secures its APIs with oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the browser-interactive flow(s).
provider_name: Cluely
provider_slug: cluely
scheme_count: 2
schemes:
- commands:
  - cluely auth login
  - cluely auth logout
  - cluely auth status
  credential_storage: OS keyring (macOS Keychain, Windows Credential Manager, Linux Secret Service)
  description: '`cluely auth login` opens the browser to sign in to your Cluely account.'
  flow: browser-interactive
  name: CLIBrowserLogin
  sources:
  - cli/cluely-cli.yml
  type: oauth2
- description: End-user sign-in to the Cluely web/desktop app via Google authentication.
  flow: authorizationCode
  name: GoogleAuth
  sources:
  - changelog/cluely-changelog.yml
  type: oauth2
slug: cluely-authentication
source_filename: cluely-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://github.com/cluely/cluely-cli\nnotes: >-\n  Cluely publishes no public REST API and therefore no OpenAPI securitySchemes\n  to derive from. The documented authentication surface is the first-party CLI,\n  which authenticates via a browser-based OAuth sign-in and stores credentials\n  in the OS keyring. End users of the desktop/web app sign in with Google Auth.\nsummary:\n  types: [oauth2]\n  oauth2_flows: [browser-interactive]\nschemes:\n  - name: CLIBrowserLogin\n    type: oauth2\n    flow: browser-interactive\n    description: >-\n      `cluely auth login` opens the browser to sign in to your Cluely account.\n    credential_storage: OS keyring (macOS Keychain, Windows Credential Manager, Linux Secret Service)\n    commands: [cluely auth login, cluely auth logout, cluely auth status]\n    sources: [cli/cluely-cli.yml]\n  - name: GoogleAuth\n    type: oauth2\n    flow: authorizationCode\n    description: End-user sign-in\
  \ to the Cluely web/desktop app via Google authentication.\n    sources: [changelog/cluely-changelog.yml]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cluely/refs/heads/main/authentication/cluely-authentication.yml
summary_line: oauth2 · 2 schemes
tags:
- Company
- Ai
- Meeting Assistant
- Productivity
- Transcription
- Speech Recognition
- Sales
- Real-Time
- Command Line Interface
---
