---
api_key_in:
- header
auth_types:
- apiKey
- oauth2
- http-bearer
description: 'Hoplite''s authentication surfaces: API keys for programmatic/API access, OAuth for the MCP server, per-automation bearer webhook tokens, and end-user sign-in options for the web app.'
kind: authentication
layout: security
method: searched
name: Hoplite Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Hoplite secures its APIs with apiKey, oauth2, and http-bearer across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Hoplite
provider_slug: hoplite
scheme_count: 3
schemes:
- docs: https://hoplite.sh/docs/cli
  in: header
  name: apiKey
  type: apiKey
  usage: Created under Settings -> Account -> API keys; used by the CLI, scripts, and other API automation.
- docs: https://hoplite.sh/docs/mcp-server
  flow: authorizationCode
  name: mcpOAuth
  type: oauth2
  usage: MCP server authorization — on first connect the client opens a browser to sign in and authorize a workspace; token stored at ~/.config/hoplite/mcp-oauth.json.
- docs: https://hoplite.sh/docs/automations
  name: automationWebhookToken
  scheme: bearer
  token_prefix: hwa2_
  type: http
  usage: Per-automation bearer token sent in the Authorization header to POST /api/automations/webhooks; scoped to a single automation, revealed once, rotatable.
slug: hoplite-authentication
source_filename: hoplite-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: >-\n  https://hoplite.sh/docs — auth model captured from the Hoplite docs (CLI, MCP\n  server, automations, getting-started). No OpenAPI is published, so this profile\n  is documented rather than derived from securitySchemes.\ndescription: >-\n  Hoplite's authentication surfaces: API keys for programmatic/API access, OAuth\n  for the MCP server, per-automation bearer webhook tokens, and end-user sign-in\n  options for the web app.\nsummary:\n  types: [apiKey, oauth2, http-bearer]\n  api_key_in: [header]\n  oauth2_flows: [authorizationCode]\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  usage: >-\n    Created under Settings -> Account -> API keys; used by the CLI, scripts, and\n    other API automation.\n  docs: https://hoplite.sh/docs/cli\n- name: mcpOAuth\n  type: oauth2\n  flow: authorizationCode\n  usage: >-\n    MCP server authorization — on first connect the client opens a browser to\n    sign in and authorize\
  \ a workspace; token stored at\n    ~/.config/hoplite/mcp-oauth.json.\n  docs: https://hoplite.sh/docs/mcp-server\n- name: automationWebhookToken\n  type: http\n  scheme: bearer\n  token_prefix: hwa2_\n  usage: >-\n    Per-automation bearer token sent in the Authorization header to POST\n    /api/automations/webhooks; scoped to a single automation, revealed once,\n    rotatable.\n  docs: https://hoplite.sh/docs/automations\nend_user_sign_in:\n  providers: [email-password, github, google]\n  extras: [two-factor-authentication, passkeys]\n  docs: https://hoplite.sh/docs/getting-started\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hoplite/refs/heads/main/authentication/hoplite-authentication.yml
summary_line: apiKey/oauth2/http-bearer · 3 schemes
tags:
- Company
- Coding Agents
- Developer Tools
- AI Agents
- Cloud Development Environments
- DevOps
- MCP
- Pull Requests
- Software Automation
- GitHub
---
