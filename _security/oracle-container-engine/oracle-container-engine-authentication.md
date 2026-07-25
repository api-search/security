---
api_key_in:
- header
api_specs:
- filename: oracle-container-engine-add-ons-api-openapi.yml
  format: yaml
  label: Oracle Container Engine for Kubernetes Add-ons API
  slug: oracle-container-engine-add-ons-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-container-engine/refs/heads/main/openapi/oracle-container-engine-add-ons-api-openapi.yml
- filename: oracle-container-engine-clusters-api-openapi.yml
  format: yaml
  label: Oracle Container Engine for Kubernetes Clusters API
  slug: oracle-container-engine-clusters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-container-engine/refs/heads/main/openapi/oracle-container-engine-clusters-api-openapi.yml
- filename: oracle-container-engine-credentials-api-openapi.yml
  format: yaml
  label: Oracle Container Engine for Kubernetes Credentials API
  slug: oracle-container-engine-credentials-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-container-engine/refs/heads/main/openapi/oracle-container-engine-credentials-api-openapi.yml
- filename: oracle-container-engine-node-pools-api-openapi.yml
  format: yaml
  label: Oracle Container Engine for Kubernetes Node Pools API
  slug: oracle-container-engine-node-pools-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-container-engine/refs/heads/main/openapi/oracle-container-engine-node-pools-api-openapi.yml
- filename: oracle-container-engine-virtual-node-pools-api-openapi.yml
  format: yaml
  label: Oracle Container Engine for Kubernetes Virtual Node Pools API
  slug: oracle-container-engine-virtual-node-pools-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-container-engine/refs/heads/main/openapi/oracle-container-engine-virtual-node-pools-api-openapi.yml
- filename: oracle-container-engine-work-requests-api-openapi.yml
  format: yaml
  label: Oracle Container Engine for Kubernetes Work Requests API
  slug: oracle-container-engine-work-requests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/oracle-container-engine/refs/heads/main/openapi/oracle-container-engine-work-requests-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Oracle Container Engine Authentication
name_suffix: Authentication
oauth_flows: []
overview: Oracle Container Engine for Kubernetes secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Oracle Container Engine for Kubernetes
provider_slug: oracle-container-engine
scheme_count: 1
schemes:
- description: OCI request signing (RFC 7615) using API key pair
  in: header
  name: ociAuth
  parameter: Authorization
  sources:
  - openapi/oracle-container-engine-openapi.yml
  type: apiKey
slug: oracle-container-engine-authentication
source_filename: oracle-container-engine-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/oracle-container-engine-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ociAuth\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: OCI request signing (RFC 7615) using API key pair\n  sources:\n  - openapi/oracle-container-engine-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/oracle-container-engine/refs/heads/main/authentication/oracle-container-engine-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Cloud
- Containers
- Kubernetes
- Oracle
- Orchestration
---
