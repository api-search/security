---
api_key_in:
- query
api_specs:
- filename: openapi.json
  format: json
  label: The Guardian Content API
  slug: the-guardian-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/guardian/refs/heads/main/openapi/openapi.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Guardian Authentication
name_suffix: Authentication
oauth_flows: []
overview: The Guardian secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: The Guardian
provider_slug: guardian
scheme_count: 1
schemes:
- description: API key obtained from https://open-platform.theguardian.com/access/. A test key 'test' is available for development.
  in: query
  name: apiKeyQuery
  parameter: api-key
  sources:
  - openapi/openapi.json
  type: apiKey
slug: guardian-authentication
source_filename: guardian-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: apiKeyQuery\n  type: apiKey\n  in: query\n  parameter: api-key\n  description: API key obtained from https://open-platform.theguardian.com/access/. A test key\n    'test' is available for development.\n  sources:\n  - openapi/openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/guardian/refs/heads/main/authentication/guardian-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- News
- Media
- Content
- Articles
- Journalism
---
