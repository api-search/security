---
api_key_in:
- header
api_specs:
- filename: trivy-server-openapi.yml
  format: yaml
  label: Trivy Server API
  slug: trivy-server
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/trivy/refs/heads/main/openapi/trivy-server-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Trivy Authentication
name_suffix: Authentication
oauth_flows: []
overview: Trivy secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Trivy
provider_slug: trivy
scheme_count: 1
schemes:
- description: Optional token-based authentication. When the server is started with --token, all requests must include the token in the Trivy-Token header.
  in: header
  name: TrivyToken
  parameter: Trivy-Token
  sources:
  - openapi/trivy-server-openapi.yml
  type: apiKey
slug: trivy-authentication
source_filename: trivy-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/trivy-server-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: TrivyToken\n  type: apiKey\n  in: header\n  parameter: Trivy-Token\n  description: Optional token-based authentication. When the server is started with --token,\n    all requests must include the token in the Trivy-Token header.\n  sources:\n  - openapi/trivy-server-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/trivy/refs/heads/main/authentication/trivy-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Containers
- Kubernetes
- SBOM
- Security
- Vulnerability Scanning
- Open Source
- DevSecOps
- Cloud Security
---
