---
api_key_in: []
api_specs:
- filename: kagi-openapi.yml
  format: yaml
  label: Kagi Search API
  slug: search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kagi/refs/heads/main/openapi/kagi-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Kagi Authentication
name_suffix: Authentication
oauth_flows: []
overview: Kagi secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Kagi
provider_slug: kagi
scheme_count: 1
schemes:
- description: Kagi API token issued from https://kagi.com/api/keys, sent in the Authorization header as "Bearer <token>" (or the equivalent "Bot <token>" form documented for the legacy Search endpoint).
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/kagi-openapi.yml
  type: http
slug: kagi-authentication
source_filename: kagi-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/kagi-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Kagi API token issued from https://kagi.com/api/keys, sent in the Authorization\n    header as \"Bearer <token>\" (or the equivalent \"Bot <token>\" form documented for the legacy\n    Search endpoint).\n  sources:\n  - openapi/kagi-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kagi/refs/heads/main/authentication/kagi-authentication.yml
summary_line: http · 1 scheme
tags:
- Search
- Premium Search
- AI Search
- Summarization
- FastGPT
- Enrichment
- OpenAPI
- Pay-Per-Use
- Privacy
- LLMs
- Web Index
---
