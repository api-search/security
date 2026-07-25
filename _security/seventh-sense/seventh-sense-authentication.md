---
api_key_in:
- header
api_specs:
- filename: seventh-sense-collections-api-openapi.yml
  format: yaml
  label: Seventh Sense Collections API
  slug: seventh-sense-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/seventh-sense/refs/heads/main/openapi/seventh-sense-collections-api-openapi.yml
- filename: seventh-sense-face-anti-spoofing-liveness-api-openapi.yml
  format: yaml
  label: Seventh Sense Face Anti-Spoofing / Liveness API
  slug: seventh-sense-face-anti-spoofing-liveness-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/seventh-sense/refs/heads/main/openapi/seventh-sense-face-anti-spoofing-liveness-api-openapi.yml
- filename: seventh-sense-face-verification-api-openapi.yml
  format: yaml
  label: Seventh Sense Face Verification API
  slug: seventh-sense-face-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/seventh-sense/refs/heads/main/openapi/seventh-sense-face-verification-api-openapi.yml
- filename: seventh-sense-persons-api-openapi.yml
  format: yaml
  label: Seventh Sense Persons API
  slug: seventh-sense-persons-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/seventh-sense/refs/heads/main/openapi/seventh-sense-persons-api-openapi.yml
- filename: seventh-sense-search-api-openapi.yml
  format: yaml
  label: Seventh Sense Search API
  slug: seventh-sense-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/seventh-sense/refs/heads/main/openapi/seventh-sense-search-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Seventh Sense Authentication
name_suffix: Authentication
oauth_flows: []
overview: Seventh Sense secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Seventh Sense
provider_slug: seventh-sense
scheme_count: 1
schemes:
- in: header
  name: APIKeyHeader
  parameter: x-api-key
  sources:
  - openapi/seventh-sense-opencv-fr-openapi.json
  type: apiKey
slug: seventh-sense-authentication
source_filename: seventh-sense-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/seventh-sense-opencv-fr-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: APIKeyHeader\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  sources:\n  - openapi/seventh-sense-opencv-fr-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/seventh-sense/refs/heads/main/authentication/seventh-sense-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Face Recognition
- Biometrics
- Identity Verification
- Liveness Detection
- Artificial Intelligence
- Computer Vision
- Security
---
