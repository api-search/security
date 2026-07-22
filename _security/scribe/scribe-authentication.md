---
api_key_in:
- header
api_specs:
- filename: scribe-search-retrieval-openapi.yml
  format: yaml
  label: Scribe Search & Retrieval API
  slug: scribe-search-retrieval-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scribe/refs/heads/main/openapi/scribe-search-retrieval-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Scribe Authentication
name_suffix: Authentication
oauth_flows: []
overview: Scribe secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Scribe
provider_slug: scribe
scheme_count: 1
schemes:
- description: 'API key authentication. Add your API key as the header value. Example: `X-API-Key: sc_1234567890abcdefg.hijklmnopqrstuvwx`'
  in: header
  name: APIKey
  parameter: X-API-Key
  sources:
  - openapi/scribe-search-retrieval-openapi.yml
  type: apiKey
slug: scribe-authentication
source_filename: scribe-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/scribe-search-retrieval-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: APIKey\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: 'API key authentication. Add your API key as the header value. Example: `X-API-Key:\n    sc_1234567890abcdefg.hijklmnopqrstuvwx`'\n  sources:\n  - openapi/scribe-search-retrieval-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/scribe/refs/heads/main/authentication/scribe-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Ai Ml
- Documentation
- Knowledge Management
- Search
- Workflow
- Process Documentation
- Enterprise
---
