---
api_key_in: []
api_specs:
- filename: synchrony-financial-credit-authorization-openapi.yml
  format: yaml
  label: Synchrony Credit Authorization API
  slug: credit-authorization
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/synchrony-financial/refs/heads/main/openapi/synchrony-financial-credit-authorization-openapi.yml
- filename: synchrony-financial-quickscreen-apply-openapi.yml
  format: yaml
  label: Synchrony Quickscreen Apply API
  slug: quickscreen-apply
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/synchrony-financial/refs/heads/main/openapi/synchrony-financial-quickscreen-apply-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Synchrony Financial Authentication
name_suffix: Authentication
oauth_flows: []
overview: Synchrony Financial secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Synchrony Financial
provider_slug: synchrony-financial
scheme_count: 1
schemes:
- name: bearerAuth
  scheme: bearer
  sources:
  - openapi/synchrony-financial-credit-authorization-openapi.yml
  - openapi/synchrony-financial-quickscreen-apply-openapi.yml
  type: http
slug: synchrony-financial-authentication
source_filename: synchrony-financial-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/synchrony-financial-credit-authorization-openapi.yml, openapi/synchrony-financial-quickscreen-apply-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/synchrony-financial-credit-authorization-openapi.yml\n  - openapi/synchrony-financial-quickscreen-apply-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/synchrony-financial/refs/heads/main/authentication/synchrony-financial-authentication.yml
summary_line: http · 1 scheme
tags:
- Financial Services
- Credit
- Payments
- Consumer Finance
- Retail Finance
---
