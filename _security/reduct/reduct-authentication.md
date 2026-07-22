---
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Reduct Authentication
name_suffix: Authentication
oauth_flows: []
overview: Reduct secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Reduct
provider_slug: reduct
scheme_count: 1
schemes:
- description: Per-workspace API key created via the backstage interface. Presented on API requests to authenticate. Available on Professional and Enterprise plans.
  in: header
  name: apiKey
  sources:
  - https://help.reduct.video/en/articles/api-access
  type: apiKey
slug: reduct-authentication
source_filename: reduct-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://help.reduct.video/en/articles/api-access\ndocs: https://help.reduct.video/en/articles/api-access\nsummary:\n  types: [apiKey]\n  api_key_in: [header]\n  oauth2_flows: []\n  notes: >-\n    Reduct exposes a RESTful API (current version 3) providing broad access\n    across a workspace. Access is limited to workspaces on the Professional or\n    Enterprise plan. Authentication is by API key: keys are generated and\n    managed by an authenticated user through the Reduct \"backstage\" interface;\n    the full API reference is available only after logging in, so the exact\n    header name and key format are not published on the public docs surface.\nschemes:\n- name: apiKey\n  type: apiKey\n  in: header\n  description: >-\n    Per-workspace API key created via the backstage interface. Presented on API\n    requests to authenticate. Available on Professional and Enterprise plans.\n  sources: [https://help.reduct.video/en/articles/api-access]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/reduct/refs/heads/main/authentication/reduct-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Applications
- Video
- Transcription
- Translation
- Redaction
- Video Editing
- Media
- Artificial Intelligence
---
