---
api_key_in:
- header
api_specs:
- filename: homeward-offer-estimate-openapi.yml
  format: yaml
  label: Homeward Offer Estimate API
  slug: homeward-offer-estimate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/homeward/refs/heads/main/openapi/homeward-offer-estimate-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Homeward Authentication
name_suffix: Authentication
oauth_flows: []
overview: Homeward secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Homeward
provider_slug: homeward
scheme_count: 1
schemes:
- description: Token authentication. Provide the testing or production token issued by Homeward in the Authentication header. Contact api@homeward.com to obtain tokens.
  in: header
  name: tokenAuth
  parameter: Authentication
  sources:
  - openapi/homeward-offer-estimate-openapi.yml
  type: apiKey
slug: homeward-authentication
source_filename: homeward-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: openapi/homeward-offer-estimate-openapi.yml\ndocs: https://api-docs.homeward.com/\nnotes: >-\n  Homeward uses token authentication. Partners email api@homeward.com to obtain\n  testing and production tokens, supplied in the Authentication request header\n  for all authenticated endpoints. The /buybox/ endpoint is documented as\n  requiring no credential.\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: tokenAuth\n  type: apiKey\n  in: header\n  parameter: Authentication\n  description: Token authentication. Provide the testing or production token issued by Homeward\n    in the Authentication header. Contact api@homeward.com to obtain tokens.\n  sources:\n  - openapi/homeward-offer-estimate-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/homeward/refs/heads/main/authentication/homeward-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Real Estate
- Home Finance
- Mortgage
- Proptech
- Cash Offer
- Title
- Lending
---
