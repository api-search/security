---
api_key_in:
- header
api_specs:
- filename: scout-rfp-events-openapi.yml
  format: yaml
  label: Workday Strategic Sourcing API
  slug: workday-strategic-sourcing
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scout-rfp/refs/heads/main/openapi/scout-rfp-events-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Scout Rfp Authentication
name_suffix: Authentication
oauth_flows: []
overview: Scout RFP secures its APIs with apiKey across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Scout RFP
provider_slug: scout-rfp
scheme_count: 3
schemes:
- description: Company-wide API key
  in: header
  name: ApiKeyAuth
  parameter: X-Api-Key
  sources:
  - openapi/scout-rfp-events-openapi.yml
  type: apiKey
- description: User-specific API token
  in: header
  name: UserTokenAuth
  parameter: X-User-Token
  sources:
  - openapi/scout-rfp-events-openapi.yml
  type: apiKey
- description: User email address
  in: header
  name: UserEmailAuth
  parameter: X-User-Email
  sources:
  - openapi/scout-rfp-events-openapi.yml
  type: apiKey
slug: scout-rfp-authentication
source_filename: scout-rfp-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/scout-rfp-events-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-Api-Key\n  description: Company-wide API key\n  sources:\n  - openapi/scout-rfp-events-openapi.yml\n- name: UserTokenAuth\n  type: apiKey\n  in: header\n  parameter: X-User-Token\n  description: User-specific API token\n  sources:\n  - openapi/scout-rfp-events-openapi.yml\n- name: UserEmailAuth\n  type: apiKey\n  in: header\n  parameter: X-User-Email\n  description: User email address\n  sources:\n  - openapi/scout-rfp-events-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/scout-rfp/refs/heads/main/authentication/scout-rfp-authentication.yml
summary_line: apiKey · 3 schemes
tags:
- Procurement
- Sourcing
- RFP
- Supply Chain
- Workday
---
