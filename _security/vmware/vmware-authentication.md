---
api_key_in:
- header
api_specs:
- filename: vmware-vsphere-api-openapi.yml
  format: yaml
  label: vSphere API
  slug: vsphere-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vmware/refs/heads/main/openapi/vmware-vsphere-api-openapi.yml
- filename: openapi.yaml
  format: yaml
  label: vCloud Director API
  slug: vcloud-director-api
  spec_type: OpenAPI
  url: https://developer.vmware.com/apis/vmware-cloud-director/latest/openapi/
- filename: openapi.yaml
  format: yaml
  label: NSX-T Data Center API
  slug: nsx-t-data-center-api
  spec_type: OpenAPI
  url: https://developer.vmware.com/apis/nsx-t/latest/openapi/
- filename: openapi.yaml
  format: yaml
  label: vRealize Automation API
  slug: vrealize-automation-api
  spec_type: OpenAPI
  url: https://developer.vmware.com/apis/vrealize-automation/latest/openapi/
- filename: openapi.yaml
  format: yaml
  label: VMware Cloud on AWS API
  slug: vmware-cloud-on-aws-api
  spec_type: OpenAPI
  url: https://developer.vmware.com/apis/vmc/latest/openapi/
- filename: openapi.yaml
  format: yaml
  label: vRealize Operations API
  slug: vrealize-operations-api
  spec_type: OpenAPI
  url: https://developer.vmware.com/apis/vrealize-operations/latest/openapi/
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
