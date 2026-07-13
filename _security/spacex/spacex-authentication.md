---
api_key_in:
- header
api_specs:
- filename: spacex-rest-api-openapi.yml
  format: yaml
  label: SpaceX REST API (v4 + v5)
  slug: rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spacex/refs/heads/main/openapi/spacex-rest-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Spacex Authentication
name_suffix: Authentication
oauth_flows: []
overview: SpaceX (Community API) secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: SpaceX (Community API)
provider_slug: spacex
scheme_count: 1
schemes:
- description: 'Admin API key for destructive (create/update/delete) operations.

    Not required for any read endpoint.'
  in: header
  name: SpacexKey
  parameter: spacex-key
  sources:
  - openapi/spacex-rest-api-openapi.yml
  type: apiKey
slug: spacex-authentication
source_filename: spacex-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/spacex-rest-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: SpacexKey\n  type: apiKey\n  in: header\n  parameter: spacex-key\n  description: |-\n    Admin API key for destructive (create/update/delete) operations.\n    Not required for any read endpoint.\n  sources:\n  - openapi/spacex-rest-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/spacex/refs/heads/main/authentication/spacex-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Space
- Launch
- Satellites
- Starlink
- Falcon 9
- Falcon Heavy
- Dragon
- Rockets
- Open Source
- Community
- REST
- GraphQL
- Open Data
---
