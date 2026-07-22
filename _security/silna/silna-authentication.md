---
api_key_in: []
api_specs:
- filename: silna-openapi.json
  format: json
  label: Silna Public API
  slug: silna-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/silna/refs/heads/main/openapi/silna-openapi.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Silna Authentication
name_suffix: Authentication
oauth_flows: []
overview: Silna secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Silna
provider_slug: silna
scheme_count: 1
schemes:
- header: Authorization
  in: header
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/silna-openapi.json
  - https://docs.silnahealth.com/api-reference/overview
  token_issuance: https://app.silnahealth.com/ - create a token associated with your provider or MSO
  type: http
slug: silna-authentication
source_filename: silna-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://docs.silnahealth.com/api-reference/overview\ndocs: https://docs.silnahealth.com/api-reference/overview\nsummary:\n  types:\n  - http\n  notes: >-\n    All Silna Public API endpoints are authenticated with Bearer tokens passed in\n    the Authorization header. Tokens are generated in the Silna Portal\n    (https://app.silnahealth.com/) and associated with a provider or MSO.\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  in: header\n  header: Authorization\n  token_issuance: 'https://app.silnahealth.com/ - create a token associated with your provider or MSO'\n  sources:\n  - openapi/silna-openapi.json\n  - https://docs.silnahealth.com/api-reference/overview\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/silna/refs/heads/main/authentication/silna-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Automation
- Healthcare
- Prior Authorization
- Benefits Check
- Eligibility
- Insurance
- Revenue Cycle
- API
---
