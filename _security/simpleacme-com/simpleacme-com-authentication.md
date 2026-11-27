---
anonymous_access: false
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: SimpleACME Authentication
name_suffix: Authentication
oauth_flows: []
overview: SimpleACME secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: SimpleACME
provider_slug: simpleacme-com
scheme_count: 2
schemes:
- in: header
  name: AcmeUser
  parameter: X-Api-User
  sources:
  - openapi/simpleacme-com-openapi.json
  type: apiKey
- in: header
  name: AcmeKey
  parameter: X-Api-Key
  sources:
  - openapi/simpleacme-com-openapi.json
  type: apiKey
slug: simpleacme-com-authentication
source_filename: simpleacme-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-12'\nmethod: derived\nsource: openapi/simpleacme-com-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: AcmeUser\n  type: apiKey\n  in: header\n  parameter: X-Api-User\n  sources:\n  - openapi/simpleacme-com-openapi.json\n- name: AcmeKey\n  type: apiKey\n  in: header\n  parameter: X-Api-Key\n  sources:\n  - openapi/simpleacme-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/simpleacme-com/authentication/simpleacme-com-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Certificates
- DNS‑01
- Wildcard
- ACME
- Integration
---
