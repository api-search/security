---
api_key_in: []
api_specs:
- filename: openapi.yaml
  format: yaml
  label: Acquia DAM API v2
  slug: acquia-dam-api-v2
  spec_type: OpenAPI
  url: https://widenv2.docs.apiary.io/
- filename: openapi.yaml
  format: yaml
  label: Acquia DAM API v1
  slug: acquia-dam-api-v1
  spec_type: OpenAPI
  url: https://widenv1.docs.apiary.io/
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Widen Authentication
name_suffix: Authentication
oauth_flows: []
overview: Widen secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Widen
provider_slug: widen
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: OAuth2 Bearer token obtained from Acquia DAM.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/openapi.yml
  type: http
slug: widen-authentication
source_filename: widen-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: OAuth2 Bearer token obtained from Acquia DAM.\n  sources:\n  - openapi/openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/widen/refs/heads/main/authentication/widen-authentication.yml
summary_line: http · 1 scheme
tags:
- Digital Asset Management
- DAM
- Media
- Assets
- Metadata
- Collections
- Workflows
- Acquia
---
