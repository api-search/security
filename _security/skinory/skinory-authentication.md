---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: skinory-inventories-api-openapi.yml
  format: yaml
  label: Skinory (submitted as g2push) Inventories API
  slug: skinory-inventories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/skinory/refs/heads/main/openapi/skinory-inventories-api-openapi.yml
- filename: skinory-inventory-api-openapi.yml
  format: yaml
  label: Skinory (submitted as g2push) Inventory API
  slug: skinory-inventory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/skinory/refs/heads/main/openapi/skinory-inventory-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Skinory Authentication
name_suffix: Authentication
oauth_flows: []
overview: Skinory (submitted as g2push) secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Skinory (submitted as g2push)
provider_slug: skinory
scheme_count: 2
schemes:
- description: 'API key in Authorization: Bearer <key>. Optional; without a key the request is anonymous and keeps the per-address limits. Create a key at https://skinory.io/en/profile after signing in through Steam (the account has to be a day old, up to 3 keys per account). A key has its own limits instead of the address ones: 600 requests per minute, 300 appraisals per hour, 30 lookups per minute of profiles n'
  name: bearerKey
  scheme: bearer
  sources:
  - openapi/skinory-openapi.json
  type: http
- description: 'API key in the X-Api-Key header. Optional; without a key the request is anonymous and keeps the per-address limits. Create a key at https://skinory.io/en/profile after signing in through Steam (the account has to be a day old, up to 3 keys per account). A key has its own limits instead of the address ones: 600 requests per minute, 300 appraisals per hour, 30 lookups per minute of profiles never ap'
  in: header
  name: headerKey
  parameter: X-Api-Key
  sources:
  - openapi/skinory-openapi.json
  type: apiKey
slug: skinory-authentication
source_filename: skinory-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-28'\nmethod: derived\nsource: openapi/skinory-openapi.json\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: bearerKey\n  type: http\n  scheme: bearer\n  description: 'API key in Authorization: Bearer <key>. Optional; without a key the request\n    is anonymous and keeps the per-address limits. Create a key at https://skinory.io/en/profile\n    after signing in through Steam (the account has to be a day old, up to 3 keys per account).\n    A key has its own limits instead of the address ones: 600 requests per minute, 300 appraisals\n    per hour, 30 lookups per minute of profiles n'\n  sources:\n  - openapi/skinory-openapi.json\n- name: headerKey\n  type: apiKey\n  in: header\n  parameter: X-Api-Key\n  description: 'API key in the X-Api-Key header. Optional; without a key the request is anonymous\n    and keeps the per-address limits. Create a key at https://skinory.io/en/profile after signing\n    in through Steam (the\
  \ account has to be a day old, up to 3 keys per account). A key has\n    its own limits instead of the address ones: 600 requests per minute, 300 appraisals per\n    hour, 30 lookups per minute of profiles never ap'\n  sources:\n  - openapi/skinory-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/skinory/refs/heads/main/authentication/skinory-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- Gaming
- Skins
- CS2
- CS:GO
- API
---
