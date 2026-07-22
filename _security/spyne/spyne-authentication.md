---
api_key_in:
- header
- body
auth_types:
- http
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Spyne Authentication
name_suffix: Authentication
oauth_flows: []
overview: Spyne secures its APIs with http and apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Spyne
provider_slug: spyne
scheme_count: 2
schemes:
- description: 'Bearer token issued from the Spyne Console (Developer Hub > API Keys). Sent as "Authorization: Bearer <token>".'
  in: header
  name: BearerToken
  parameter: Authorization
  scheme: bearer
  source: https://docs.spyne.ai/docs/authentication
  type: http
- description: Legacy image endpoints (e.g. replace-bg) accept the API key as an auth_key body field; a 401 "Invalid Auth-key" is returned when it is missing/invalid.
  in: body
  name: AuthKey
  parameter: auth_key
  source: https://docs.spyne.ai/reference/autotransformation
  type: apiKey
slug: spyne-authentication
source_filename: spyne-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://docs.spyne.ai/docs/authentication\ndocs: https://docs.spyne.ai/docs/authentication\nsummary:\n  types: [http, apiKey]\n  api_key_in: [header, body]\n  oauth2_flows: []\n  notes: >-\n    All Spyne Unified API calls use Bearer Token authentication via the\n    Authorization header. API keys are generated in the Spyne Console under\n    Developer Hub > API Keys (\"Generate Key\"); the key is shown only once.\n    Some legacy image endpoints additionally accept the credential as an\n    auth_key request field / Auth-key.\nschemes:\n- name: BearerToken\n  type: http\n  scheme: bearer\n  in: header\n  parameter: Authorization\n  source: https://docs.spyne.ai/docs/authentication\n  description: >-\n    Bearer token issued from the Spyne Console (Developer Hub > API Keys).\n    Sent as \"Authorization: Bearer <token>\".\n- name: AuthKey\n  type: apiKey\n  in: body\n  parameter: auth_key\n  source: https://docs.spyne.ai/reference/autotransformation\n\
  \  description: >-\n    Legacy image endpoints (e.g. replace-bg) accept the API key as an auth_key\n    body field; a 401 \"Invalid Auth-key\" is returned when it is missing/invalid.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/spyne/refs/heads/main/authentication/spyne-authentication.yml
summary_line: http/apiKey · 2 schemes
tags:
- Company
- Ai
- Automotive
- Images
- Video
- Computer Vision
- Machine Learning
- Dealerships
- Media Processing
- Webhooks
---
