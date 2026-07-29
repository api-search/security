---
api_key_in: []
api_specs:
- filename: openapi
  format: yaml
  label: Attio REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://docs.attio.com/rest-api/endpoint-reference/openapi
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Attio Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Attio secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Attio
provider_slug: attio
scheme_count: 2
schemes:
- description: Attio API key or OAuth bearer token.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/attio-openapi.yml
  type: http
- flows:
  - authorizationUrl: https://app.attio.com/authorize
    flow: authorizationCode
    scopes: 7
    tokenUrl: https://api.attio.com/oauth/token
  name: oauth2
  sources:
  - openapi/attio-openapi.yml
  type: oauth2
slug: attio-authentication
source_filename: attio-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/attio-openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Attio API key or OAuth bearer token.\n  sources:\n  - openapi/attio-openapi.yml\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://app.attio.com/authorize\n    tokenUrl: https://api.attio.com/oauth/token\n    scopes: 7\n  sources:\n  - openapi/attio-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/attio/refs/heads/main/authentication/attio-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- CRM
- Customer Relationship Management
- Sales
- Contacts
- Companies
- Pipeline
- Workflows
---
