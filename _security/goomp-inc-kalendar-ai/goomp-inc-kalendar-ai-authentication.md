---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Goomp Inc Kalendar Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Goomp Inc, Kalendar AI declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Goomp Inc, Kalendar AI
provider_slug: goomp-inc-kalendar-ai
scheme_count: 1
schemes:
- authorization_content_type: application/json
  authorization_url: https://kalendar.ai/chatgpt/authorize_callback.json
  client_registration_url: https://kalendar.ai/users/new/onboard/
  evidence: 'ai-plugin.json auth: {"type":"oauth","scope":"read write"}'
  flow: authorization_code
  name: oauth
  scopes:
  - read
  - write
  source: https://api.oncockpit.ai/.well-known/ai-plugin.json
  type: oauth2
  user_authenticated: true
slug: goomp-inc-kalendar-ai-authentication
source_filename: goomp-inc-kalendar-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://api.oncockpit.ai/.well-known/ai-plugin.json\ndocs: null\nnote: >-\n  There is no OpenAPI to derive from — the only machine-readable statement the provider makes\n  about authentication is the `auth` block of its live ChatGPT plugin manifest, served from its\n  own API host (api.oncockpit.ai, HTTP 200, application/json). It declares an OAuth flow with the\n  scopes \"read write\" and an authorization callback on the legacy kalendar.ai domain. The manifest\n  also names an OpenAPI at https://kalendar.ai/openapi.yaml; that URL now 301s to\n  https://oncockpit.ai/openapi.yaml, which returns the site's 5,130-byte SPA catch-all shell\n  (text/html), so the contract behind this auth flow is no longer published. Treat this profile as\n  the provider's last published position on auth, not as a live, documented developer program.\nschemes:\n- name: oauth\n  type: oauth2\n  flow: authorization_code\n  authorization_url: https://kalendar.ai/chatgpt/authorize_callback.json\n\
  \  client_registration_url: https://kalendar.ai/users/new/onboard/\n  authorization_content_type: application/json\n  scopes:\n  - read\n  - write\n  user_authenticated: true\n  source: https://api.oncockpit.ai/.well-known/ai-plugin.json\n  evidence: 'ai-plugin.json auth: {\"type\":\"oauth\",\"scope\":\"read write\"}'\nobservations:\n- surface: https://api.oncockpit.ai/\n  status: 200\n  body: '{\"name\":\"Cockpit AI API\",\"status\":\"active\",\"timestamp\":\"...\"}'\n  note: API host self-identifies but publishes no unauthenticated reference or spec\n- surface: https://api.oncockpit.ai/health\n  status: 200\n  body: OK\n- surface: https://kalendar.ai/openapi.yaml\n  status: 301\n  note: redirects to oncockpit.ai/openapi.yaml which returns the SPA shell, not a spec\ngaps:\n- No public authentication documentation page was found on oncockpit.ai or any subdomain.\n- No /.well-known/oauth-authorization-server or /.well-known/oauth-protected-resource is served.\n- No API key issuance flow\
  \ is documented publicly.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/goomp-inc-kalendar-ai/refs/heads/main/authentication/goomp-inc-kalendar-ai-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Artificial Intelligence
- Sales
- Sales Automation
- Outbound
- Lead Generation
- Scheduling
- Agents
- Email
- CRM
---
