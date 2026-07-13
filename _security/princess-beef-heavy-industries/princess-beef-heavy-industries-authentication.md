---
api_key_in:
- header
api_specs:
- filename: princess-beef-heavy-industries-giftshop-openapi.yml
  format: yaml
  label: Pb33f Giftshop API
  slug: giftshop-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/princess-beef-heavy-industries/refs/heads/main/openapi/princess-beef-heavy-industries-giftshop-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Princess Beef Heavy Industries Authentication
name_suffix: Authentication
oauth_flows: []
overview: Princess Beef Heavy Industries secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Princess Beef Heavy Industries
provider_slug: princess-beef-heavy-industries
scheme_count: 1
schemes:
- description: API Key authentication. Provide your API key as the value of the `X-API-Key` header.
  in: header
  name: ApiKeyAuth
  parameter: X-API-Key
  sources:
  - openapi/princess-beef-heavy-industries-giftshop-openapi.yml
  type: apiKey
slug: princess-beef-heavy-industries-authentication
source_filename: princess-beef-heavy-industries-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/princess-beef-heavy-industries-giftshop-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: API Key authentication. Provide your API key as the value of the `X-API-Key`\n    header.\n  sources:\n  - openapi/princess-beef-heavy-industries-giftshop-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/princess-beef-heavy-industries/refs/heads/main/authentication/princess-beef-heavy-industries-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Commerce
- Documentation
- Editors
- Governance
- Platform
- Products
- Rules
---
