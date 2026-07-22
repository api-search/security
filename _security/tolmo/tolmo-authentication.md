---
api_key_in:
- header
auth_types:
- oauth2
- http-bearer
description: ''
kind: authentication
layout: security
method: searched
name: Tolmo Authentication
name_suffix: Authentication
oauth_flows:
- browser-based interactive login
overview: Tolmo secures its APIs with oauth2 and http-bearer across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the browser-based interactive login flow(s).
provider_name: Tolmo
provider_slug: tolmo
scheme_count: 2
schemes:
- description: Browser-based OAuth flow started with `tolmo auth login`. Credentials are stored locally in ~/.tolmo/ as a named profile and reused for subsequent commands. Supports multiple named profiles (--profile / TOLMO_PROFILE) and per-command org override (--org).
  name: interactive-oauth
  sources:
  - https://docs.tolmo.com/authentication
  type: oauth2
- description: Non-interactive API token for CI/CD and automation. Set TOLMO_API_TOKEN (generated from org settings in the Tolmo dashboard) together with TOLMO_ORG_SLUG (the token does not encode an org identity). When set, Tolmo skips profile lookup entirely.
  name: api-token
  scheme: bearer
  sources:
  - https://docs.tolmo.com/configuration/environment-variables
  type: http
slug: tolmo-authentication
source_filename: tolmo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://docs.tolmo.com/authentication\ndocs: https://docs.tolmo.com/authentication\nnote: >-\n  No public OpenAPI is published, so this profile is captured from the CLI\n  authentication docs rather than derived from securitySchemes. Requests to the\n  Tolmo backend (default https://api.tolmo.com) are authenticated two ways.\nsummary:\n  types: [oauth2, http-bearer]\n  api_key_in: [header]\n  oauth2_flows: [browser-based interactive login]\nschemes:\n- name: interactive-oauth\n  type: oauth2\n  description: >-\n    Browser-based OAuth flow started with `tolmo auth login`. Credentials are\n    stored locally in ~/.tolmo/ as a named profile and reused for subsequent\n    commands. Supports multiple named profiles (--profile / TOLMO_PROFILE) and\n    per-command org override (--org).\n  sources: [https://docs.tolmo.com/authentication]\n- name: api-token\n  type: http\n  scheme: bearer\n  description: >-\n    Non-interactive API\
  \ token for CI/CD and automation. Set TOLMO_API_TOKEN\n    (generated from org settings in the Tolmo dashboard) together with\n    TOLMO_ORG_SLUG (the token does not encode an org identity). When set,\n    Tolmo skips profile lookup entirely.\n  sources: [https://docs.tolmo.com/configuration/environment-variables]\nenvironment_variables:\n- {name: TOLMO_API_TOKEN, description: API token; skips profile lookup when set}\n- {name: TOLMO_ORG_SLUG, description: Organization slug; required when TOLMO_API_TOKEN is set}\n- {name: TOLMO_API_URL, description: Backend API base URL; defaults to production}\n- {name: TOLMO_PROFILE, description: Default profile name when --profile is not passed}\ncredential_model: >-\n  Connected-service credentials (GitHub App tokens, AWS role credentials,\n  Datadog API keys) are resolved server-side and never reach the client machine;\n  the CLI only carries the Tolmo token/profile.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tolmo/refs/heads/main/authentication/tolmo-authentication.yml
summary_line: oauth2/http-bearer · 2 schemes
tags:
- Company
- Security
- Cybersecurity
- Cloud Security
- Vulnerability Management
- CLI
- DevSecOps
- AI Agents
- Infrastructure Graph
---
