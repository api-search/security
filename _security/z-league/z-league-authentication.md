---
api_key_in: []
api_specs:
- filename: z-league-crm-lead-openapi.json
  format: json
  label: MEGA Public CRM Lead API
  slug: mega-public-crm-lead-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/z-league/refs/heads/main/openapi/z-league-crm-lead-openapi.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Z League Authentication
name_suffix: Authentication
oauth_flows: []
overview: Z League secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Z League
provider_slug: z-league
scheme_count: 1
schemes:
- description: 'Admin-issued Personal Access Token (PAT), e.g. `Authorization: Bearer mega_<64 hex>`. Keys are issued by MEGA and delivered securely (there is no self-serve key portal — request one from your MEGA account manager or support@gomega.ai). Each key is customer-locked (using it with a different x-customer-id returns 403), scoped, and shown only once.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/z-league-crm-lead-openapi.json
  type: http
slug: z-league-authentication
source_filename: z-league-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/z-league-crm-lead-openapi.json\ndocs: https://docs.gomega.ai/authentication\nsummary:\n  types:\n  - http\n  http_schemes:\n  - bearer\n  key_delivery: admin-issued (no self-serve key portal)\n  key_prefix: mega_\n  customer_scoped: true\n  extra_required_header: x-customer-id\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: >-\n    Admin-issued Personal Access Token (PAT), e.g. `Authorization: Bearer mega_<64 hex>`.\n    Keys are issued by MEGA and delivered securely (there is no self-serve key portal —\n    request one from your MEGA account manager or support@gomega.ai). Each key is\n    customer-locked (using it with a different x-customer-id returns 403), scoped, and\n    shown only once.\n  sources:\n  - openapi/z-league-crm-lead-openapi.json\nrequired_headers:\n- name: Authorization\n  value: 'Bearer mega_<token>'\n- name: x-customer-id\n  value: UUID of the customer the request acts\
  \ on; must match the customer the key is locked to\nscopes:\n- scope: public_api:leads:read\n  grants: GET /api/agents/crm/leads\n- scope: public_api:leads:write\n  grants: POST /api/agents/crm/leads, POST /api/agents/crm/leads/bulk\n- scope: public_api:webhooks:manage\n  grants: The /api/agents/crm/lead-webhooks endpoints (list/create/update/delete)\nnotes:\n- Server-to-server only — secret-key endpoints; never call from a browser or mobile client.\n- Missing/invalid token or missing x-customer-id returns 401; missing scope or wrong customer returns 403.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/z-league/refs/heads/main/authentication/z-league-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- CRM
- Leads
- Marketing
- AI Agents
- SEO
- Advertising
- Webhooks
- Gaming
---
