---
api_key_in: []
api_specs:
- filename: brellium-audits-api-openapi.yml
  format: yaml
  label: Brellium Audits API
  slug: brellium-audits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brellium/refs/heads/main/openapi/brellium-audits-api-openapi.yml
- filename: brellium-auth-api-openapi.yml
  format: yaml
  label: Brellium Auth API
  slug: brellium-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brellium/refs/heads/main/openapi/brellium-auth-api-openapi.yml
- filename: brellium-coding-api-openapi.yml
  format: yaml
  label: Brellium Coding API
  slug: brellium-coding-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brellium/refs/heads/main/openapi/brellium-coding-api-openapi.yml
- filename: brellium-documents-api-openapi.yml
  format: yaml
  label: Brellium Documents API
  slug: brellium-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brellium/refs/heads/main/openapi/brellium-documents-api-openapi.yml
- filename: brellium-documents-multiple-api-openapi.yml
  format: yaml
  label: Brellium Documents Multiple API
  slug: brellium-documents-multiple-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brellium/refs/heads/main/openapi/brellium-documents-multiple-api-openapi.yml
- filename: brellium-link-providers-api-openapi.yml
  format: yaml
  label: Brellium Link Providers API
  slug: brellium-link-providers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brellium/refs/heads/main/openapi/brellium-link-providers-api-openapi.yml
- filename: brellium-question-sets-api-openapi.yml
  format: yaml
  label: Brellium Question Sets API
  slug: brellium-question-sets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brellium/refs/heads/main/openapi/brellium-question-sets-api-openapi.yml
- filename: brellium-update-audits-flags-api-openapi.yml
  format: yaml
  label: Brellium Update Audits Flags API
  slug: brellium-update-audits-flags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brellium/refs/heads/main/openapi/brellium-update-audits-flags-api-openapi.yml
- filename: brellium-users-api-openapi.yml
  format: yaml
  label: Brellium Users API
  slug: brellium-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brellium/refs/heads/main/openapi/brellium-users-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Brellium Authentication
name_suffix: Authentication
oauth_flows: []
overview: Brellium secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Brellium
provider_slug: brellium
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/brellium-openapi-original.json
  type: http
slug: brellium-authentication
source_filename: brellium-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: derived\nsource: openapi/brellium-openapi-original.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/brellium-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/brellium/refs/heads/main/authentication/brellium-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Healthcare
- Clinical Compliance
- Clinical Documentation
- Medical Coding
- Audit
- Behavioral Health
- Digital Health
---
