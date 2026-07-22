---
api_key_in: []
api_specs:
- filename: vendasta-marketplace-openapi-original.yml
  format: yaml
  label: Vendasta Marketplace API V1
  slug: vendasta-marketplace-api-v1
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vendasta/refs/heads/main/openapi/vendasta-marketplace-openapi-original.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Vendasta Authentication
name_suffix: Authentication
oauth_flows: []
overview: Vendasta secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Vendasta
provider_slug: vendasta
scheme_count: 1
schemes:
- name: BearerAuth
  scheme: bearer
  sources:
  - openapi/vendasta-marketplace-openapi-original.yml
  type: http
slug: vendasta-authentication
source_filename: vendasta-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/vendasta-marketplace-openapi-original.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/vendasta-marketplace-openapi-original.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vendasta/refs/heads/main/authentication/vendasta-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- SaaS
- Marketplace
- SMB
- White Label
- Reseller
- Marketing
- CRM
- Digital Agency
- Platform
---
