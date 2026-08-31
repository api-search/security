---
api_key_in:
- header
api_specs:
- filename: weld-connection-bridge-api-openapi.yml
  format: yaml
  label: Weld Connection Bridge API
  slug: weld-connection-bridge-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weld/refs/heads/main/openapi/weld-connection-bridge-api-openapi.yml
- filename: weld-connections-api-openapi.yml
  format: yaml
  label: Weld Connections API
  slug: weld-connections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weld/refs/heads/main/openapi/weld-connections-api-openapi.yml
- filename: weld-custom-reports-api-openapi.yml
  format: yaml
  label: Weld Custom Reports API
  slug: weld-custom-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weld/refs/heads/main/openapi/weld-custom-reports-api-openapi.yml
- filename: weld-elt-stream-runs-api-openapi.yml
  format: yaml
  label: Weld ELT Stream Runs API
  slug: weld-elt-stream-runs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weld/refs/heads/main/openapi/weld-elt-stream-runs-api-openapi.yml
- filename: weld-elt-streams-api-openapi.yml
  format: yaml
  label: Weld ELT Streams API
  slug: weld-elt-streams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weld/refs/heads/main/openapi/weld-elt-streams-api-openapi.yml
- filename: weld-elt-syncs-api-openapi.yml
  format: yaml
  label: Weld ELT Syncs API
  slug: weld-elt-syncs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weld/refs/heads/main/openapi/weld-elt-syncs-api-openapi.yml
- filename: weld-integrations-api-openapi.yml
  format: yaml
  label: Weld Integrations API
  slug: weld-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weld/refs/heads/main/openapi/weld-integrations-api-openapi.yml
- filename: weld-orchestration-runs-api-openapi.yml
  format: yaml
  label: Weld Orchestration Runs API
  slug: weld-orchestration-runs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weld/refs/heads/main/openapi/weld-orchestration-runs-api-openapi.yml
- filename: weld-orchestrations-api-openapi.yml
  format: yaml
  label: Weld Orchestrations API
  slug: weld-orchestrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weld/refs/heads/main/openapi/weld-orchestrations-api-openapi.yml
- filename: weld-reverse-etl-failed-records-api-openapi.yml
  format: yaml
  label: Weld Reverse ETL Failed Records API
  slug: weld-reverse-etl-failed-records-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weld/refs/heads/main/openapi/weld-reverse-etl-failed-records-api-openapi.yml
- filename: weld-reverse-etl-sync-runs-api-openapi.yml
  format: yaml
  label: Weld Reverse ETL Sync Runs API
  slug: weld-reverse-etl-sync-runs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weld/refs/heads/main/openapi/weld-reverse-etl-sync-runs-api-openapi.yml
- filename: weld-reverse-etl-syncs-api-openapi.yml
  format: yaml
  label: Weld Reverse ETL Syncs API
  slug: weld-reverse-etl-syncs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weld/refs/heads/main/openapi/weld-reverse-etl-syncs-api-openapi.yml
- filename: weld-transforms-api-openapi.yml
  format: yaml
  label: Weld Transforms API
  slug: weld-transforms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weld/refs/heads/main/openapi/weld-transforms-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Weld Authentication
name_suffix: Authentication
oauth_flows: []
overview: Weld secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Weld
provider_slug: weld
scheme_count: 1
schemes:
- description: The API key from Settings -> API Keys
  in: header
  name: api_key
  parameter: x-api-key
  sources:
  - openapi/weld-connect-openapi.json
  type: apiKey
slug: weld-authentication
source_filename: weld-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/weld-connect-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: api_key\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: The API key from Settings -> API Keys\n  sources:\n  - openapi/weld-connect-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/weld/refs/heads/main/authentication/weld-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Data
- ETL
- ELT
- Reverse ETL
- Data Pipeline
- Data Integration
- Change Data Capture
- Transformations
- Analytics
- MCP
- AI Agents
---
