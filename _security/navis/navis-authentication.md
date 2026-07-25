---
api_key_in:
- header
api_specs:
- filename: navis-gate-api-openapi.yml
  format: yaml
  label: Navis (Kaleris) Gate API
  slug: navis-gate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/navis/refs/heads/main/openapi/navis-gate-api-openapi.yml
- filename: navis-holds-api-openapi.yml
  format: yaml
  label: Navis (Kaleris) Holds API
  slug: navis-holds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/navis/refs/heads/main/openapi/navis-holds-api-openapi.yml
- filename: navis-operations-api-openapi.yml
  format: yaml
  label: Navis (Kaleris) Operations API
  slug: navis-operations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/navis/refs/heads/main/openapi/navis-operations-api-openapi.yml
- filename: navis-units-api-openapi.yml
  format: yaml
  label: Navis (Kaleris) Units API
  slug: navis-units-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/navis/refs/heads/main/openapi/navis-units-api-openapi.yml
- filename: navis-vessel-visits-api-openapi.yml
  format: yaml
  label: Navis (Kaleris) Vessel Visits API
  slug: navis-vessel-visits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/navis/refs/heads/main/openapi/navis-vessel-visits-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Navis Authentication
name_suffix: Authentication
oauth_flows: []
overview: Navis (Kaleris) secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Navis (Kaleris)
provider_slug: navis
scheme_count: 2
schemes:
- name: BasicAuth
  scheme: basic
  sources:
  - openapi/navis-n4-openapi.yml
  type: http
- in: header
  name: APIKey
  parameter: X-API-Key
  sources:
  - openapi/navis-n4-openapi.yml
  type: apiKey
slug: navis-authentication
source_filename: navis-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/navis-n4-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: BasicAuth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/navis-n4-openapi.yml\n- name: APIKey\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  sources:\n  - openapi/navis-n4-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/navis/refs/heads/main/authentication/navis-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Maritime
- Port
- Terminal
- Container
- Logistics
---
