---
api_key_in:
- url
auth_types:
- oauth2
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Tabtabtab Authentication
name_suffix: Authentication
oauth_flows:
- browser-login
overview: TabTabTab secures its APIs with oauth2 and apiKey across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the browser-login flow(s).
provider_name: TabTabTab
provider_slug: tabtabtab
scheme_count: 3
schemes:
- description: The tabtabtab CLI authenticates via `tabtabtab auth login`, a browser OAuth flow, and calls the control plane at api.tabtabtab.ai.
  name: cli-oauth
  scheme: browser-login
  sources:
  - docs
  - tabtabtab-skill
  type: oauth2
- description: Each inbound webhook is a secret URL (https://<env>.tabtabtab.app/webhooks/<token>). The full URL is the credential, shown once at creation and revocable.
  in: url
  name: webhook-secret-url
  sources:
  - docs/webhooks
  type: apiKey
- description: Per-environment Slack integration uses a bot token + signing secret, stored encrypted on the environment and never shown back in the UI.
  in: header
  name: slack-bot
  sources:
  - docs/slack
  type: apiKey
slug: tabtabtab-authentication
source_filename: tabtabtab-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://tabtabtab.ai/docs.md\ndocs: https://tabtabtab.ai/docs/cli-reference\nsummary:\n  types: [oauth2, apiKey]\n  api_key_in: [url]\n  oauth2_flows: [browser-login]\n  note: >-\n    No OpenAPI is published, so this profile is captured from the developer\n    docs and the official CLI/skill rather than derived from securitySchemes.\nschemes:\n  - name: cli-oauth\n    type: oauth2\n    scheme: browser-login\n    description: >-\n      The tabtabtab CLI authenticates via `tabtabtab auth login`, a browser\n      OAuth flow, and calls the control plane at api.tabtabtab.ai.\n    sources: [docs, tabtabtab-skill]\n  - name: webhook-secret-url\n    type: apiKey\n    in: url\n    description: >-\n      Each inbound webhook is a secret URL (https://<env>.tabtabtab.app/webhooks/<token>).\n      The full URL is the credential, shown once at creation and revocable.\n    sources: [docs/webhooks]\n  - name: slack-bot\n    type: apiKey\n\
  \    in: header\n    description: >-\n      Per-environment Slack integration uses a bot token + signing secret,\n      stored encrypted on the environment and never shown back in the UI.\n    sources: [docs/slack]\nruntime_secrets:\n  model: >-\n    Application credentials (API keys, DB URLs) are set once in the dashboard,\n    stored encrypted and environment-scoped, and injected at runtime without the\n    raw value being exposed to the agent, transcript, or output.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tabtabtab/refs/heads/main/authentication/tabtabtab-authentication.yml
summary_line: oauth2/apiKey · 3 schemes
tags:
- Company
- Agents
- AI
- Coding Agents
- Developer Tools
- Automation
- Webhooks
- CLI
- DevOps
- Cloud Development Environments
---
