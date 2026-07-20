---
api_key_in:
- header
api_specs:
- filename: delivery-hero-on-demand-rider-openapi.json
  format: json
  label: Delivery Hero On Demand Rider API
  slug: delivery-hero-on-demand-rider
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/delivery-hero/refs/heads/main/openapi/delivery-hero-on-demand-rider-openapi.json
auth_types:
- apiKey
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Delivery Hero Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Delivery Hero secures its APIs with apiKey and oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Delivery Hero
provider_slug: delivery-hero
scheme_count: 2
schemes:
- description: 'Provide the access token in the format: `Bearer {access-token}`. You can obtain the access token from the [Authentication endpoint](#tag/Authentication).'
  in: header
  name: Bearer_Token
  parameter: Authorization
  sources:
  - openapi/delivery-hero-on-demand-rider-openapi.json
  type: apiKey
- client_assertion_type: urn:ietf:params:oauth:client-assertion-type:jwt-bearer
  description: 'Machine-to-machine: register an RSA-2048 public key with ODR, sign a JWT assertion (kid, iss, sub, jti, exp, aud=https://sts.deliveryhero.io), exchange via client_credentials for a Bearer access token.'
  flow: clientCredentials
  name: OAuth2
  sources:
  - https://on-demand-rider-docs.deliveryhero.io/
  tokenUrl: https://sts.deliveryhero.io/oauth2/token
  type: oauth2
slug: delivery-hero-authentication
source_filename: delivery-hero-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: openapi/delivery-hero-on-demand-rider-openapi.json\nsummary:\n  types:\n  - apiKey\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: Bearer_Token\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: 'Provide the access token in the format: `Bearer {access-token}`. You\n    can obtain the access token from the [Authentication endpoint](#tag/Authentication).'\n  sources:\n  - openapi/delivery-hero-on-demand-rider-openapi.json\n- name: OAuth2\n  type: oauth2\n  flow: clientCredentials\n  tokenUrl: https://sts.deliveryhero.io/oauth2/token\n  client_assertion_type: urn:ietf:params:oauth:client-assertion-type:jwt-bearer\n  description: 'Machine-to-machine: register an RSA-2048 public key with ODR, sign\n    a JWT assertion (kid, iss, sub, jti, exp, aud=https://sts.deliveryhero.io), exchange\n    via client_credentials for a Bearer access token.'\n  sources:\n  -\
  \ https://on-demand-rider-docs.deliveryhero.io/\ndocs: https://on-demand-rider-docs.deliveryhero.io/\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/delivery-hero/refs/heads/main/authentication/delivery-hero-authentication.yml
summary_line: apiKey/oauth2 · 2 schemes
tags:
- Company
- Technology
- Food Delivery
- Logistics
- Quick Commerce
- Last Mile Delivery
- On Demand
- Orders
---
