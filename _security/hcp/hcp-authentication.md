---
api_key_in: []
api_specs:
- filename: hcp-apps-api-openapi.yml
  format: yaml
  label: HashiCorp Cloud Platform Apps API
  slug: hcp-apps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hcp/refs/heads/main/openapi/hcp-apps-api-openapi.yml
- filename: hcp-gateway-api-openapi.yml
  format: yaml
  label: HashiCorp Cloud Platform Gateway API
  slug: hcp-gateway-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hcp/refs/heads/main/openapi/hcp-gateway-api-openapi.yml
- filename: hcp-integrations-api-openapi.yml
  format: yaml
  label: HashiCorp Cloud Platform Integrations API
  slug: hcp-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hcp/refs/heads/main/openapi/hcp-integrations-api-openapi.yml
- filename: hcp-secrets-api-openapi.yml
  format: yaml
  label: HashiCorp Cloud Platform Secrets API
  slug: hcp-secrets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hcp/refs/heads/main/openapi/hcp-secrets-api-openapi.yml
- filename: hcp-sync-api-openapi.yml
  format: yaml
  label: HashiCorp Cloud Platform Sync API
  slug: hcp-sync-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hcp/refs/heads/main/openapi/hcp-sync-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Hcp Authentication
name_suffix: Authentication
oauth_flows: []
overview: HashiCorp Cloud Platform secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: HashiCorp Cloud Platform
provider_slug: hcp
scheme_count: 1
schemes:
- name: bearerAuth
  scheme: bearer
  sources:
  - openapi/hcp-openapi.yml
  type: http
slug: hcp-authentication
source_filename: hcp-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/hcp-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/hcp-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hcp/refs/heads/main/authentication/hcp-authentication.yml
summary_line: http · 1 scheme
tags:
- Cloud
- Infrastructure
- DevOps
- Secrets Management
- Service Networking
- Fortune 1000
---
