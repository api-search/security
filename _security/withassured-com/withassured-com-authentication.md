---
anonymous_access: false
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Withassured Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: Assured secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Assured
provider_slug: withassured-com
scheme_count: 1
schemes:
- in: header
  name: apiKeyAuth
  parameter: x-api-key
  sources:
  - openapi/withassured-com-openapi.json
  type: apiKey
slug: withassured-com-authentication
source_filename: withassured-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-26'\nmethod: derived\nsource: openapi/withassured-com-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  sources:\n  - openapi/withassured-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/withassured-com/authentication/withassured-com-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Healthcare
- Credentialing
- AI
- Platform
---
