---
api_key_in: []
api_specs:
- filename: sentrial-openapi.yml
  format: yaml
  label: Sentrial SDK API
  slug: sentrial-sdk-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sentrial/refs/heads/main/openapi/sentrial-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Sentrial Authentication
name_suffix: Authentication
oauth_flows: []
overview: Sentrial secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Sentrial
provider_slug: sentrial
scheme_count: 1
schemes:
- description: API key passed as a Bearer token in the Authorization header. Keys follow the format sentrial_live_xxxxxxxxxxxxx and are created in organization Settings -> API Keys.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/sentrial-openapi.yml
  type: http
slug: sentrial-authentication
source_filename: sentrial-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/sentrial-openapi.yml\ndocs: https://www.sentrial.com/docs/api/auth\nsummary:\n  types:\n  - http\n  key_format: sentrial_live_xxxxxxxxxxxxx\n  header: 'Authorization: Bearer <api_key>'\n  key_management: Organization Settings -> API Keys (keys shown once)\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: API key passed as a Bearer token in the Authorization header. Keys follow the\n    format sentrial_live_xxxxxxxxxxxxx and are created in organization Settings -> API Keys.\n  sources:\n  - openapi/sentrial-openapi.yml\nerrors:\n- status: 401\n  error: Unauthorized\n  message: Invalid or missing API key\n- status: 403\n  error: Forbidden\n  message: API key does not have access to this resource\nbest_practices:\n- Store API keys in environment variables (SENTRIAL_API_KEY), never in code.\n- Rotate keys regularly and revoke compromised keys immediately in Settings.\n- Use separate keys per\
  \ environment (dev, staging, production).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sentrial/refs/heads/main/authentication/sentrial-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- AI Agents
- Observability
- Monitoring
- LLM
- Developer Tools
- Tracing
---
