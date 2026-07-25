---
api_key_in:
- header
api_specs:
- filename: digicert-account-api-openapi.yml
  format: yaml
  label: Digicert Account API
  slug: digicert-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/digicert/refs/heads/main/openapi/digicert-account-api-openapi.yml
- filename: digicert-domain-api-openapi.yml
  format: yaml
  label: Digicert Domain API
  slug: digicert-domain-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/digicert/refs/heads/main/openapi/digicert-domain-api-openapi.yml
- filename: digicert-order-api-openapi.yml
  format: yaml
  label: Digicert Order API
  slug: digicert-order-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/digicert/refs/heads/main/openapi/digicert-order-api-openapi.yml
- filename: digicert-organization-api-openapi.yml
  format: yaml
  label: Digicert Organization API
  slug: digicert-organization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/digicert/refs/heads/main/openapi/digicert-organization-api-openapi.yml
- filename: digicert-user-api-openapi.yml
  format: yaml
  label: Digicert User API
  slug: digicert-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/digicert/refs/heads/main/openapi/digicert-user-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Digicert Authentication
name_suffix: Authentication
oauth_flows: []
overview: Digicert secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Digicert
provider_slug: digicert
scheme_count: 1
schemes:
- in: header
  name: apiKey
  parameter: X-DC-DEVKEY
  sources:
  - openapi/digicert-openapi.yml
  type: apiKey
slug: digicert-authentication
source_filename: digicert-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/digicert-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  parameter: X-DC-DEVKEY\n  sources:\n  - openapi/digicert-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/digicert/refs/heads/main/authentication/digicert-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Certificates
- Encryption
- PKI
- SSL
- TLS
---
