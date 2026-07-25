---
api_key_in: []
api_specs:
- filename: hex-cells-api-openapi.yml
  format: yaml
  label: Hex Cells API
  slug: hex-cells-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hex/refs/heads/main/openapi/hex-cells-api-openapi.yml
- filename: hex-collections-api-openapi.yml
  format: yaml
  label: Hex Collections API
  slug: hex-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hex/refs/heads/main/openapi/hex-collections-api-openapi.yml
- filename: hex-context-api-openapi.yml
  format: yaml
  label: Hex Context API
  slug: hex-context-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hex/refs/heads/main/openapi/hex-context-api-openapi.yml
- filename: hex-data-connections-api-openapi.yml
  format: yaml
  label: Hex Data Connections API
  slug: hex-data-connections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hex/refs/heads/main/openapi/hex-data-connections-api-openapi.yml
- filename: hex-embedding-api-openapi.yml
  format: yaml
  label: Hex Embedding API
  slug: hex-embedding-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hex/refs/heads/main/openapi/hex-embedding-api-openapi.yml
- filename: hex-groups-api-openapi.yml
  format: yaml
  label: Hex Groups API
  slug: hex-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hex/refs/heads/main/openapi/hex-groups-api-openapi.yml
- filename: hex-guides-api-openapi.yml
  format: yaml
  label: Hex Guides API
  slug: hex-guides-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hex/refs/heads/main/openapi/hex-guides-api-openapi.yml
- filename: hex-projects-api-openapi.yml
  format: yaml
  label: Hex Projects API
  slug: hex-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hex/refs/heads/main/openapi/hex-projects-api-openapi.yml
- filename: hex-semantic-projects-models-api-openapi.yml
  format: yaml
  label: Hex Semantic (projects|models) API
  slug: hex-semantic-projects-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hex/refs/heads/main/openapi/hex-semantic-projects-models-api-openapi.yml
- filename: hex-threads-api-openapi.yml
  format: yaml
  label: Hex Threads API
  slug: hex-threads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hex/refs/heads/main/openapi/hex-threads-api-openapi.yml
- filename: hex-users-api-openapi.yml
  format: yaml
  label: Hex Users API
  slug: hex-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hex/refs/heads/main/openapi/hex-users-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Hex Authentication
name_suffix: Authentication
oauth_flows: []
overview: Hex secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Hex
provider_slug: hex
scheme_count: 1
schemes:
- name: bearerAuth
  scheme: bearer
  sources:
  - openapi/hex-openapi-original.json
  type: http
slug: hex-authentication
source_filename: hex-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: derived\nsource: openapi/hex-openapi-original.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/hex-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hex/refs/heads/main/authentication/hex-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Analytics
- Data Science
- Notebooks
- Business Intelligence
- Data Apps
- AI
- Agents
- Semantic Layer
- Developer Tools
---
