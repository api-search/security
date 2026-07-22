---
api_key_in:
- header
auth_types:
- http
description: Authentication profile captured from the Wordware API documentation. API keys are generated per user in the app (avatar menu -> API Keys) and passed as a bearer token in the Authorization header on every request to the WordApps run API. No OAuth 2.0, OpenID Connect, or mTLS surface is documented, and no openid-configuration / oauth-authorization-server well-known documents are published (both probed 404).
kind: authentication
layout: security
method: searched
name: Wordware Authentication
name_suffix: Authentication
oauth_flows: []
overview: Wordware secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Wordware
provider_slug: wordware
scheme_count: 1
schemes:
- header: 'Authorization: Bearer <API_KEY>'
  key_management: https://app.wordware.ai (Settings -> API Keys)
  name: bearerAuth
  scheme: bearer
  sources:
  - https://docs.wordware.ai/api.md
  type: http
slug: wordware-authentication
source_filename: wordware-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\ndocs: https://docs.wordware.ai/api\ndescription: >-\n  Authentication profile captured from the Wordware API documentation. API\n  keys are generated per user in the app (avatar menu -> API Keys) and passed\n  as a bearer token in the Authorization header on every request to the\n  WordApps run API. No OAuth 2.0, OpenID Connect, or mTLS surface is\n  documented, and no openid-configuration / oauth-authorization-server\n  well-known documents are published (both probed 404).\nsummary:\n  types: [http]\n  schemes: [bearer]\n  api_key_in: [header]\n  oauth2_flows: []\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  header: \"Authorization: Bearer <API_KEY>\"\n  key_management: https://app.wordware.ai (Settings -> API Keys)\n  sources: [https://docs.wordware.ai/api.md]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wordware/refs/heads/main/authentication/wordware-authentication.yml
summary_line: http · 1 scheme
tags:
- Artificial Intelligence
- AI Agents
- LLM
- Prompt Engineering
- Workflow Automation
- No Code
- Company
---
