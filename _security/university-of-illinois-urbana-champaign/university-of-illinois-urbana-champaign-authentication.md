---
api_key_in: []
api_specs:
- filename: university-of-illinois-urbana-champaign-admin-api-openapi.yml
  format: yaml
  label: University of Illinois Urbana-Champaign Admin API
  slug: university-of-illinois-urbana-champaign-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-illinois-urbana-champaign/refs/heads/main/openapi/university-of-illinois-urbana-champaign-admin-api-openapi.yml
- filename: university-of-illinois-urbana-champaign-bbs-api-openapi.yml
  format: yaml
  label: University of Illinois Urbana-Champaign BBs API
  slug: university-of-illinois-urbana-champaign-bbs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-illinois-urbana-champaign/refs/heads/main/openapi/university-of-illinois-urbana-champaign-bbs-api-openapi.yml
- filename: university-of-illinois-urbana-champaign-client-api-openapi.yml
  format: yaml
  label: University of Illinois Urbana-Champaign Client API
  slug: university-of-illinois-urbana-champaign-client-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-illinois-urbana-champaign/refs/heads/main/openapi/university-of-illinois-urbana-champaign-client-api-openapi.yml
- filename: university-of-illinois-urbana-champaign-default-api-openapi.yml
  format: yaml
  label: University of Illinois Urbana-Champaign Default API
  slug: university-of-illinois-urbana-champaign-default-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-illinois-urbana-champaign/refs/heads/main/openapi/university-of-illinois-urbana-champaign-default-api-openapi.yml
- filename: university-of-illinois-urbana-champaign-enc-api-openapi.yml
  format: yaml
  label: University of Illinois Urbana-Champaign Enc API
  slug: university-of-illinois-urbana-champaign-enc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-illinois-urbana-champaign/refs/heads/main/openapi/university-of-illinois-urbana-champaign-enc-api-openapi.yml
- filename: university-of-illinois-urbana-champaign-services-api-openapi.yml
  format: yaml
  label: University of Illinois Urbana-Champaign Services API
  slug: university-of-illinois-urbana-champaign-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-illinois-urbana-champaign/refs/heads/main/openapi/university-of-illinois-urbana-champaign-services-api-openapi.yml
- filename: university-of-illinois-urbana-champaign-system-api-openapi.yml
  format: yaml
  label: University of Illinois Urbana-Champaign System API
  slug: university-of-illinois-urbana-champaign-system-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-illinois-urbana-champaign/refs/heads/main/openapi/university-of-illinois-urbana-champaign-system-api-openapi.yml
- filename: university-of-illinois-urbana-champaign-third-party-services-api-openapi.yml
  format: yaml
  label: University of Illinois Urbana-Champaign Third-Party Services API
  slug: university-of-illinois-urbana-champaign-third-party-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-illinois-urbana-champaign/refs/heads/main/openapi/university-of-illinois-urbana-champaign-third-party-services-api-openapi.yml
- filename: university-of-illinois-urbana-champaign-tps-api-openapi.yml
  format: yaml
  label: University of Illinois Urbana-Champaign TPS API
  slug: university-of-illinois-urbana-champaign-tps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-illinois-urbana-champaign/refs/heads/main/openapi/university-of-illinois-urbana-champaign-tps-api-openapi.yml
- filename: university-of-illinois-urbana-champaign-ui-api-openapi.yml
  format: yaml
  label: University of Illinois Urbana-Champaign UI API
  slug: university-of-illinois-urbana-champaign-ui-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-illinois-urbana-champaign/refs/heads/main/openapi/university-of-illinois-urbana-champaign-ui-api-openapi.yml
- filename: university-of-illinois-urbana-champaign-version-api-openapi.yml
  format: yaml
  label: University of Illinois Urbana-Champaign Version API
  slug: university-of-illinois-urbana-champaign-version-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-illinois-urbana-champaign/refs/heads/main/openapi/university-of-illinois-urbana-champaign-version-api-openapi.yml
- filename: university-of-illinois-urbana-champaign-well-known-api-openapi.yml
  format: yaml
  label: University of Illinois Urbana-Champaign .well Known API
  slug: university-of-illinois-urbana-champaign-well-known-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-illinois-urbana-champaign/refs/heads/main/openapi/university-of-illinois-urbana-champaign-well-known-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: University Of Illinois Urbana Champaign Authentication
name_suffix: Authentication
oauth_flows: []
overview: University of Illinois Urbana-Champaign secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: University of Illinois Urbana-Champaign
provider_slug: university-of-illinois-urbana-champaign
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/university-of-illinois-urbana-champaign-rokwire-core.yaml
  - openapi/university-of-illinois-urbana-champaign-rokwire-gateway.yaml
  type: http
slug: university-of-illinois-urbana-champaign-authentication
source_filename: university-of-illinois-urbana-champaign-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/university-of-illinois-urbana-champaign-rokwire-core.yaml, openapi/university-of-illinois-urbana-champaign-rokwire-gateway.yaml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/university-of-illinois-urbana-champaign-rokwire-core.yaml\n  - openapi/university-of-illinois-urbana-champaign-rokwire-gateway.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/university-of-illinois-urbana-champaign/refs/heads/main/authentication/university-of-illinois-urbana-champaign-authentication.yml
summary_line: http · 1 scheme
tags:
- Education
- Higher Education
- University
- Open Data
- Courses
- Library
- United States
---
