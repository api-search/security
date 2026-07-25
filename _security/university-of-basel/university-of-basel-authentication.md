---
api_key_in: []
api_specs:
- filename: university-of-basel-admin-api-api-openapi.yml
  format: yaml
  label: University of Basel Admin API API
  slug: university-of-basel-admin-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-basel/refs/heads/main/openapi/university-of-basel-admin-api-api-openapi.yml
- filename: university-of-basel-api-v2-api-openapi.yml
  format: yaml
  label: University of Basel API v2 API
  slug: university-of-basel-api-v2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-basel/refs/heads/main/openapi/university-of-basel-api-v2-api-openapi.yml
- filename: university-of-basel-api-v3-api-openapi.yml
  format: yaml
  label: University of Basel API v3 API
  slug: university-of-basel-api-v3-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-basel/refs/heads/main/openapi/university-of-basel-api-v3-api-openapi.yml
- filename: university-of-basel-management-api-api-openapi.yml
  format: yaml
  label: University of Basel Management API API
  slug: university-of-basel-management-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-basel/refs/heads/main/openapi/university-of-basel-management-api-api-openapi.yml
- filename: university-of-basel-ontology-mappings-api-openapi.yml
  format: yaml
  label: University of Basel Ontology Mappings API
  slug: university-of-basel-ontology-mappings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-basel/refs/heads/main/openapi/university-of-basel-ontology-mappings-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: University Of Basel Authentication
name_suffix: Authentication
oauth_flows: []
overview: University of Basel secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: University of Basel
provider_slug: university-of-basel
scheme_count: 2
schemes:
- name: httpAuth
  scheme: bearer
  sources:
  - openapi/university-of-basel-dsp-api.yaml
  type: http
- name: httpAuth1
  scheme: basic
  sources:
  - openapi/university-of-basel-dsp-api.yaml
  type: http
slug: university-of-basel-authentication
source_filename: university-of-basel-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/university-of-basel-dsp-api.yaml\nsummary:\n  types:\n  - http\nschemes:\n- name: httpAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/university-of-basel-dsp-api.yaml\n- name: httpAuth1\n  type: http\n  scheme: basic\n  sources:\n  - openapi/university-of-basel-dsp-api.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/university-of-basel/refs/heads/main/authentication/university-of-basel-authentication.yml
summary_line: http · 2 schemes
tags:
- Education
- Higher Education
- University
- Switzerland
- Research Data
- Open Access
- Institutional Repository
- Library
- Digital Humanities
---
