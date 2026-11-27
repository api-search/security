---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: uservane-com-privacy-api-openapi.yml
  format: yaml
  label: UserVane Privacy API
  slug: uservane-com-privacy-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/uservane-com/openapi/uservane-com-privacy-api-openapi.yml
- filename: uservane-com-public-sdk-api-openapi.yml
  format: yaml
  label: UserVane Public SDK API
  slug: uservane-com-public-sdk-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/uservane-com/openapi/uservane-com-public-sdk-api-openapi.yml
- filename: uservane-com-secret-sdk-api-openapi.yml
  format: yaml
  label: UserVane Secret SDK API
  slug: uservane-com-secret-sdk-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/uservane-com/openapi/uservane-com-secret-sdk-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: UserVane Authentication
name_suffix: Authentication
oauth_flows: []
overview: UserVane secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: UserVane
provider_slug: uservane-com
scheme_count: 2
schemes:
- description: Project secret key (`uv_sk_...`). Server-only.
  name: SecretKeyBearer
  scheme: bearer
  sources:
  - openapi/uservane-com-openapi.yaml
  type: http
- description: Alternate secret key header. Server-only.
  in: header
  name: SecretKeyHeader
  parameter: X-UserVane-Key
  sources:
  - openapi/uservane-com-openapi.yaml
  type: apiKey
slug: uservane-com-authentication
source_filename: uservane-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-27'\nmethod: derived\nsource: openapi/uservane-com-openapi.yaml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: SecretKeyBearer\n  type: http\n  scheme: bearer\n  description: Project secret key (`uv_sk_...`). Server-only.\n  sources:\n  - openapi/uservane-com-openapi.yaml\n- name: SecretKeyHeader\n  type: apiKey\n  in: header\n  parameter: X-UserVane-Key\n  description: Alternate secret key header. Server-only.\n  sources:\n  - openapi/uservane-com-openapi.yaml\n"
source_yaml_url: https://artifacts.apis.io/uservane-com/authentication/uservane-com-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- SaaS
- Survey
- AI
- CustomerFeedback
---
