---
api_key_in: []
api_specs:
- filename: stannp-account-api-openapi.yml
  format: yaml
  label: Stannp Account API
  slug: stannp-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stannp/refs/heads/main/openapi/stannp-account-api-openapi.yml
- filename: stannp-campaigns-api-openapi.yml
  format: yaml
  label: Stannp Campaigns API
  slug: stannp-campaigns-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stannp/refs/heads/main/openapi/stannp-campaigns-api-openapi.yml
- filename: stannp-events-api-openapi.yml
  format: yaml
  label: Stannp Events API
  slug: stannp-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stannp/refs/heads/main/openapi/stannp-events-api-openapi.yml
- filename: stannp-groups-api-openapi.yml
  format: yaml
  label: Stannp Groups API
  slug: stannp-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stannp/refs/heads/main/openapi/stannp-groups-api-openapi.yml
- filename: stannp-letters-api-openapi.yml
  format: yaml
  label: Stannp Letters API
  slug: stannp-letters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stannp/refs/heads/main/openapi/stannp-letters-api-openapi.yml
- filename: stannp-postcards-api-openapi.yml
  format: yaml
  label: Stannp Postcards API
  slug: stannp-postcards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stannp/refs/heads/main/openapi/stannp-postcards-api-openapi.yml
- filename: stannp-recipients-api-openapi.yml
  format: yaml
  label: Stannp Recipients API
  slug: stannp-recipients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/stannp/refs/heads/main/openapi/stannp-recipients-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Stannp Authentication
name_suffix: Authentication
oauth_flows: []
overview: Stannp secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Stannp
provider_slug: stannp
scheme_count: 1
schemes:
- description: Use your API key as the username and leave the password blank.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/stannp-direct-mail-api-openapi.yml
  type: http
slug: stannp-authentication
source_filename: stannp-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/stannp-direct-mail-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: Use your API key as the username and leave the password blank.\n  sources:\n  - openapi/stannp-direct-mail-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/stannp/refs/heads/main/authentication/stannp-authentication.yml
summary_line: http · 1 scheme
tags:
- Direct Mail
- Postcards
- Letters
- Print
- Physical Mail
- Marketing Automation
- Campaigns
---
