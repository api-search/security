---
api_key_in: []
api_specs:
- filename: censys-account-management-api-openapi.yml
  format: yaml
  label: Censys Account Management API
  slug: censys-account-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/censys/refs/heads/main/openapi/censys-account-management-api-openapi.yml
- filename: censys-adversary-investigation-api-openapi.yml
  format: yaml
  label: Censys Adversary Investigation API
  slug: censys-adversary-investigation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/censys/refs/heads/main/openapi/censys-adversary-investigation-api-openapi.yml
- filename: censys-asset-graphs-api-openapi.yml
  format: yaml
  label: Censys Asset Graphs API
  slug: censys-asset-graphs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/censys/refs/heads/main/openapi/censys-asset-graphs-api-openapi.yml
- filename: censys-assets-api-openapi.yml
  format: yaml
  label: Censys Assets API
  slug: censys-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/censys/refs/heads/main/openapi/censys-assets-api-openapi.yml
- filename: censys-collections-api-openapi.yml
  format: yaml
  label: Censys Collections API
  slug: censys-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/censys/refs/heads/main/openapi/censys-collections-api-openapi.yml
- filename: censys-excluded-assets-api-openapi.yml
  format: yaml
  label: Censys Excluded Assets API
  slug: censys-excluded-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/censys/refs/heads/main/openapi/censys-excluded-assets-api-openapi.yml
- filename: censys-global-data-api-openapi.yml
  format: yaml
  label: Censys Global Data API
  slug: censys-global-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/censys/refs/heads/main/openapi/censys-global-data-api-openapi.yml
- filename: censys-graph-executions-api-openapi.yml
  format: yaml
  label: Censys Graph Executions API
  slug: censys-graph-executions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/censys/refs/heads/main/openapi/censys-graph-executions-api-openapi.yml
- filename: censys-risks-api-openapi.yml
  format: yaml
  label: Censys Risks API
  slug: censys-risks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/censys/refs/heads/main/openapi/censys-risks-api-openapi.yml
- filename: censys-seeds-api-openapi.yml
  format: yaml
  label: Censys Seeds API
  slug: censys-seeds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/censys/refs/heads/main/openapi/censys-seeds-api-openapi.yml
- filename: censys-shards-api-openapi.yml
  format: yaml
  label: Censys Shards API
  slug: censys-shards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/censys/refs/heads/main/openapi/censys-shards-api-openapi.yml
- filename: censys-supply-chain-intelligence-api-openapi.yml
  format: yaml
  label: Censys Supply Chain Intelligence API
  slug: censys-supply-chain-intelligence-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/censys/refs/heads/main/openapi/censys-supply-chain-intelligence-api-openapi.yml
- filename: censys-tags-and-comments-api-openapi.yml
  format: yaml
  label: Censys Tags and Comments API
  slug: censys-tags-and-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/censys/refs/heads/main/openapi/censys-tags-and-comments-api-openapi.yml
- filename: censys-threat-hunting-api-openapi.yml
  format: yaml
  label: Censys Threat Hunting API
  slug: censys-threat-hunting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/censys/refs/heads/main/openapi/censys-threat-hunting-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Censys Authentication
name_suffix: Authentication
oauth_flows: []
overview: Censys secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Censys
provider_slug: censys
scheme_count: 1
schemes:
- description: Your Censys personal access token.
  name: PersonalAccessToken
  scheme: bearer
  sources:
  - openapi/censys-asset-graph-openapi.yml
  - openapi/censys-platform-openapi.yml
  type: http
slug: censys-authentication
source_filename: censys-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/censys-asset-graph-openapi.yml, openapi/censys-platform-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: PersonalAccessToken\n  type: http\n  scheme: bearer\n  description: Your Censys personal access token.\n  sources:\n  - openapi/censys-asset-graph-openapi.yml\n  - openapi/censys-platform-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/censys/refs/heads/main/authentication/censys-authentication.yml
summary_line: http · 1 scheme
tags:
- Security
- Internet Intelligence
- Attack Surface Management
- Threat Hunting
- Cyber Threat Intelligence
- OSINT
- Internet Scanning
- Certificates
- Asset Discovery
---
