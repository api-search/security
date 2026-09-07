---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: druva-authentication-openapi.json
  format: json
  label: Druva Authentication API
  slug: authentication
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/druva/refs/heads/main/openapi/druva-authentication-openapi.json
- filename: druva-msp-authentication-openapi.json
  format: json
  label: Druva MSP Authentication API
  slug: msp-authentication
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/druva/refs/heads/main/openapi/druva-msp-authentication-openapi.json
- filename: druva-govcloud-authentication-openapi.json
  format: json
  label: Druva GovCloud Authentication API
  slug: govcloud-authentication
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/druva/refs/heads/main/openapi/druva-govcloud-authentication-openapi.json
- filename: druva-hybrid-workload-govcloud-authentication-openapi.json
  format: json
  label: Druva Hybrid Workloads GovCloud Authentication API
  slug: hybrid-workload-govcloud-authentication
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/druva/refs/heads/main/openapi/druva-hybrid-workload-govcloud-authentication-openapi.json
- filename: druva-insync-cloud-openapi.json
  format: json
  label: Druva Endpoints and Data Governance API
  slug: endpoints-data-governance
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/druva/refs/heads/main/openapi/druva-insync-cloud-openapi.json
- filename: druva-insync-govcloud-openapi.json
  format: json
  label: Druva Endpoints and Data Governance GovCloud API
  slug: insync-govcloud
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/druva/refs/heads/main/openapi/druva-insync-govcloud-openapi.json
- filename: druva-enterprise-workloads-openapi.json
  format: json
  label: Druva Enterprise Workloads API
  slug: enterprise-workloads
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/druva/refs/heads/main/openapi/druva-enterprise-workloads-openapi.json
- filename: druva-enterprise-workloads-govcloud-openapi.json
  format: json
  label: Druva Enterprise Workloads GovCloud API
  slug: enterprise-workloads-govcloud
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/druva/refs/heads/main/openapi/druva-enterprise-workloads-govcloud-openapi.json
- filename: druva-cyber-resilience-openapi.json
  format: json
  label: Druva Cyber Resilience API
  slug: cyber-resilience
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/druva/refs/heads/main/openapi/druva-cyber-resilience-openapi.json
- filename: druva-cyber-resilience-govcloud-openapi.json
  format: json
  label: Druva Cyber Resilience GovCloud API
  slug: cyber-resilience-govcloud
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/druva/refs/heads/main/openapi/druva-cyber-resilience-govcloud-openapi.json
- filename: druva-cyber-resilience-govcloud-authorization-openapi.json
  format: json
  label: Druva GovCloud Cyber Resilience Authorization API
  slug: cyber-resilience-govcloud-authorization
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/druva/refs/heads/main/openapi/druva-cyber-resilience-govcloud-authorization-openapi.json
- filename: druva-cloudranger-openapi.json
  format: json
  label: Druva CloudRanger Native Workloads API
  slug: cloudranger
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/druva/refs/heads/main/openapi/druva-cloudranger-openapi.json
- filename: druva-aws-native-openapi.json
  format: json
  label: Druva AWS Native Workloads API
  slug: aws-native
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/druva/refs/heads/main/openapi/druva-aws-native-openapi.json
- filename: druva-msp-openapi.json
  format: json
  label: Druva MSP API
  slug: msp
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/druva/refs/heads/main/openapi/druva-msp-openapi.json
- filename: druva-platform-openapi.json
  format: json
  label: Druva Platform API
  slug: platform
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/druva/refs/heads/main/openapi/druva-platform-openapi.json
- filename: druva-microsoft-365-openapi.json
  format: json
  label: Druva Microsoft 365 API
  slug: microsoft-365
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/druva/refs/heads/main/openapi/druva-microsoft-365-openapi.json
- filename: druva-google-workspace-openapi.json
  format: json
  label: Druva Google Workspace API
  slug: google-workspace
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/druva/refs/heads/main/openapi/druva-google-workspace-openapi.json
- filename: druva-job-management-cloud-openapi.json
  format: json
  label: Druva Job Management API for Cloud Workloads
  slug: job-management-cloud
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/druva/refs/heads/main/openapi/druva-job-management-cloud-openapi.json
- filename: druva-job-management-govcloud-openapi.json
  format: json
  label: Druva Job Management API for GovCloud Workloads
  slug: job-management-govcloud
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/druva/refs/heads/main/openapi/druva-job-management-govcloud-openapi.json
- filename: druva-insync-cloud-openapi.json
  format: json
  label: Druva Legal Hold Targeted Download API
  slug: legal-hold
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/druva/refs/heads/main/openapi/druva-insync-cloud-openapi.json
auth_types:
- apiKey
- http
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 4
method: derived
name: Druva Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Druva secures its APIs with apiKey, http, and oauth2 across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Druva
provider_slug: druva
scheme_count: 4
schemes:
- name: sec0
  scheme: basic
  sources:
  - openapi/druva-authentication-openapi.json
  - openapi/druva-cyber-resilience-govcloud-authorization-openapi.json
  - openapi/druva-govcloud-authentication-openapi.json
  - openapi/druva-hybrid-workload-govcloud-authentication-openapi.json
  - openapi/druva-msp-authentication-openapi.json
  type: http
