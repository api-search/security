---
api_key_in:
- header
api_specs:
- filename: broadcom-vsphere-automation-openapi.yml
  format: yaml
  label: Broadcom vSphere Automation API
  slug: vsphere-automation
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/broadcom/refs/heads/main/openapi/broadcom-vsphere-automation-openapi.yml
- filename: broadcom-operations-for-applications-openapi.yml
  format: yaml
  label: Broadcom Operations for Applications REST API
  slug: operations-for-applications
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/broadcom/refs/heads/main/openapi/broadcom-operations-for-applications-openapi.yml
- filename: broadcom-vmware-cloud-foundation-openapi.yml
  format: yaml
  label: Broadcom VMware Cloud Foundation API
  slug: vmware-cloud-foundation
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/broadcom/refs/heads/main/openapi/broadcom-vmware-cloud-foundation-openapi.yml
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
