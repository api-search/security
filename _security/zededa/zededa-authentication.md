---
api_key_in:
- header
api_specs:
- filename: zededa-node_service-openapi.json
  format: json
  label: ZEDEDA Edge Node Service
  slug: zededa-edge-node-service
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zededa/refs/heads/main/openapi/zededa-node_service-openapi.json
- filename: zededa-app_service-openapi.json
  format: json
  label: ZEDEDA Edge Application Service
  slug: zededa-edge-application-service
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zededa/refs/heads/main/openapi/zededa-app_service-openapi.json
- filename: zededa-app_profile_service-openapi.json
  format: json
  label: ZEDEDA App Profiles Service
  slug: zededa-app-profiles-service
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zededa/refs/heads/main/openapi/zededa-app_profile_service-openapi.json
- filename: zededa-network_service-openapi.json
  format: json
  label: ZEDEDA Edge Network Service
  slug: zededa-edge-network-service
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zededa/refs/heads/main/openapi/zededa-network_service-openapi.json
- filename: zededa-storage_service-openapi.json
  format: json
  label: ZEDEDA Storage Service
  slug: zededa-storage-service
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zededa/refs/heads/main/openapi/zededa-storage_service-openapi.json
- filename: zededa-kubernetes_service-openapi.json
  format: json
  label: ZEDEDA Kubernetes Service (ZKS)
  slug: zededa-kubernetes-service-zks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zededa/refs/heads/main/openapi/zededa-kubernetes_service-openapi.json
- filename: zededa-node_cluster_service-openapi.json
  format: json
  label: ZEDEDA Edge-Node Cluster Service
  slug: zededa-edge-node-cluster-service
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zededa/refs/heads/main/openapi/zededa-node_cluster_service-openapi.json
- filename: zededa-user_service-openapi.json
  format: json
  label: ZEDEDA IAM Service
  slug: zededa-iam-service
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zededa/refs/heads/main/openapi/zededa-user_service-openapi.json
- filename: zededa-job_service-openapi.json
  format: json
  label: ZEDEDA Job Service
  slug: zededa-job-service
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zededa/refs/heads/main/openapi/zededa-job_service-openapi.json
- filename: zededa-diag_service-openapi.json
  format: json
  label: ZEDEDA Diagnostics Service
  slug: zededa-diagnostics-service
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zededa/refs/heads/main/openapi/zededa-diag_service-openapi.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Zededa Authentication
name_suffix: Authentication
oauth_flows: []
overview: Zededa secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Zededa
provider_slug: zededa
scheme_count: 2
schemes:
- description: Bearer token for user session
  in: header
  name: BearerToken
  parameter: Authorization
  sources:
  - openapi/zededa-app_profile_service-openapi.json
  - openapi/zededa-app_service-openapi.json
  - openapi/zededa-diag_service-openapi.json
  - openapi/zededa-job_service-openapi.json
  - openapi/zededa-network_service-openapi.json
  - openapi/zededa-node_cluster_service-openapi.json
  - openapi/zededa-node_service-openapi.json
  - openapi/zededa-storage_service-openapi.json
  - openapi/zededa-user_service-openapi.json
  type: apiKey
- in: header
  name: ApiKeyAuth
  parameter: X-API-KEY
  sources:
  - openapi/zededa-kubernetes_service-openapi.json
  type: apiKey
slug: zededa-authentication
source_filename: zededa-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: derived\nsource: openapi/zededa-app_profile_service-openapi.json, openapi/zededa-app_service-openapi.json,\n  openapi/zededa-diag_service-openapi.json, openapi/zededa-job_service-openapi.json, openapi/zededa-kubernetes_service-openapi.json,\n  openapi/zededa-network_service-openapi.json, openapi/zededa-node_cluster_service-openapi.json,\n  openapi/zededa-node_service-openapi.json, openapi/zededa-storage_service-openapi.json, openapi/zededa-user_service-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: BearerToken\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Bearer token for user session\n  sources:\n  - openapi/zededa-app_profile_service-openapi.json\n  - openapi/zededa-app_service-openapi.json\n  - openapi/zededa-diag_service-openapi.json\n  - openapi/zededa-job_service-openapi.json\n  - openapi/zededa-network_service-openapi.json\n  - openapi/zededa-node_cluster_service-openapi.json\n\
  \  - openapi/zededa-node_service-openapi.json\n  - openapi/zededa-storage_service-openapi.json\n  - openapi/zededa-user_service-openapi.json\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-KEY\n  sources:\n  - openapi/zededa-kubernetes_service-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zededa/refs/heads/main/authentication/zededa-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Company
- Edge Computing
- Edge Intelligence
- IoT
- Kubernetes
- Device Management
- Orchestration
- AI at the Edge
---
