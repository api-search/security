---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: bezal-ai-businesses-api-openapi.yml
  format: yaml
  label: Bezal Businesses API
  slug: bezal-ai-businesses-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bezal-ai/openapi/bezal-ai-businesses-api-openapi.yml
- filename: bezal-ai-categories-api-openapi.yml
  format: yaml
  label: Bezal Categories API
  slug: bezal-ai-categories-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bezal-ai/openapi/bezal-ai-categories-api-openapi.yml
- filename: bezal-ai-health-api-openapi.yml
  format: yaml
  label: Bezal Health API
  slug: bezal-ai-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bezal-ai/openapi/bezal-ai-health-api-openapi.yml
- filename: bezal-ai-requests-api-openapi.yml
  format: yaml
  label: Bezal Requests API
  slug: bezal-ai-requests-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bezal-ai/openapi/bezal-ai-requests-api-openapi.yml
- filename: bezal-ai-open-api-api-openapi.yml
  format: yaml
  label: Bezal Open API
  slug: bezal-ai-open-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bezal-ai/openapi/bezal-ai-open-api-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Bezal Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Bezal secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Bezal
provider_slug: bezal-ai
scheme_count: 2
schemes:
- bearerFormat: bzl_...
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/bezal-ai-openapi.yaml
  type: http
- in: header
  name: apiKeyHeader
  parameter: X-API-Key
  sources:
  - openapi/bezal-ai-openapi.yaml
  type: apiKey
slug: bezal-ai-authentication
source_filename: bezal-ai-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: derived\nsource: openapi/bezal-ai-openapi.yaml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: bzl_...\n  sources:\n  - openapi/bezal-ai-openapi.yaml\n- name: apiKeyHeader\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  sources:\n  - openapi/bezal-ai-openapi.yaml\n"
source_yaml_url: https://artifacts.apis.io/bezal-ai/authentication/bezal-ai-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- Artificial Intelligence
- Software-as-a-Service
- Local Business
- Lead Generation
- Automation
---
