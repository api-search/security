---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Trilo Chat Authentication
name_suffix: Authentication
oauth_flows: []
overview: trilo-chat declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: trilo-chat
provider_slug: trilo-chat
scheme_count: 2
schemes:
- description: Browser-based OAuth login via `trilo login` which opens a browser to the Trilo authorization page and stores a token.
  docs: https://docs.trilo.chat/developers/cli/authentication
  flow: authorization_code
  type: oauth2
- description: Personal Access Token (PAT) set via environment variable or config file for CI/CD.
  docs: https://docs.trilo.chat/developers/cli/authentication
  in: header
  name: TRILO_TOKEN
  type: apiKey
slug: trilo-chat-authentication
source_filename: trilo-chat-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: searched\nsource: https://docs.trilo.chat/developers/cli/authentication\nschemes:\n  - type: oauth2\n    flow: authorization_code\n    description: Browser-based OAuth login via `trilo login` which opens a browser to the Trilo authorization page and stores a token.\n    docs: https://docs.trilo.chat/developers/cli/authentication\n  - type: apiKey\n    name: TRILO_TOKEN\n    in: header\n    description: Personal Access Token (PAT) set via environment variable or config file for CI/CD.\n    docs: https://docs.trilo.chat/developers/cli/authentication\n"
source_yaml_url: https://artifacts.apis.io/trilo-chat/authentication/trilo-chat-authentication.yml
summary_line: 2 schemes
tags:
- AI
- Collaboration
- Productivity
- Workspace
- Chatbot
---
