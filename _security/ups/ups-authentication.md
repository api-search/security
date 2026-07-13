---
api_key_in: []
api_specs:
- filename: ups-shipping-openapi.yml
  format: yaml
  label: UPS Shipping API
  slug: ups-shipping
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ups/refs/heads/main/openapi/ups-shipping-openapi.yml
auth_types:
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Ups Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: UPS secures its APIs with http and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: UPS
provider_slug: ups
scheme_count: 2
schemes:
- flows:
  - flow: clientCredentials
    scopes: 0
    tokenUrl: https://onlinetools.ups.com/api/security/v1/oauth/token
  name: OAuth2
  sources:
  - openapi/ups-shipping-openapi.yml
  type: oauth2
- description: OAuth 2.0 bearer token from /security/v1/oauth/token
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/ups-shipping-openapi.yml
  type: http
slug: ups-authentication
source_filename: ups-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/ups-shipping-openapi.yml\nsummary:\n  types:\n  - http\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://onlinetools.ups.com/api/security/v1/oauth/token\n    scopes: 0\n  sources:\n  - openapi/ups-shipping-openapi.yml\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: OAuth 2.0 bearer token from /security/v1/oauth/token\n  sources:\n  - openapi/ups-shipping-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ups/refs/heads/main/authentication/ups-authentication.yml
summary_line: http/oauth2 · 2 schemes
tags:
- Logistics
- Shipping
- Fortune 500
- Supply Chain
---
