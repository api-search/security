---
api_key_in: []
api_specs:
- filename: united-technologies-arinc-messaging-openapi.yml
  format: yaml
  label: Collins Aerospace ARINC Messaging API
  slug: arinc-messaging-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/united-technologies/refs/heads/main/openapi/united-technologies-arinc-messaging-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: United Technologies Authentication
name_suffix: Authentication
oauth_flows: []
overview: United Technologies secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: United Technologies
provider_slug: united-technologies
scheme_count: 1
schemes:
- description: Bearer token for ARINC Online API authentication.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/united-technologies-arinc-messaging-openapi.yml
  type: http
slug: united-technologies-authentication
source_filename: united-technologies-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/united-technologies-arinc-messaging-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Bearer token for ARINC Online API authentication.\n  sources:\n  - openapi/united-technologies-arinc-messaging-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/united-technologies/refs/heads/main/authentication/united-technologies-authentication.yml
summary_line: http · 1 scheme
tags:
- Aerospace
- Defense
- Aviation
- Manufacturing
- Connectivity
- Fortune 100
---
