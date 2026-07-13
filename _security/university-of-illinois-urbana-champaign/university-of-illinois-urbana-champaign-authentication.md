---
api_key_in: []
api_specs:
- filename: university-of-illinois-urbana-champaign-rokwire-core.yaml
  format: yaml
  label: Rokwire Core Building Block
  slug: rokwire-core
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-illinois-urbana-champaign/refs/heads/main/openapi/university-of-illinois-urbana-champaign-rokwire-core.yaml
- filename: university-of-illinois-urbana-champaign-rokwire-gateway.yaml
  format: yaml
  label: Rokwire Gateway Building Block
  slug: rokwire-gateway
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-illinois-urbana-champaign/refs/heads/main/openapi/university-of-illinois-urbana-champaign-rokwire-gateway.yaml
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
