---
api_key_in: []
api_specs:
- filename: openapi.yaml
  format: yaml
  label: DataCite REST API
  slug: datacite-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/datacite/lupo/master/openapi.yaml
- filename: openapi.yaml
  format: yaml
  label: DataCite MDS API
  slug: datacite-mds-api
  spec_type: OpenAPI
  url: https://github.com/datacite/sashimi/blob/master/openapi.yaml
- filename: openapi.yaml
  format: yaml
  label: DataCite Usage Reports API
  slug: datacite-usage-reports-api
  spec_type: OpenAPI
  url: https://github.com/datacite/sashimi/blob/master/openapi.yaml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Datacite Authentication
name_suffix: Authentication
oauth_flows: []
overview: DataCite secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: DataCite
provider_slug: datacite
scheme_count: 2
schemes:
- name: BasicAuth
  scheme: basic
  sources:
  - openapi/datacite-rest-api-openapi.yml
  type: http
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/datacite-rest-api-openapi.yml
  - openapi/datacite-usage-reports-api-openapi.yml
  type: http
slug: datacite-authentication
source_filename: datacite-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/datacite-rest-api-openapi.yml, openapi/datacite-usage-reports-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BasicAuth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/datacite-rest-api-openapi.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/datacite-rest-api-openapi.yml\n  - openapi/datacite-usage-reports-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/datacite/refs/heads/main/authentication/datacite-authentication.yml
summary_line: http · 2 schemes
tags:
- DOI
- Persistent Identifiers
- Scholarly Metadata
- Research Data
- Open Science
- Linked Data
---
