---
anonymous_access: false
api_key_in:
- header
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: AI Audit Exchange (Ingenious AI) Authentication
name_suffix: Authentication
oauth_flows: []
overview: AI Audit Exchange (Ingenious AI) secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: AI Audit Exchange (Ingenious AI)
provider_slug: auditexchange-getingeniousai-com
scheme_count: 2
schemes:
- in: header
  name: ApiKeyAuth
  parameter: X-API-Key
  sources:
  - openapi/auditexchange-getingeniousai-com-admt-openapi.json
  - openapi/auditexchange-getingeniousai-com-openapi.json
  type: apiKey
- name: BearerAuth
  scheme: bearer
  sources:
  - openapi/auditexchange-getingeniousai-com-openapi.json
  type: http
slug: auditexchange-getingeniousai-com-authentication
source_filename: auditexchange-getingeniousai-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-17'\nmethod: derived\nsource: openapi/auditexchange-getingeniousai-com-admt-openapi.json, openapi/auditexchange-getingeniousai-com-openapi.json\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  sources:\n  - openapi/auditexchange-getingeniousai-com-admt-openapi.json\n  - openapi/auditexchange-getingeniousai-com-openapi.json\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/auditexchange-getingeniousai-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/auditexchange-getingeniousai-com/authentication/auditexchange-getingeniousai-com-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- Artificial Intelligence
- Audit
- Platform
- California
---
