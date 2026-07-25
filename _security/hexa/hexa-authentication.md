---
api_key_in: []
api_specs:
- filename: hexa-cells-api-openapi.yml
  format: yaml
  label: Hex Cells API
  slug: hexa-cells-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hexa/refs/heads/main/openapi/hexa-cells-api-openapi.yml
- filename: hexa-collections-api-openapi.yml
  format: yaml
  label: Hex Collections API
  slug: hexa-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hexa/refs/heads/main/openapi/hexa-collections-api-openapi.yml
- filename: hexa-data-connections-api-openapi.yml
  format: yaml
  label: Hex Data Connections API
  slug: hexa-data-connections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hexa/refs/heads/main/openapi/hexa-data-connections-api-openapi.yml
- filename: hexa-embedding-api-openapi.yml
  format: yaml
  label: Hex Embedding API
  slug: hexa-embedding-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hexa/refs/heads/main/openapi/hexa-embedding-api-openapi.yml
- filename: hexa-groups-api-openapi.yml
  format: yaml
  label: Hex Groups API
  slug: hexa-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hexa/refs/heads/main/openapi/hexa-groups-api-openapi.yml
- filename: hexa-guides-api-openapi.yml
  format: yaml
  label: Hex Guides API
  slug: hexa-guides-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hexa/refs/heads/main/openapi/hexa-guides-api-openapi.yml
- filename: hexa-projects-api-openapi.yml
  format: yaml
  label: Hex Projects API
  slug: hexa-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hexa/refs/heads/main/openapi/hexa-projects-api-openapi.yml
- filename: hexa-semantic-projects-models-api-openapi.yml
  format: yaml
  label: Hex Semantic (projects|models) API
  slug: hexa-semantic-projects-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hexa/refs/heads/main/openapi/hexa-semantic-projects-models-api-openapi.yml
- filename: hexa-users-api-openapi.yml
  format: yaml
  label: Hex Users API
  slug: hexa-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hexa/refs/heads/main/openapi/hexa-users-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Hexa Authentication
name_suffix: Authentication
oauth_flows: []
overview: Hex secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Hex
provider_slug: hexa
scheme_count: 1
schemes:
- name: bearerAuth
  scheme: bearer
  sources:
  - openapi/hexa-openapi.yml
  type: http
slug: hexa-authentication
source_filename: hexa-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/hexa-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/hexa-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hexa/refs/heads/main/authentication/hexa-authentication.yml
summary_line: http · 1 scheme
tags:
- Analytics
- Collaboration
- Data
- Notebooks
---
