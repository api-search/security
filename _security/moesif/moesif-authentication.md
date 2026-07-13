---
api_key_in: []
api_specs:
- filename: moesif-openapi.yml
  format: yaml
  label: Moesif Management API
  slug: moesif
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moesif/refs/heads/main/openapi/moesif-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Moesif Authentication
name_suffix: Authentication
oauth_flows:
- password
overview: Moesif secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the password flow(s).
provider_name: Moesif
provider_slug: moesif
scheme_count: 1
schemes:
- description: "Your Management API token must be added to the request _Authorization_ header using the following format:\n\n `Authorization: Bearer YOUR_MANAGEMENT_API_KEY`"
  flows:
  - flow: password
    scopes: 41
    tokenUrl: https://api.moesif.com/v1/:orgId/oauth/access_tokens
  name: managementAPIToken
  sources:
  - openapi/moesif-openapi.json
  - openapi/moesif-openapi.yml
  type: oauth2
slug: moesif-authentication
source_filename: moesif-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/moesif-openapi.json, openapi/moesif-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - password\nschemes:\n- name: managementAPIToken\n  type: oauth2\n  flows:\n  - flow: password\n    tokenUrl: https://api.moesif.com/v1/:orgId/oauth/access_tokens\n    scopes: 41\n  description: |-\n    Your Management API token must be added to the request _Authorization_ header using the following format:\n\n     `Authorization: Bearer YOUR_MANAGEMENT_API_KEY`\n  sources:\n  - openapi/moesif-openapi.json\n  - openapi/moesif-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/moesif/refs/heads/main/authentication/moesif-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Analytics
- Monitoring
- Monetization
- Governance
- Observability
- Billing
- AI Agents
- LLM Analytics
- OpenTelemetry
- Developer Portal
- Platform
- Insights
---
