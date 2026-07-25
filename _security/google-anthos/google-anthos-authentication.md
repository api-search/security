---
api_key_in: []
api_specs:
- filename: google-anthos-baremetalclusters-api-openapi.yml
  format: yaml
  label: Google Anthos BareMetalClusters API
  slug: google-anthos-baremetalclusters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-anthos/refs/heads/main/openapi/google-anthos-baremetalclusters-api-openapi.yml
- filename: google-anthos-vmwareclusters-api-openapi.yml
  format: yaml
  label: Google Anthos VmwareClusters API
  slug: google-anthos-vmwareclusters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-anthos/refs/heads/main/openapi/google-anthos-vmwareclusters-api-openapi.yml
- filename: google-anthos-vmwarenodepools-api-openapi.yml
  format: yaml
  label: Google Anthos VmwareNodePools API
  slug: google-anthos-vmwarenodepools-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/google-anthos/refs/heads/main/openapi/google-anthos-vmwarenodepools-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Google Anthos Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Google Anthos secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Google Anthos
provider_slug: google-anthos
scheme_count: 1
schemes:
- flows:
  - authorizationUrl: https://accounts.google.com/o/oauth2/auth
    flow: authorizationCode
    scopes: 1
    tokenUrl: https://oauth2.googleapis.com/token
  name: oauth2
  sources:
  - openapi/gke-on-prem-api-openapi.yml
  type: oauth2
slug: google-anthos-authentication
source_filename: google-anthos-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/gke-on-prem-api-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\nschemes:\n- name: oauth2\n  type: oauth2\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://accounts.google.com/o/oauth2/auth\n    tokenUrl: https://oauth2.googleapis.com/token\n    scopes: 1\n  sources:\n  - openapi/gke-on-prem-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/google-anthos/refs/heads/main/authentication/google-anthos-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Container Platform
- Hybrid Cloud
- Kubernetes
- Multi-Cloud
- On-Premises
- Service Mesh
---
