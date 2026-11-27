---
anonymous_access: false
api_key_in: []
api_specs:
- filename: founden-ai-founden-api-openapi.yml
  format: yaml
  label: Founden Founden API
  slug: founden-ai-founden-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/founden-ai/openapi/founden-ai-founden-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Founden Authentication
name_suffix: Authentication
oauth_flows: []
overview: Founden secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Founden
provider_slug: founden-ai
scheme_count: 1
schemes:
- bearerFormat: omk_ API key
  description: 'Your API key, sent as ''Authorization: Bearer omk_...''. The same key works across every product.'
  name: apiKey
  scheme: bearer
  sources:
  - openapi/founden-ai-openapi.json
  type: http
slug: founden-ai-authentication
source_filename: founden-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-17'\nmethod: derived\nsource: openapi/founden-ai-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: apiKey\n  type: http\n  scheme: bearer\n  bearerFormat: omk_ API key\n  description: 'Your API key, sent as ''Authorization: Bearer omk_...''. The same key works\n    across every product.'\n  sources:\n  - openapi/founden-ai-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/founden-ai/authentication/founden-ai-authentication.yml
summary_line: http · 1 scheme
tags:
- Artificial Intelligence
- Automation
- Platform
- Software-as-a-Service
- Company
---
