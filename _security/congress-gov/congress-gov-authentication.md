---
api_key_in:
- query
api_specs:
- filename: openapi.yaml
  format: yaml
  label: Congress.gov API v3
  slug: congressgov-api-v3
  spec_type: OpenAPI
  url: https://api.congress.gov/
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Congress Gov Authentication
name_suffix: Authentication
oauth_flows: []
overview: Congress.gov API secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Congress.gov API
provider_slug: congress-gov
scheme_count: 1
schemes:
- in: query
  name: ApiKeyAuth
  parameter: api_key
  sources:
  - openapi/congress-gov-openapi.yml
  type: apiKey
slug: congress-gov-authentication
source_filename: congress-gov-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/congress-gov-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: query\n  parameter: api_key\n  sources:\n  - openapi/congress-gov-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/congress-gov/refs/heads/main/authentication/congress-gov-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Government
- Legislative
- Congress
- Bills
- Amendments
- Members
- Treaties
- Nominations
- Congressional Record
- US Federal
---
