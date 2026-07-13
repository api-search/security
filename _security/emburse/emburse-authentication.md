---
api_key_in:
- header
api_specs:
- filename: emburse-virtual-cards-openapi.yml
  format: yaml
  label: Emburse Virtual Cards API
  slug: emburse-virtual-cards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/emburse/refs/heads/main/openapi/emburse-virtual-cards-openapi.yml
- filename: emburse-enterprise-allocation-openapi.yml
  format: yaml
  label: Emburse Enterprise REST APIs
  slug: emburse-enterprise-rest-apis
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/emburse/refs/heads/main/openapi/emburse-enterprise-allocation-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Emburse Authentication
name_suffix: Authentication
oauth_flows: []
overview: Emburse secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Emburse
provider_slug: emburse
scheme_count: 2
schemes:
- description: API key for Authentication
  in: header
  name: x-api-key
  parameter: x-api-key
  sources:
  - openapi/emburse-enterprise-expense-image-openapi.yml
  type: apiKey
- description: 'OAuth2 access token. Include in Authorization header: `Authorization: Bearer YOUR_ACCESS_TOKEN`'
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/emburse-virtual-cards-openapi.yml
  type: http
slug: emburse-authentication
source_filename: emburse-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/emburse-enterprise-expense-image-openapi.yml, openapi/emburse-virtual-cards-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: x-api-key\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: API key for Authentication\n  sources:\n  - openapi/emburse-enterprise-expense-image-openapi.yml\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: 'OAuth2 access token. Include in Authorization header: `Authorization: Bearer\n    YOUR_ACCESS_TOKEN`'\n  sources:\n  - openapi/emburse-virtual-cards-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/emburse/refs/heads/main/authentication/emburse-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Expense Management
- AP Automation
- Corporate Cards
- Virtual Cards
- Receipt Capture
- Reimbursement
- Invoice Processing
- Finance
- FinTech
---
