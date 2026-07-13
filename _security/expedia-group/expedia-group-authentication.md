---
api_key_in:
- header
api_specs:
- filename: expedia-rapid-openapi-original.yml
  format: yaml
  label: Expedia Rapid API
  slug: rapid
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/expedia-group/refs/heads/main/openapi/expedia-rapid-openapi-original.yml
- filename: expedia-fraud-protection-openapi-original.yml
  format: yaml
  label: Expedia Fraud Protection API
  slug: fraud-protection
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/expedia-group/refs/heads/main/openapi/expedia-fraud-protection-openapi-original.yml
- filename: expedia-lodging-product-openapi-original.yml
  format: yaml
  label: Expedia Lodging API
  slug: lodging
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/expedia-group/refs/heads/main/openapi/expedia-lodging-product-openapi-original.yml
- filename: expedia-deposit-openapi-original.yml
  format: yaml
  label: Expedia EPS Deposit API
  slug: deposit
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/expedia-group/refs/heads/main/openapi/expedia-deposit-openapi-original.yml
- filename: expedia-loyalty-openapi-original.yml
  format: yaml
  label: Expedia Loyalty Earn API
  slug: loyalty
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/expedia-group/refs/heads/main/openapi/expedia-loyalty-openapi-original.yml
auth_types:
- apiKey
- http
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Expedia Group Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Expedia Group secures its APIs with apiKey, http, and oauth2 across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Expedia Group
provider_slug: expedia-group
scheme_count: 3
schemes:
- name: Basic
  scheme: basic
  sources:
  - openapi/expedia-deposit-openapi-original.yml
  - openapi/expedia-lodging-product-openapi-original.yml
  type: http
- flows:
  - flow: clientCredentials
    scopes: 1
    tokenUrl: https://api.expediagroup.com/identity/oauth2/v3/token?grant_type=client_credentials
  name: orderPurchaseScreenAuth
  sources:
  - openapi/expedia-fraud-protection-openapi-original.yml
  - openapi/expedia-loyalty-openapi-original.yml
  type: oauth2
- description: The custom generated authentication header. Refer to our [signature authentication](https://developers.expediagroup.com/docs/rapid/resources/reference/signature-authentication) page for full details.
  in: header
  name: rapidAuth
  parameter: Authorization
  sources:
  - openapi/expedia-rapid-openapi-original.yml
  type: apiKey
slug: expedia-group-authentication
source_filename: expedia-group-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/expedia-deposit-openapi-original.yml, openapi/expedia-fraud-protection-openapi-original.yml,\n  openapi/expedia-lodging-product-openapi-original.yml, openapi/expedia-loyalty-openapi-original.yml,\n  openapi/expedia-rapid-openapi-original.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: Basic\n  type: http\n  scheme: basic\n  sources:\n  - openapi/expedia-deposit-openapi-original.yml\n  - openapi/expedia-lodging-product-openapi-original.yml\n- name: orderPurchaseScreenAuth\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.expediagroup.com/identity/oauth2/v3/token?grant_type=client_credentials\n    scopes: 1\n  sources:\n  - openapi/expedia-fraud-protection-openapi-original.yml\n  - openapi/expedia-loyalty-openapi-original.yml\n- name: rapidAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n\
  \  description: The custom generated authentication header. Refer to our [signature authentication](https://developers.expediagroup.com/docs/rapid/resources/reference/signature-authentication)\n    page for full details.\n  sources:\n  - openapi/expedia-rapid-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/expedia-group/refs/heads/main/authentication/expedia-group-authentication.yml
summary_line: apiKey/http/oauth2 · 3 schemes
tags:
- Flights
- Hotels
- Lodging
- Travel
- Fortune 500
---
