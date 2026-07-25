---
api_key_in:
- header
api_specs:
- filename: vmware-clusters-api-openapi.yml
  format: yaml
  label: VMware Clusters API
  slug: vmware-clusters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vmware/refs/heads/main/openapi/vmware-clusters-api-openapi.yml
- filename: vmware-content-library-api-openapi.yml
  format: yaml
  label: VMware Content Library API
  slug: vmware-content-library-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vmware/refs/heads/main/openapi/vmware-content-library-api-openapi.yml
- filename: vmware-datacenters-api-openapi.yml
  format: yaml
  label: VMware Datacenters API
  slug: vmware-datacenters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vmware/refs/heads/main/openapi/vmware-datacenters-api-openapi.yml
- filename: vmware-datastores-api-openapi.yml
  format: yaml
  label: VMware Datastores API
  slug: vmware-datastores-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vmware/refs/heads/main/openapi/vmware-datastores-api-openapi.yml
- filename: vmware-folders-api-openapi.yml
  format: yaml
  label: VMware Folders API
  slug: vmware-folders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vmware/refs/heads/main/openapi/vmware-folders-api-openapi.yml
- filename: vmware-hosts-api-openapi.yml
  format: yaml
  label: VMware Hosts API
  slug: vmware-hosts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vmware/refs/heads/main/openapi/vmware-hosts-api-openapi.yml
- filename: vmware-networks-api-openapi.yml
  format: yaml
  label: VMware Networks API
  slug: vmware-networks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vmware/refs/heads/main/openapi/vmware-networks-api-openapi.yml
- filename: vmware-resource-pools-api-openapi.yml
  format: yaml
  label: VMware Resource Pools API
  slug: vmware-resource-pools-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vmware/refs/heads/main/openapi/vmware-resource-pools-api-openapi.yml
- filename: vmware-session-api-openapi.yml
  format: yaml
  label: VMware Session API
  slug: vmware-session-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vmware/refs/heads/main/openapi/vmware-session-api-openapi.yml
- filename: vmware-storage-policies-api-openapi.yml
  format: yaml
  label: VMware Storage Policies API
  slug: vmware-storage-policies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vmware/refs/heads/main/openapi/vmware-storage-policies-api-openapi.yml
- filename: vmware-tagging-api-openapi.yml
  format: yaml
  label: VMware Tagging API
  slug: vmware-tagging-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vmware/refs/heads/main/openapi/vmware-tagging-api-openapi.yml
- filename: vmware-vm-guest-api-openapi.yml
  format: yaml
  label: VMware VM Guest API
  slug: vmware-vm-guest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vmware/refs/heads/main/openapi/vmware-vm-guest-api-openapi.yml
- filename: vmware-vm-hardware-api-openapi.yml
  format: yaml
  label: VMware VM Hardware API
  slug: vmware-vm-hardware-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vmware/refs/heads/main/openapi/vmware-vm-hardware-api-openapi.yml
- filename: vmware-vm-power-api-openapi.yml
  format: yaml
  label: VMware VM Power API
  slug: vmware-vm-power-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vmware/refs/heads/main/openapi/vmware-vm-power-api-openapi.yml
- filename: vmware-vms-api-openapi.yml
  format: yaml
  label: VMware VMs API
  slug: vmware-vms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vmware/refs/heads/main/openapi/vmware-vms-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Vmware Authentication
name_suffix: Authentication
oauth_flows: []
overview: VMware secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: VMware
provider_slug: vmware
scheme_count: 2
schemes:
- description: Session token obtained from POST /session. Include this header in all subsequent API requests.
  in: header
  name: sessionAuth
  parameter: vmware-api-session-id
  sources:
  - openapi/vmware-vsphere-api-openapi.yml
  type: apiKey
- description: HTTP Basic authentication using vCenter Server credentials. Used primarily for creating sessions.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/vmware-vsphere-api-openapi.yml
  type: http
slug: vmware-authentication
source_filename: vmware-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/vmware-vsphere-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: sessionAuth\n  type: apiKey\n  in: header\n  parameter: vmware-api-session-id\n  description: Session token obtained from POST /session. Include this header in all subsequent\n    API requests.\n  sources:\n  - openapi/vmware-vsphere-api-openapi.yml\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic authentication using vCenter Server credentials. Used primarily for\n    creating sessions.\n  sources:\n  - openapi/vmware-vsphere-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vmware/refs/heads/main/authentication/vmware-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Cloud Computing
- Container Management
- Hybrid Cloud
- Infrastructure
- Virtualization
---
