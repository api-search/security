---
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Capella Space Authentication
name_suffix: Authentication
oauth_flows: []
overview: Capella Space secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Capella Space
provider_slug: capella-space
scheme_count: 1
schemes:
- description: 'Bearer token issued via the Capella Console. API keys can be

    requested at POST /keys and exchanged for bearer tokens per the

    documented authentication flow.'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/capella-space-openapi.yml
  type: http
slug: capella-space-authentication
source_filename: capella-space-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/capella-space-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: |-\n    Bearer token issued via the Capella Console. API keys can be\n    requested at POST /keys and exchanged for bearer tokens per the\n    documented authentication flow.\n  sources:\n  - openapi/capella-space-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/capella-space/refs/heads/main/authentication/capella-space-authentication.yml
summary_line: http · 1 scheme
tags:
- Synthetic Aperture Radar
- SAR
- Earth Observation
- Satellite Imagery
- Geospatial
- STAC
- Remote Sensing
- Tasking
- Catalog
---
