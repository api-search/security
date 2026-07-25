---
api_key_in: []
api_specs:
- filename: capella-space-collects-api-openapi.yml
  format: yaml
  label: Capella Space Collects API
  slug: capella-space-collects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/capella-space/refs/heads/main/openapi/capella-space-collects-api-openapi.yml
- filename: capella-space-keys-api-openapi.yml
  format: yaml
  label: Capella Space Keys API
  slug: capella-space-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/capella-space/refs/heads/main/openapi/capella-space-keys-api-openapi.yml
- filename: capella-space-orders-api-openapi.yml
  format: yaml
  label: Capella Space Orders API
  slug: capella-space-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/capella-space/refs/heads/main/openapi/capella-space-orders-api-openapi.yml
- filename: capella-space-repeatrequests-api-openapi.yml
  format: yaml
  label: Capella Space RepeatRequests API
  slug: capella-space-repeatrequests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/capella-space/refs/heads/main/openapi/capella-space-repeatrequests-api-openapi.yml
- filename: capella-space-tasking-api-openapi.yml
  format: yaml
  label: Capella Space Tasking API
  slug: capella-space-tasking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/capella-space/refs/heads/main/openapi/capella-space-tasking-api-openapi.yml
- filename: capella-space-tiles-api-openapi.yml
  format: yaml
  label: Capella Space Tiles API
  slug: capella-space-tiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/capella-space/refs/heads/main/openapi/capella-space-tiles-api-openapi.yml
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
