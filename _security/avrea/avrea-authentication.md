---
api_key_in:
- header
- environment
auth_types:
- apiKey
- browser-oauth
description: ''
kind: authentication
layout: security
method: searched
name: Avrea Authentication
name_suffix: Authentication
oauth_flows:
- browser-login
overview: Avrea secures its APIs with apiKey and browser-oauth across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the browser-login flow(s).
provider_name: Avrea
provider_slug: avrea
scheme_count: 2
schemes:
- description: API key used for non-interactive / CI authentication with the avr CLI. Presented via the AVR_TOKEN environment variable; `avr auth logout` revokes the active API key.
  in: environment
  name: AVR_TOKEN
  parameter: AVR_TOKEN
  sources:
  - https://docs.avrea.com/cli
  type: apiKey
- description: Interactive browser-based login (`avr auth login`) that authenticates the CLI against the Avrea console session at console.avrea.com.
  flow: browser
  name: browser-login
  sources:
  - https://docs.avrea.com/cli
  type: oauth2-like
slug: avrea-authentication
source_filename: avrea-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://docs.avrea.com/cli ; https://avrea.com/trust-security\ndocs: https://docs.avrea.com/cli\nnote: >-\n  Avrea publishes no public REST API OpenAPI, so this profile is derived from\n  the documented CLI and console authentication rather than from securitySchemes.\nsummary:\n  types: [apiKey, browser-oauth]\n  api_key_in: [header, environment]\n  oauth2_flows: [browser-login]\nschemes:\n- name: AVR_TOKEN\n  type: apiKey\n  in: environment\n  parameter: AVR_TOKEN\n  description: >-\n    API key used for non-interactive / CI authentication with the avr CLI.\n    Presented via the AVR_TOKEN environment variable; `avr auth logout` revokes\n    the active API key.\n  sources: [https://docs.avrea.com/cli]\n- name: browser-login\n  type: oauth2-like\n  flow: browser\n  description: >-\n    Interactive browser-based login (`avr auth login`) that authenticates the\n    CLI against the Avrea console session at console.avrea.com.\n\
  \  sources: [https://docs.avrea.com/cli]\naccount_security:\n- Multi-factor authentication (MFA)\n- Single sign-on (SSO)\n- Role-based access control for runners, logs, and build data\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/avrea/refs/heads/main/authentication/avrea-authentication.yml
summary_line: apiKey/browser-oauth · 2 schemes
tags:
- Company
- CI/CD
- Continuous Integration
- GitHub Actions
- Build Infrastructure
- Runners
- Caching
- Observability
- DevOps
- Developer Tools
---
