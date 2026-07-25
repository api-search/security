---
api_key_in:
- header
api_specs:
- filename: broadcom-alerts-api-openapi.yml
  format: yaml
  label: Broadcom Alerts API
  slug: broadcom-alerts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/broadcom/refs/heads/main/openapi/broadcom-alerts-api-openapi.yml
- filename: broadcom-api-tokens-api-openapi.yml
  format: yaml
  label: Broadcom API Tokens API
  slug: broadcom-api-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/broadcom/refs/heads/main/openapi/broadcom-api-tokens-api-openapi.yml
- filename: broadcom-authentication-api-openapi.yml
  format: yaml
  label: Broadcom Authentication API
  slug: broadcom-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/broadcom/refs/heads/main/openapi/broadcom-authentication-api-openapi.yml
- filename: broadcom-clusters-api-openapi.yml
  format: yaml
  label: Broadcom Clusters API
  slug: broadcom-clusters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/broadcom/refs/heads/main/openapi/broadcom-clusters-api-openapi.yml
- filename: broadcom-content-library-api-openapi.yml
  format: yaml
  label: Broadcom Content Library API
  slug: broadcom-content-library-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/broadcom/refs/heads/main/openapi/broadcom-content-library-api-openapi.yml
- filename: broadcom-dashboards-api-openapi.yml
  format: yaml
  label: Broadcom Dashboards API
  slug: broadcom-dashboards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/broadcom/refs/heads/main/openapi/broadcom-dashboards-api-openapi.yml
- filename: broadcom-datastores-api-openapi.yml
  format: yaml
  label: Broadcom Datastores API
  slug: broadcom-datastores-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/broadcom/refs/heads/main/openapi/broadcom-datastores-api-openapi.yml
- filename: broadcom-events-api-openapi.yml
  format: yaml
  label: Broadcom Events API
  slug: broadcom-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/broadcom/refs/heads/main/openapi/broadcom-events-api-openapi.yml
- filename: broadcom-hosts-api-openapi.yml
  format: yaml
  label: Broadcom Hosts API
  slug: broadcom-hosts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/broadcom/refs/heads/main/openapi/broadcom-hosts-api-openapi.yml
- filename: broadcom-network-pools-api-openapi.yml
  format: yaml
  label: Broadcom Network Pools API
  slug: broadcom-network-pools-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/broadcom/refs/heads/main/openapi/broadcom-network-pools-api-openapi.yml
- filename: broadcom-networks-api-openapi.yml
  format: yaml
  label: Broadcom Networks API
  slug: broadcom-networks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/broadcom/refs/heads/main/openapi/broadcom-networks-api-openapi.yml
- filename: broadcom-proxies-api-openapi.yml
  format: yaml
  label: Broadcom Proxies API
  slug: broadcom-proxies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/broadcom/refs/heads/main/openapi/broadcom-proxies-api-openapi.yml
- filename: broadcom-query-api-openapi.yml
  format: yaml
  label: Broadcom Query API
  slug: broadcom-query-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/broadcom/refs/heads/main/openapi/broadcom-query-api-openapi.yml
- filename: broadcom-session-api-openapi.yml
  format: yaml
  label: Broadcom Session API
  slug: broadcom-session-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/broadcom/refs/heads/main/openapi/broadcom-session-api-openapi.yml
- filename: broadcom-sources-api-openapi.yml
  format: yaml
  label: Broadcom Sources API
  slug: broadcom-sources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/broadcom/refs/heads/main/openapi/broadcom-sources-api-openapi.yml
- filename: broadcom-tagging-api-openapi.yml
  format: yaml
  label: Broadcom Tagging API
  slug: broadcom-tagging-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/broadcom/refs/heads/main/openapi/broadcom-tagging-api-openapi.yml
- filename: broadcom-tasks-api-openapi.yml
  format: yaml
  label: Broadcom Tasks API
  slug: broadcom-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/broadcom/refs/heads/main/openapi/broadcom-tasks-api-openapi.yml
- filename: broadcom-upgrades-api-openapi.yml
  format: yaml
  label: Broadcom Upgrades API
  slug: broadcom-upgrades-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/broadcom/refs/heads/main/openapi/broadcom-upgrades-api-openapi.yml
- filename: broadcom-virtual-machines-api-openapi.yml
  format: yaml
  label: Broadcom Virtual Machines API
  slug: broadcom-virtual-machines-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/broadcom/refs/heads/main/openapi/broadcom-virtual-machines-api-openapi.yml
- filename: broadcom-workload-domains-api-openapi.yml
  format: yaml
  label: Broadcom Workload Domains API
  slug: broadcom-workload-domains-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/broadcom/refs/heads/main/openapi/broadcom-workload-domains-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Broadcom Authentication
name_suffix: Authentication
oauth_flows: []
overview: Broadcom secures its APIs with apiKey and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Broadcom
provider_slug: broadcom
scheme_count: 3
schemes:
- description: API token for authentication
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/broadcom-operations-for-applications-openapi.yml
  - openapi/broadcom-vmware-cloud-foundation-openapi.yml
  type: http
- name: basicAuth
  scheme: basic
  sources:
  - openapi/broadcom-vmware-cloud-foundation-openapi.yml
  - openapi/broadcom-vsphere-automation-openapi.yml
  type: http
- description: Session token obtained via POST /cis/session
  in: header
  name: sessionAuth
  parameter: vmware-api-session-id
  sources:
  - openapi/broadcom-vsphere-automation-openapi.yml
  type: apiKey
slug: broadcom-authentication
source_filename: broadcom-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/broadcom-operations-for-applications-openapi.yml, openapi/broadcom-vmware-cloud-foundation-openapi.yml,\n  openapi/broadcom-vsphere-automation-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: API token for authentication\n  sources:\n  - openapi/broadcom-operations-for-applications-openapi.yml\n  - openapi/broadcom-vmware-cloud-foundation-openapi.yml\n- name: basicAuth\n  type: http\n  scheme: basic\n  sources:\n  - openapi/broadcom-vmware-cloud-foundation-openapi.yml\n  - openapi/broadcom-vsphere-automation-openapi.yml\n- name: sessionAuth\n  type: apiKey\n  in: header\n  parameter: vmware-api-session-id\n  description: Session token obtained via POST /cis/session\n  sources:\n  - openapi/broadcom-vsphere-automation-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/broadcom/refs/heads/main/authentication/broadcom-authentication.yml
summary_line: apiKey/http · 3 schemes
tags:
- Cloud Infrastructure
- Gateways
- Management
- Networks
- Observability
- Virtualization
- Fortune 500
---
