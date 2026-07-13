---
api_key_in:
- header
api_specs:
- filename: integry-openapi.yml
  format: yaml
  label: Integry API
  slug: apis
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/integry/refs/heads/main/openapi/integry-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Integry Authentication
name_suffix: Authentication
oauth_flows: []
overview: Integry secures its APIs with apiKey across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Integry
provider_slug: integry
scheme_count: 3
schemes:
- description: Integry application key.
  in: header
  name: AppKey
  parameter: App-Key
  sources:
  - openapi/integry-openapi.yml
  type: apiKey
- description: End user identifier within the Integry workspace.
  in: header
  name: UserID
  parameter: User-ID
  sources:
  - openapi/integry-openapi.yml
  type: apiKey
- description: HMAC SHA256 hash of the User-ID using the App-Secret.
  in: header
  name: Hash
  parameter: Hash
  sources:
  - openapi/integry-openapi.yml
  type: apiKey
slug: integry-authentication
source_filename: integry-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/integry-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: AppKey\n  type: apiKey\n  in: header\n  parameter: App-Key\n  description: Integry application key.\n  sources:\n  - openapi/integry-openapi.yml\n- name: UserID\n  type: apiKey\n  in: header\n  parameter: User-ID\n  description: End user identifier within the Integry workspace.\n  sources:\n  - openapi/integry-openapi.yml\n- name: Hash\n  type: apiKey\n  in: header\n  parameter: Hash\n  description: HMAC SHA256 hash of the User-ID using the App-Secret.\n  sources:\n  - openapi/integry-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/integry/refs/heads/main/authentication/integry-authentication.yml
summary_line: apiKey · 3 schemes
tags:
- Embedded iPaaS
- Integration
- Native Integrations
---
