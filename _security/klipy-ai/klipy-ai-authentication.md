---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: klipy-ai-authentication-api-openapi.yml
  format: yaml
  label: Klipy Authentication API
  slug: klipy-ai-authentication-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/klipy-ai/openapi/klipy-ai-authentication-api-openapi.yml
- filename: klipy-ai-companies-api-openapi.yml
  format: yaml
  label: Klipy Companies API
  slug: klipy-ai-companies-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/klipy-ai/openapi/klipy-ai-companies-api-openapi.yml
- filename: klipy-ai-interactions-api-openapi.yml
  format: yaml
  label: Klipy Interactions API
  slug: klipy-ai-interactions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/klipy-ai/openapi/klipy-ai-interactions-api-openapi.yml
- filename: klipy-ai-people-api-openapi.yml
  format: yaml
  label: Klipy People API
  slug: klipy-ai-people-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/klipy-ai/openapi/klipy-ai-people-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Klipy Authentication
name_suffix: Authentication
oauth_flows: []
overview: Klipy secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Klipy
provider_slug: klipy-ai
scheme_count: 2
schemes:
- description: API key passed as a header
  in: header
  name: ApiKeyHeader
  parameter: X-Klipy-Api-Key
  sources:
  - openapi/klipy-ai-openapi.json
  type: apiKey
- description: API key passed as a Bearer token in the Authorization header
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/klipy-ai-openapi.json
  type: http
slug: klipy-ai-authentication
source_filename: klipy-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-13'\nmethod: derived\nsource: openapi/klipy-ai-openapi.json\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyHeader\n  type: apiKey\n  in: header\n  parameter: X-Klipy-Api-Key\n  description: API key passed as a header\n  sources:\n  - openapi/klipy-ai-openapi.json\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: API key passed as a Bearer token in the Authorization header\n  sources:\n  - openapi/klipy-ai-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/klipy-ai/authentication/klipy-ai-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Artificial Intelligence
- Sales
- CRO
- Automation
- Software-as-a-Service
---
