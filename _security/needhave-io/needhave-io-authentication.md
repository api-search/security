---
anonymous_access: false
api_key_in: []
api_specs:
- filename: needhave-io-copier-api-openapi.yml
  format: yaml
  label: Needhave Copier API
  slug: needhave-io-copier-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/needhave-io/openapi/needhave-io-copier-api-openapi.yml
- filename: needhave-io-messages-api-openapi.yml
  format: yaml
  label: Needhave Messages API
  slug: needhave-io-messages-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/needhave-io/openapi/needhave-io-messages-api-openapi.yml
- filename: needhave-io-posts-api-openapi.yml
  format: yaml
  label: Needhave Posts API
  slug: needhave-io-posts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/needhave-io/openapi/needhave-io-posts-api-openapi.yml
- filename: needhave-io-stats-api-openapi.yml
  format: yaml
  label: Needhave Stats API
  slug: needhave-io-stats-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/needhave-io/openapi/needhave-io-stats-api-openapi.yml
- filename: needhave-io-threads-api-openapi.yml
  format: yaml
  label: Needhave Threads API
  slug: needhave-io-threads-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/needhave-io/openapi/needhave-io-threads-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Needhave Authentication
name_suffix: Authentication
oauth_flows: []
overview: Needhave secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Needhave
provider_slug: needhave-io
scheme_count: 1
schemes:
- description: COPIER_INGEST_SECRET. Off unless set. Never logged.
  name: ingestBearer
  scheme: bearer
  sources:
  - openapi/needhave-io-openapi.json
  type: http
slug: needhave-io-authentication
source_filename: needhave-io-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: derived\nsource: openapi/needhave-io-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: ingestBearer\n  type: http\n  scheme: bearer\n  description: COPIER_INGEST_SECRET. Off unless set. Never logged.\n  sources:\n  - openapi/needhave-io-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/needhave-io/authentication/needhave-io-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Public APIs
- No Auth
- Marketplace
- Open Data
---
