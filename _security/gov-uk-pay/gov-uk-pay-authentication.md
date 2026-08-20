---
api_key_in: []
api_specs:
- filename: gov-uk-pay-agreements-api-openapi.yml
  format: yaml
  label: GOV.UK Pay Agreements API
  slug: gov-uk-pay-agreements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gov-uk-pay/refs/heads/main/openapi/gov-uk-pay-agreements-api-openapi.yml
- filename: gov-uk-pay-authorise-card-payments-api-openapi.yml
  format: yaml
  label: GOV.UK Pay Authorise card payments API
  slug: gov-uk-pay-authorise-card-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gov-uk-pay/refs/heads/main/openapi/gov-uk-pay-authorise-card-payments-api-openapi.yml
- filename: gov-uk-pay-card-payments-api-openapi.yml
  format: yaml
  label: GOV.UK Pay Card payments API
  slug: gov-uk-pay-card-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gov-uk-pay/refs/heads/main/openapi/gov-uk-pay-card-payments-api-openapi.yml
- filename: gov-uk-pay-disputes-api-openapi.yml
  format: yaml
  label: GOV.UK Pay Disputes API
  slug: gov-uk-pay-disputes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gov-uk-pay/refs/heads/main/openapi/gov-uk-pay-disputes-api-openapi.yml
- filename: gov-uk-pay-refunding-card-payments-api-openapi.yml
  format: yaml
  label: GOV.UK Pay Refunding card payments API
  slug: gov-uk-pay-refunding-card-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gov-uk-pay/refs/heads/main/openapi/gov-uk-pay-refunding-card-payments-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Gov Uk Pay Authentication
name_suffix: Authentication
oauth_flows: []
overview: GOV.UK Pay secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: GOV.UK Pay
provider_slug: gov-uk-pay
scheme_count: 1
schemes:
- description: 'GOV.UK Pay authenticates API calls with [OAuth2 HTTP bearer tokens](http://tools.ietf.org/html/rfc6750). You need to use an `"Authorization"` HTTP header to provide your API key, with a `"Bearer"` prefix. For example: `Authorization: Bearer {YOUR_API_KEY_HERE}`'
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/openapi.json
  type: http
slug: gov-uk-pay-authentication
source_filename: gov-uk-pay-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: 'GOV.UK Pay authenticates API calls with [OAuth2 HTTP bearer tokens](http://tools.ietf.org/html/rfc6750).\n    You need to use an `\"Authorization\"` HTTP header to provide your API key, with a `\"Bearer\"`\n    prefix. For example: `Authorization: Bearer {YOUR_API_KEY_HERE}`'\n  sources:\n  - openapi/openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gov-uk-pay/refs/heads/main/authentication/gov-uk-pay-authentication.yml
summary_line: http · 1 scheme
tags:
- Payments
- Government
- UK
- Public Sector
- REST
- PCI DSS
- Refunds
- Recurring Payments
- Webhook
---
