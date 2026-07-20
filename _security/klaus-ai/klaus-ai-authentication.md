---
api_key_in:
- header
auth_types:
- apiKey
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Klaus Ai Authentication
name_suffix: Authentication
oauth_flows:
- deviceCode
overview: Klaus AI secures its APIs with apiKey, http, and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the deviceCode flow(s).
provider_name: Klaus AI
provider_slug: klaus-ai
scheme_count: 3
schemes:
- create_at: https://klausai.com/account
  description: Personal API key created at https://klausai.com/account. The CLI reads it from the KLAUS_API_KEY environment variable first, then from its on-disk config file.
  env_var: KLAUS_API_KEY
  in: header
  name: apiKeyAuth
  parameter_name: x-api-key
  sources:
  - npm:@klausai/cli@0.1.7
  type: apiKey
- description: 'Session access token issued by the device authorization grant, sent as Authorization: Bearer <token>.'
  name: bearerAuth
  scheme: bearer
  sources:
  - npm:@klausai/cli@0.1.7
  type: http
- flows:
  - client_id: klaus-cli
    device_authorization_url: https://api.klausai.com/api/auth/device/code
    flow: deviceCode
    grant_type: urn:ietf:params:oauth:grant-type:device_code
    scopes: []
    scopes_note: The device grant as implemented by the CLI requests no scopes; Klaus documents no scope registry.
    standard: RFC 8628 OAuth 2.0 Device Authorization Grant
    token_url: https://api.klausai.com/api/auth/device/token
  name: deviceGrant
  sources:
  - npm:@klausai/cli@0.1.7
  type: oauth2
slug: klaus-ai-authentication
source_filename: klaus-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: derived\nsource: npm @klausai/cli@0.1.7 (dist/klaus.js published bundle); https://klausai.com/terms/; https://klausai.com/privacy/\ndocs: https://klausai.com/account\nnote: >-\n  Klaus publishes no OpenAPI description, so 0-working/derive-authentication.py had nothing to read. This\n  profile was derived from the provider's own published npm client (@klausai/cli), which is the authoritative\n  first-party implementation of the auth handshake, plus the Terms and Privacy pages for end-user account auth.\nsummary:\n  types:\n  - apiKey\n  - http\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - deviceCode\n  end_user_identity: Google OAuth (account registration, per Terms of Service section 3)\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter_name: x-api-key\n  description: >-\n    Personal API key created at https://klausai.com/account. The CLI reads it from the KLAUS_API_KEY\n    environment variable first, then\
  \ from its on-disk config file.\n  env_var: KLAUS_API_KEY\n  create_at: https://klausai.com/account\n  sources:\n  - npm:@klausai/cli@0.1.7\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: >-\n    Session access token issued by the device authorization grant, sent as Authorization: Bearer <token>.\n  sources:\n  - npm:@klausai/cli@0.1.7\n- name: deviceGrant\n  type: oauth2\n  flows:\n  - flow: deviceCode\n    standard: RFC 8628 OAuth 2.0 Device Authorization Grant\n    device_authorization_url: https://api.klausai.com/api/auth/device/code\n    token_url: https://api.klausai.com/api/auth/device/token\n    grant_type: 'urn:ietf:params:oauth:grant-type:device_code'\n    client_id: klaus-cli\n    scopes: []\n    scopes_note: The device grant as implemented by the CLI requests no scopes; Klaus documents no scope registry.\n  sources:\n  - npm:@klausai/cli@0.1.7\nrequest_scoping:\n- header: x-klaus-instance-id\n  description: Selects which hosted OpenClaw instance a request\
  \ targets when an account has more than one.\nwebhook_authentication:\n  description: >-\n    Instance webhooks are created from the Klaus Integrations page and issue a URL plus a token; external\n    services send authenticated HTTP requests to that URL to trigger the agent.\n  source: https://klausai.com/faq/\nintegration_authentication:\n  description: >-\n    Downstream provider credentials (Google Workspace OAuth, Slack, GitHub, AgentMail, OpenRouter BYOK,\n    ChatGPT subscription linking) are connected per-instance from the Integrations and Billing pages, with\n    user-selectable Google permission scopes (none, read-only, or full access).\n  source: https://klausai.com/privacy/\nscopes_artifact: null\nscopes_note: >-\n  No OAuth scope registry is published for the Klaus platform API itself, so scopes/ is intentionally absent.\n  The only user-facing scope selection is over Google Workspace, which is Google's scope surface, not Klaus's.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/klaus-ai/refs/heads/main/authentication/klaus-ai-authentication.yml
summary_line: apiKey/http/oauth2 · 3 schemes
tags:
- Artificial Intelligence
- AI Agents
- Agent Hosting
- OpenClaw
- Personal Assistant
- Automation
- Managed Hosting
- Integrations
- Webhooks
- Command Line
- Messaging
- Y Combinator
---
