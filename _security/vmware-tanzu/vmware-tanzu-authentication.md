---
api_key_in:
- header
api_specs:
- filename: vmware-tanzu-service-mesh-openapi.yml
  format: yaml
  label: VMware Tanzu Service Mesh API
  slug: tanzu-service-mesh-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vmware-tanzu/refs/heads/main/openapi/vmware-tanzu-service-mesh-openapi.yml
- filename: vmware-tanzu-kubernetes-grid-openapi.yml
  format: yaml
  label: VMware Tanzu Kubernetes Grid API
  slug: tanzu-kubernetes-grid-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vmware-tanzu/refs/heads/main/openapi/vmware-tanzu-kubernetes-grid-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Vmware Tanzu Authentication
name_suffix: Authentication
oauth_flows: []
overview: VMware Tanzu secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: VMware Tanzu
provider_slug: vmware-tanzu
scheme_count: 1
schemes:
- description: Short-lived Bearer token obtained by exchanging a CSP API token via POST /csp/gateway/am/api/auth/api-tokens/authorize.
  in: header
  name: CspAuthToken
  parameter: csp-auth-token
  sources:
  - openapi/vmware-tanzu-service-mesh-openapi.yml
  type: apiKey
slug: vmware-tanzu-authentication
source_filename: vmware-tanzu-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/vmware-tanzu-service-mesh-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: CspAuthToken\n  type: apiKey\n  in: header\n  parameter: csp-auth-token\n  description: Short-lived Bearer token obtained by exchanging a CSP API token via POST /csp/gateway/am/api/auth/api-tokens/authorize.\n  sources:\n  - openapi/vmware-tanzu-service-mesh-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vmware-tanzu/refs/heads/main/authentication/vmware-tanzu-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Cloud Native
- Containers
- Enterprise
- Kubernetes
- Multi-Cloud
- Service Mesh
- VMware
---