- flows:
  - flow: clientCredentials
    scopes: 1
    tokenUrl: https://apis.druva.com/token
  name: OAuth2
  sources:
  - openapi/druva-aws-native-openapi.json
  - openapi/druva-cyber-resilience-govcloud-openapi.json
  - openapi/druva-cyber-resilience-openapi.json
  - openapi/druva-enterprise-workloads-govcloud-openapi.json
  - openapi/druva-enterprise-workloads-openapi.json
  - openapi/druva-insync-cloud-openapi.json
  - openapi/druva-insync-govcloud-openapi.json
  - openapi/druva-job-management-cloud-openapi.json
  - openapi/druva-job-management-govcloud-openapi.json
  - openapi/druva-msp-openapi.json
  - openapi/druva-platform-openapi.json
  type: oauth2
- in: header
  name: Bearer
  parameter: Authorization
  sources:
  - openapi/druva-aws-native-openapi.json
  - openapi/druva-cloudranger-openapi.json
  - openapi/druva-cyber-resilience-govcloud-openapi.json
  - openapi/druva-cyber-resilience-openapi.json
  - openapi/druva-enterprise-workloads-govcloud-openapi.json
  - openapi/druva-enterprise-workloads-openapi.json
  - openapi/druva-google-workspace-openapi.json
  - openapi/druva-insync-cloud-openapi.json
  - openapi/druva-insync-govcloud-openapi.json
  - openapi/druva-job-management-cloud-openapi.json
  - openapi/druva-job-management-govcloud-openapi.json
  - openapi/druva-microsoft-365-openapi.json
  - openapi/druva-msp-openapi.json
  - openapi/druva-platform-openapi.json
  type: apiKey
- in: header
  name: api_key
  parameter: x-api-key
  sources:
  - openapi/druva-cloudranger-openapi.json
  type: apiKey
slug: druva-authentication
source_filename: druva-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-06'\nmethod: derived\nsource: openapi/druva-authentication-openapi.json, openapi/druva-aws-native-openapi.json, openapi/druva-cloudranger-openapi.json,\n  openapi/druva-cyber-resilience-govcloud-authorization-openapi.json, openapi/druva-cyber-resilience-govcloud-openapi.json,\n  openapi/druva-cyber-resilience-openapi.json, openapi/druva-enterprise-workloads-govcloud-openapi.json,\n  openapi/druva-enterprise-workloads-openapi.json, openapi/druva-google-workspace-openapi.json,\n  openapi/druva-govcloud-authentication-openapi.json, openapi/druva-hybrid-workload-govcloud-authentication-openapi.json,\n  openapi/druva-insync-cloud-openapi.json ...\nsummary:\n  types:\n  - apiKey\n  - http\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: sec0\n  type: http\n  scheme: basic\n  sources:\n  - openapi/druva-authentication-openapi.json\n  - openapi/druva-cyber-resilience-govcloud-authorization-openapi.json\n  - openapi/druva-govcloud-authentication-openapi.json\n\
  \  - openapi/druva-hybrid-workload-govcloud-authentication-openapi.json\n  - openapi/druva-msp-authentication-openapi.json\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://apis.druva.com/token\n    scopes: 1\n  sources:\n  - openapi/druva-aws-native-openapi.json\n  - openapi/druva-cyber-resilience-govcloud-openapi.json\n  - openapi/druva-cyber-resilience-openapi.json\n  - openapi/druva-enterprise-workloads-govcloud-openapi.json\n  - openapi/druva-enterprise-workloads-openapi.json\n  - openapi/druva-insync-cloud-openapi.json\n  - openapi/druva-insync-govcloud-openapi.json\n  - openapi/druva-job-management-cloud-openapi.json\n  - openapi/druva-job-management-govcloud-openapi.json\n  - openapi/druva-msp-openapi.json\n  - openapi/druva-platform-openapi.json\n- name: Bearer\n  type: apiKey\n  in: header\n  parameter: Authorization\n  sources:\n  - openapi/druva-aws-native-openapi.json\n  - openapi/druva-cloudranger-openapi.json\n  - openapi/druva-cyber-resilience-govcloud-openapi.json\n\
  \  - openapi/druva-cyber-resilience-openapi.json\n  - openapi/druva-enterprise-workloads-govcloud-openapi.json\n  - openapi/druva-enterprise-workloads-openapi.json\n  - openapi/druva-google-workspace-openapi.json\n  - openapi/druva-insync-cloud-openapi.json\n  - openapi/druva-insync-govcloud-openapi.json\n  - openapi/druva-job-management-cloud-openapi.json\n  - openapi/druva-job-management-govcloud-openapi.json\n  - openapi/druva-microsoft-365-openapi.json\n  - openapi/druva-msp-openapi.json\n  - openapi/druva-platform-openapi.json\n- name: api_key\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  sources:\n  - openapi/druva-cloudranger-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/druva/refs/heads/main/authentication/druva-authentication.yml
summary_line: apiKey/http/oauth2 · 4 schemes
tags:
- Backup
- Cyber Resilience
- Data Protection
- Disaster Recovery
- SaaS Backup
- Ransomware Recovery
- Data Governance
- Enterprise Workloads
- MSP
- Legal Hold
- Endpoints
- GovCloud
- MCP
---
