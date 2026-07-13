---
api_key_in:
- header
api_specs:
- filename: jumpcloud-openapi.yml
  format: yaml
  label: JumpCloud API V1
  slug: v1-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/jumpcloud/refs/heads/main/openapi/jumpcloud-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Jumpcloud Authentication
name_suffix: Authentication
oauth_flows: []
overview: JumpCloud secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: JumpCloud
provider_slug: jumpcloud
scheme_count: 1
schemes:
- description: JumpCloud API key from the Admin Console > API Settings.
  in: header
  name: ApiKeyAuth
  parameter: x-api-key
  sources:
  - openapi/jumpcloud-openapi.yml
  type: apiKey
slug: jumpcloud-authentication
source_filename: jumpcloud-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/jumpcloud-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: JumpCloud API key from the Admin Console > API Settings.\n  sources:\n  - openapi/jumpcloud-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/jumpcloud/refs/heads/main/authentication/jumpcloud-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Identity
- Directory Services
- SSO
- MFA
- Device Management
- MDM
- IT Operations
- Zero Trust
---
