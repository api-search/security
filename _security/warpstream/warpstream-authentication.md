---
api_key_in:
- header
api_specs:
- filename: warpstream-acls-api-openapi.yml
  format: yaml
  label: WarpStream ACLs API
  slug: warpstream-acls-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/warpstream/refs/heads/main/openapi/warpstream-acls-api-openapi.yml
- filename: warpstream-api-keys-api-openapi.yml
  format: yaml
  label: WarpStream API Keys API
  slug: warpstream-api-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/warpstream/refs/heads/main/openapi/warpstream-api-keys-api-openapi.yml
- filename: warpstream-monitoring-api-openapi.yml
  format: yaml
  label: WarpStream Monitoring API
  slug: warpstream-monitoring-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/warpstream/refs/heads/main/openapi/warpstream-monitoring-api-openapi.yml
- filename: warpstream-pipelines-api-openapi.yml
  format: yaml
  label: WarpStream Pipelines API
  slug: warpstream-pipelines-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/warpstream/refs/heads/main/openapi/warpstream-pipelines-api-openapi.yml
- filename: warpstream-topics-api-openapi.yml
  format: yaml
  label: WarpStream Topics API
  slug: warpstream-topics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/warpstream/refs/heads/main/openapi/warpstream-topics-api-openapi.yml
- filename: warpstream-virtual-cluster-credentials-api-openapi.yml
  format: yaml
  label: WarpStream Virtual Cluster Credentials API
  slug: warpstream-virtual-cluster-credentials-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/warpstream/refs/heads/main/openapi/warpstream-virtual-cluster-credentials-api-openapi.yml
- filename: warpstream-virtual-clusters-api-openapi.yml
  format: yaml
  label: WarpStream Virtual Clusters API
  slug: warpstream-virtual-clusters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/warpstream/refs/heads/main/openapi/warpstream-virtual-clusters-api-openapi.yml
- filename: warpstream-workspaces-api-openapi.yml
  format: yaml
  label: WarpStream Workspaces API
  slug: warpstream-workspaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/warpstream/refs/heads/main/openapi/warpstream-workspaces-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Warpstream Authentication
name_suffix: Authentication
oauth_flows: []
overview: WarpStream secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: WarpStream
provider_slug: warpstream
scheme_count: 1
schemes:
- description: 'WarpStream API key. Three key types are supported: Application Keys (manage workspace-specific resources), Agent Keys (scoped to a specific virtual cluster), and Account Keys (manage account-level resources such as workspaces and users).'
  in: header
  name: ApiKeyAuth
  parameter: warpstream-api-key
  sources:
  - openapi/warpstream-management-openapi.yml
  type: apiKey
slug: warpstream-authentication
source_filename: warpstream-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/warpstream-management-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: warpstream-api-key\n  description: 'WarpStream API key. Three key types are supported: Application Keys (manage\n    workspace-specific resources), Agent Keys (scoped to a specific virtual cluster), and Account\n    Keys (manage account-level resources such as workspaces and users).'\n  sources:\n  - openapi/warpstream-management-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/warpstream/refs/heads/main/authentication/warpstream-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Kafka
- Streaming
- Serverless
- Object Storage
- BYOC
- Data Streaming
- Apache Kafka
- Message Queue
- Event Streaming
---
