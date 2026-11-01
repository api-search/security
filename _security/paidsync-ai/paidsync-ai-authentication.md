---
anonymous_access: false
api_key_in: []
api_specs:
- filename: paidsync-ai-billing-api-openapi.yml
  format: yaml
  label: paidsync-ai Billing API
  slug: paidsync-ai-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/paidsync-ai/openapi/paidsync-ai-billing-api-openapi.yml
- filename: paidsync-ai-mcp-api-openapi.yml
  format: yaml
  label: paidsync-ai MCP API
  slug: paidsync-ai-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/paidsync-ai/openapi/paidsync-ai-mcp-api-openapi.yml
- filename: paidsync-ai-paidsync-api-api-openapi.yml
  format: yaml
  label: paidsync-ai PaidSync API
  slug: paidsync-ai-paidsync-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/paidsync-ai/openapi/paidsync-ai-paidsync-api-api-openapi.yml
- filename: paidsync-ai-payment-api-openapi.yml
  format: yaml
  label: paidsync-ai Payment API
  slug: paidsync-ai-payment-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/paidsync-ai/openapi/paidsync-ai-payment-api-openapi.yml
- filename: paidsync-ai-subscribe-api-openapi.yml
  format: yaml
  label: paidsync-ai Subscribe API
  slug: paidsync-ai-subscribe-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/paidsync-ai/openapi/paidsync-ai-subscribe-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Paidsync Ai Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: paidsync-ai secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: paidsync-ai
provider_slug: paidsync-ai
scheme_count: 1
schemes:
- flows:
  - authorizationUrl: https://api.paidsync.ai/authorize
    flow: authorizationCode
    scopes: 4
    tokenUrl: https://api.paidsync.ai/token
  name: oauth2
  sources:
  - openapi/paidsync-ai-openapi.json
  type: oauth2
slug: paidsync-ai-authentication
source_filename: paidsync-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: derived\nsource: openapi/paidsync-ai-openapi.json\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.paidsync.ai/authorize\n    tokenUrl: https://api.paidsync.ai/token\n    scopes: 4\n  sources:\n  - openapi/paidsync-ai-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/paidsync-ai/authentication/paidsync-ai-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- AI
- Advertising
- Automation
- Marketing
---
