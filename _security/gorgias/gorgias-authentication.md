---
api_key_in: []
api_specs:
- filename: gorgias-openapi.yml
  format: yaml
  label: Gorgias REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gorgias/refs/heads/main/openapi/gorgias-openapi.yml
- filename: gorgias-asyncapi.yml
  format: yaml
  label: Gorgias Webhooks
  slug: webhooks
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/gorgias/refs/heads/main/asyncapi/gorgias-asyncapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Gorgias Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Gorgias secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Gorgias
provider_slug: gorgias
scheme_count: 2
schemes:
- description: Use account email as username and API key as password
  name: basicAuth
  scheme: basic
  sources:
  - openapi/gorgias-openapi.yml
  type: http
- flows:
  - authorizationUrl: https://{account}.gorgias.com/oauth/authorize
    flow: authorizationCode
    scopes: 6
    tokenUrl: https://{account}.gorgias.com/oauth/token
  name: oauth2
  sources:
  - openapi/gorgias-openapi.yml
  type: oauth2
slug: gorgias-authentication
source_filename: gorgias-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/gorgias-openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: Use account email as username and API key as password\n  sources:\n  - openapi/gorgias-openapi.yml\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://{account}.gorgias.com/oauth/authorize\n    tokenUrl: https://{account}.gorgias.com/oauth/token\n    scopes: 6\n  sources:\n  - openapi/gorgias-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gorgias/refs/heads/main/authentication/gorgias-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Customer Support
- Helpdesk
- Ecommerce
- Shopify
- Tickets
- Conversations
---
