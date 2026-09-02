---
api_key_in: []
api_specs:
- filename: legal-ge-public-apis-directory-api-openapi.yml
  format: yaml
  label: legal.ge Public APIs Directory API
  slug: legal-ge-public-apis-directory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/legal-ge-public-apis/refs/heads/main/openapi/legal-ge-public-apis-directory-api-openapi.yml
- filename: legal-ge-public-apis-matching-api-openapi.yml
  format: yaml
  label: legal.ge Public APIs Matching API
  slug: legal-ge-public-apis-matching-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/legal-ge-public-apis/refs/heads/main/openapi/legal-ge-public-apis-matching-api-openapi.yml
auth_types:
- none
description: ''
kind: authentication
layout: security
method: searched
name: Legal Ge Public Apis Authentication
name_suffix: Authentication
oauth_flows: []
overview: legal.ge Public APIs secures its APIs with none across 0 declared security schemes, as derived from its OpenAPI definitions.
provider_name: legal.ge Public APIs
provider_slug: legal-ge-public-apis
scheme_count: 0
schemes: []
slug: legal-ge-public-apis-authentication
source_filename: legal-ge-public-apis-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-09'\nmethod: searched\nsource: https://legal.ge/llms.txt + openapi/legal-ge-public-apis-openapi.yml\ndocs: https://legal.ge/llms.txt\nsummary:\n  types: [none]\n  keyless: true\n  api_key_in: []\n  oauth2_flows: []\n  note: >-\n    The OpenAPI 3.1 document declares NO components.securitySchemes and no global or per-operation\n    `security` requirement. This is not a thin spec — the API is genuinely public and keyless by\n    design, documented as such in llms.txt and in the MCP server README (\"No keys required. The\n    legal.ge Ask API is public; rate-limited per IP.\").\nschemes: []\naccess_control:\n  model: anonymous-public-read\n  gate: per-IP rate limiting only\n  sources:\n    - openapi/legal-ge-public-apis-openapi.yml\n    - https://legal.ge/llms.txt\n    - https://github.com/infolegalge/legal.ge-mcp\nprivileged_surface:\n  description: >-\n    The one PII-bearing operation, GET /api/specialists/{id}/contact, is not protected by a\n    credential\
  \ either — it is protected by CONSENT plus throttling: the field is returned only when\n    the profile set info_activate=true and is in a public compliance state, and the endpoint is\n    capped at 10 requests/minute per IP explicitly \"to make bulk PII harvest impractical\".\n  operationId: revealSpecialistContact\nwhat_requires_sign_in:\n  - Sending an inquiry or message to a specialist (interactive sign-in on legal.ge; not exposed via API).\n  - Dashboards (specialist, company, client, trainer, author, litigation cabinet) — all Disallowed in robots.txt.\noauth_discovery:\n  '/.well-known/openid-configuration': 404\n  '/.well-known/oauth-authorization-server': 404\nscopes:\n  applicable: false\n  note: No OAuth surface, therefore no scope model. scopes/ is intentionally not emitted.\nx-evidence:\n  fetched: '2026-08-09'\n  url: https://legal.ge/api/openapi.json\n  http_status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/legal-ge-public-apis/refs/heads/main/authentication/legal-ge-public-apis-authentication.yml
summary_line: none · 0 schemes
tags:
- Legal
- Law
- Legal Services
- Directory
- Georgia
- AI Agents
- MCP
- specialists
- Professional Services
- Marketplace
- Multilingual
- Legal Tech
---
