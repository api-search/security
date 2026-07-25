---
api_key_in: []
api_specs:
- filename: acuant-authentication-api-openapi.yml
  format: yaml
  label: Acuant Authentication API
  slug: acuant-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/acuant/refs/heads/main/openapi/acuant-authentication-api-openapi.yml
- filename: acuant-chip-data-api-openapi.yml
  format: yaml
  label: Acuant Chip Data API
  slug: acuant-chip-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/acuant/refs/heads/main/openapi/acuant-chip-data-api-openapi.yml
- filename: acuant-document-data-api-openapi.yml
  format: yaml
  label: Acuant Document Data API
  slug: acuant-document-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/acuant/refs/heads/main/openapi/acuant-document-data-api-openapi.yml
- filename: acuant-document-instances-api-openapi.yml
  format: yaml
  label: Acuant Document Instances API
  slug: acuant-document-instances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/acuant/refs/heads/main/openapi/acuant-document-instances-api-openapi.yml
- filename: acuant-face-match-api-openapi.yml
  format: yaml
  label: Acuant Face Match API
  slug: acuant-face-match-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/acuant/refs/heads/main/openapi/acuant-face-match-api-openapi.yml
- filename: acuant-images-api-openapi.yml
  format: yaml
  label: Acuant Images API
  slug: acuant-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/acuant/refs/heads/main/openapi/acuant-images-api-openapi.yml
- filename: acuant-liveness-api-openapi.yml
  format: yaml
  label: Acuant Liveness API
  slug: acuant-liveness-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/acuant/refs/heads/main/openapi/acuant-liveness-api-openapi.yml
- filename: acuant-metadata-api-openapi.yml
  format: yaml
  label: Acuant Metadata API
  slug: acuant-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/acuant/refs/heads/main/openapi/acuant-metadata-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Acuant Authentication
name_suffix: Authentication
oauth_flows: []
overview: Acuant secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Acuant
provider_slug: acuant
scheme_count: 2
schemes:
- description: HTTP Basic authentication. Credentials encoded as Base64("username:password") in the Authorization header.
  name: BasicAuth
  scheme: basic
  sources:
  - openapi/acuant-acas-openapi.yml
  - openapi/acuant-assureid-connect-openapi.yml
  - openapi/acuant-frm-openapi.yml
  - openapi/acuant-passive-liveness-openapi.yml
  type: http
- bearerFormat: JWT
  description: JWT bearer token obtained from the /api/v1/token endpoint.
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/acuant-acas-openapi.yml
  - openapi/acuant-frm-openapi.yml
  - openapi/acuant-passive-liveness-openapi.yml
  type: http
slug: acuant-authentication
source_filename: acuant-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/acuant-acas-openapi.yml, openapi/acuant-assureid-connect-openapi.yml, openapi/acuant-frm-openapi.yml,\n  openapi/acuant-passive-liveness-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BasicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic authentication. Credentials encoded as Base64(\"username:password\")\n    in the Authorization header.\n  sources:\n  - openapi/acuant-acas-openapi.yml\n  - openapi/acuant-assureid-connect-openapi.yml\n  - openapi/acuant-frm-openapi.yml\n  - openapi/acuant-passive-liveness-openapi.yml\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: JWT bearer token obtained from the /api/v1/token endpoint.\n  sources:\n  - openapi/acuant-acas-openapi.yml\n  - openapi/acuant-frm-openapi.yml\n  - openapi/acuant-passive-liveness-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/acuant/refs/heads/main/authentication/acuant-authentication.yml
summary_line: http · 2 schemes
tags:
- Identity Verification
- Document Authentication
- Biometrics
- Face Matching
- Liveness Detection
- KYC
- AML
- ID Capture
---
