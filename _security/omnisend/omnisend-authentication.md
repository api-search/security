---
api_key_in:
- header
api_specs:
- filename: omnisend-openapi.yml
  format: yaml
  label: Omnisend REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/omnisend/refs/heads/main/openapi/omnisend-openapi.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Omnisend Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Omnisend secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Omnisend
provider_slug: omnisend
scheme_count: 2
schemes:
- in: header
  name: ApiKeyAuth
  parameter: X-API-KEY
  sources:
  - openapi/omnisend-openapi.yml
  type: apiKey
- flows:
  - authorizationUrl: https://app.omnisend.com/oauth/authorize
    flow: authorizationCode
    scopes: 5
    tokenUrl: https://api.omnisend.com/v5/oauth/token
  name: OAuth2
  sources:
  - openapi/omnisend-openapi.yml
  type: oauth2
slug: omnisend-authentication
source_filename: omnisend-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/omnisend-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-KEY\n  sources:\n  - openapi/omnisend-openapi.yml\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://app.omnisend.com/oauth/authorize\n    tokenUrl: https://api.omnisend.com/v5/oauth/token\n    scopes: 5\n  sources:\n  - openapi/omnisend-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/omnisend/refs/heads/main/authentication/omnisend-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Email Marketing
- Marketing Automation
- Ecommerce
- SMS Marketing
- Customer Engagement
- Segmentation
- Campaigns
- Forms
- Popups
- Web Push
---
