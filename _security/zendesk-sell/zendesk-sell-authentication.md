---
api_key_in: []
api_specs:
- filename: zendesk-sell-openapi.yml
  format: yaml
  label: Zendesk Sell (Sales CRM) API
  slug: sales-crm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zendesk-sell/refs/heads/main/openapi/zendesk-sell-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Zendesk Sell Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Zendesk Sell secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Zendesk Sell
provider_slug: zendesk-sell
scheme_count: 1
schemes:
- description: OAuth 2.0 (authorization code, implicit, password, and refresh token grants).
  flows:
  - authorizationUrl: https://api.getbase.com/oauth2/authorize
    flow: authorizationCode
    scopes: 2
    tokenUrl: https://api.getbase.com/oauth2/token
  name: oauth2
  sources:
  - openapi/zendesk-sell-openapi.yml
  type: oauth2
slug: zendesk-sell-authentication
source_filename: zendesk-sell-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/zendesk-sell-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://api.getbase.com/oauth2/authorize\n    tokenUrl: https://api.getbase.com/oauth2/token\n    scopes: 2\n  description: OAuth 2.0 (authorization code, implicit, password, and refresh token grants).\n  sources:\n  - openapi/zendesk-sell-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zendesk-sell/refs/heads/main/authentication/zendesk-sell-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- CRM
- Sales
- Sales Automation
- Leads
- Deals
- Pipeline
- Customer Experience
---
