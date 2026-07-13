---
api_key_in:
- header
api_specs:
- filename: wix-openapi.yml
  format: yaml
  label: Wix REST API
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wix/refs/heads/main/openapi/wix-openapi.yml
- filename: wix-asyncapi.yml
  format: yaml
  label: Wix Webhooks
  slug: webhooks
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/wix/refs/heads/main/asyncapi/wix-asyncapi.yml
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Wix Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Wix secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Wix
provider_slug: wix
scheme_count: 2
schemes:
- description: OAuth 2.0 for Wix third-party apps
  flows:
  - authorizationUrl: https://www.wix.com/installer/install
    flow: authorizationCode
    scopes: 0
    tokenUrl: https://www.wixapis.com/oauth2/token
  name: oauth2
  sources:
  - openapi/wix-openapi.yml
  type: oauth2
- description: API key authentication (Wix-account-only; not for third-party apps)
  in: header
  name: apiKey
  parameter: Authorization
  sources:
  - openapi/wix-openapi.yml
  type: apiKey
slug: wix-authentication
source_filename: wix-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/wix-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://www.wix.com/installer/install\n    tokenUrl: https://www.wixapis.com/oauth2/token\n    scopes: 0\n  description: OAuth 2.0 for Wix third-party apps\n  sources:\n  - openapi/wix-openapi.yml\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: API key authentication (Wix-account-only; not for third-party apps)\n  sources:\n  - openapi/wix-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wix/refs/heads/main/authentication/wix-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- CMS
- eCommerce
- Headless
- Website Builder
---
