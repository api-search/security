---
anonymous_access: false
api_key_in:
- cookie
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Dechonet Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: DechoNet secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: DechoNet
provider_slug: dechonet-com
scheme_count: 2
schemes:
- description: Current case session/access cookie; public keys do not grant case access.
  in: cookie
  name: caseSession
  parameter: dn_acct
  sources:
  - openapi/dechonet-com-openapi.json
  type: apiKey
- description: Key from the monitoring account page (dn_…).
  name: apiKey
  scheme: bearer
  sources:
  - openapi/dechonet-com-openapi.json
  type: http
slug: dechonet-com-authentication
source_filename: dechonet-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: derived\nsource: openapi/dechonet-com-openapi.json\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - cookie\nschemes:\n- name: caseSession\n  type: apiKey\n  in: cookie\n  parameter: dn_acct\n  description: Current case session/access cookie; public keys do not grant case access.\n  sources:\n  - openapi/dechonet-com-openapi.json\n- name: apiKey\n  type: http\n  scheme: bearer\n  description: Key from the monitoring account page (dn_…).\n  sources:\n  - openapi/dechonet-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/dechonet-com/authentication/dechonet-com-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- Security
- Monitoring
- Phishing
---
