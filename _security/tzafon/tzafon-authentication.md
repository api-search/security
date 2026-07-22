---
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Tzafon Authentication
name_suffix: Authentication
oauth_flows: []
overview: Tzafon secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Tzafon
provider_slug: tzafon
scheme_count: 1
schemes:
- description: All API requests require a Bearer token. API keys start with the sk_ prefix, are scoped to the organization, and are hashed at rest (shown once at creation). SDKs read the key from the TZAFON_API_KEY environment variable by default; base URL default is https://api.tzafon.ai (override with LIGHTCONE_BASE_URL).
  env_var: TZAFON_API_KEY
  key_prefix: sk_
  name: bearerAuth
  scheme: bearer
  type: http
slug: tzafon-authentication
source_filename: tzafon-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\ndocs: https://docs.lightcone.ai/guides/authentication\nsource: https://docs.lightcone.ai/guides/authentication + https://docs.lightcone.ai/guides/security\nsummary:\n  types: [http]\n  schemes: [bearer]\n  oauth2_flows: []\nschemes:\n  - name: bearerAuth\n    type: http\n    scheme: bearer\n    description: >-\n      All API requests require a Bearer token. API keys start with the sk_\n      prefix, are scoped to the organization, and are hashed at rest (shown\n      once at creation). SDKs read the key from the TZAFON_API_KEY environment\n      variable by default; base URL default is https://api.tzafon.ai\n      (override with LIGHTCONE_BASE_URL).\n    key_prefix: sk_\n    env_var: TZAFON_API_KEY\nnotes:\n  - Temporary keys are supported for short-lived or scoped access (CI jobs, limited service access).\n  - Keys can be revoked at any time in the dashboard (https://lightcone.ai/dashboard).\n  - 10 failed authentication attempts\
  \ in 10 minutes will block the client IP.\n  - The CLI also supports browser device-flow sign-in (lightcone login), inheriting org SSO and MFA.\n  - Designed for server-side use; do not embed keys in client-side code.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tzafon/refs/heads/main/authentication/tzafon-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Artificial Intelligence
- Computer Use Agents
- Browser Automation
- AI Agents
- Vision Language Models
- Cloud Computers
- Automation
---
