---
api_key_in:
- header
api_specs:
- filename: enviance-restapi-openapi-original.json
  format: json
  label: Cority Enviance EMS REST API
  slug: enviance-ems-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/enviance/refs/heads/main/openapi/enviance-restapi-openapi-original.json
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Enviance Authentication
name_suffix: Authentication
oauth_flows: []
overview: Enviance secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Enviance
provider_slug: enviance
scheme_count: 2
schemes:
- description: Forces authentication with credentials via an api gateway
  name: Basic
  scheme: basic
  sources:
  - openapi/enviance-restapi-openapi-original.json
  type: http
- description: "**Enviance \\<SessionId\\>**. \r\n\t\t\t\t\t  Obtain SessionId by POST /ver2/AuthenticationService.svc/sessions first"
  in: header
  name: EnvianceAuth
  parameter: Authorization
  sources:
  - openapi/enviance-restapi-openapi-original.json
  type: apiKey
slug: enviance-authentication
source_filename: enviance-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: derived\nsource: openapi/enviance-restapi-openapi-original.json\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: Basic\n  type: http\n  scheme: basic\n  description: Forces authentication with credentials via an api gateway\n  sources:\n  - openapi/enviance-restapi-openapi-original.json\n- name: EnvianceAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: \"**Enviance \\\\<SessionId\\\\>**. \\r\\n\\t\\t\\t\\t\\t  Obtain SessionId by POST /ver2/AuthenticationService.svc/sessions\\\n    \\ first\"\n  sources:\n  - openapi/enviance-restapi-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/enviance/refs/heads/main/authentication/enviance-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- Environmental
- Compliance
- EHS
- Sustainability
- Chemical Management
- Regulatory
- SaaS
---
