---
api_key_in:
- query
api_specs:
- filename: trefle-distributions-api-openapi.yml
  format: yaml
  label: Trefle Distributions API
  slug: trefle-distributions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trefle/refs/heads/main/openapi/trefle-distributions-api-openapi.yml
- filename: trefle-division-classes-api-openapi.yml
  format: yaml
  label: Trefle Division Classes API
  slug: trefle-division-classes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trefle/refs/heads/main/openapi/trefle-division-classes-api-openapi.yml
- filename: trefle-division-orders-api-openapi.yml
  format: yaml
  label: Trefle Division Orders API
  slug: trefle-division-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trefle/refs/heads/main/openapi/trefle-division-orders-api-openapi.yml
- filename: trefle-divisions-api-openapi.yml
  format: yaml
  label: Trefle Divisions API
  slug: trefle-divisions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trefle/refs/heads/main/openapi/trefle-divisions-api-openapi.yml
- filename: trefle-families-api-openapi.yml
  format: yaml
  label: Trefle Families API
  slug: trefle-families-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trefle/refs/heads/main/openapi/trefle-families-api-openapi.yml
- filename: trefle-genus-api-openapi.yml
  format: yaml
  label: Trefle Genus API
  slug: trefle-genus-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trefle/refs/heads/main/openapi/trefle-genus-api-openapi.yml
- filename: trefle-kingdoms-api-openapi.yml
  format: yaml
  label: Trefle Kingdoms API
  slug: trefle-kingdoms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trefle/refs/heads/main/openapi/trefle-kingdoms-api-openapi.yml
- filename: trefle-plants-api-openapi.yml
  format: yaml
  label: Trefle Plants API
  slug: trefle-plants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trefle/refs/heads/main/openapi/trefle-plants-api-openapi.yml
- filename: trefle-species-api-openapi.yml
  format: yaml
  label: Trefle Species API
  slug: trefle-species-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trefle/refs/heads/main/openapi/trefle-species-api-openapi.yml
- filename: trefle-subkingdoms-api-openapi.yml
  format: yaml
  label: Trefle Subkingdoms API
  slug: trefle-subkingdoms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trefle/refs/heads/main/openapi/trefle-subkingdoms-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Trefle Authentication
name_suffix: Authentication
oauth_flows: []
overview: Trefle secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Trefle
provider_slug: trefle
scheme_count: 1
schemes:
- description: 'Trefle personal access token obtained by registering at trefle.io. Can be passed as a query parameter (?token=YOUR_TOKEN) or in the Authorization header (Authorization: Bearer [example key]).'
  in: query
  name: tokenAuth
  parameter: token
  sources:
  - openapi/trefle-openapi.yml
  type: apiKey
slug: trefle-authentication
source_filename: trefle-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/trefle-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: tokenAuth\n  type: apiKey\n  in: query\n  parameter: token\n  description: 'Trefle personal access token obtained by registering at trefle.io. Can be passed\n    as a query parameter (?token=YOUR_TOKEN) or in the Authorization header (Authorization:\n    Bearer [example key]).'\n  sources:\n  - openapi/trefle-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/trefle/refs/heads/main/authentication/trefle-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Agriculture
- Botany
- Open Data
- Plants
- Science
---
