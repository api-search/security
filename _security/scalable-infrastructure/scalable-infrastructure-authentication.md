---
api_key_in:
- header
api_specs:
- filename: scalable-infrastructure-ec2-api-openapi.yml
  format: yaml
  label: Scalable Infrastructure EC2 API
  slug: scalable-infrastructure-ec2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/scalable-infrastructure/refs/heads/main/openapi/scalable-infrastructure-ec2-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Scalable Infrastructure Authentication
name_suffix: Authentication
oauth_flows: []
overview: Scalable Infrastructure secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Scalable Infrastructure
provider_slug: scalable-infrastructure
scheme_count: 1
schemes:
- description: AWS Signature Version 4 signed request (Authorization header).
  in: header
  name: SigV4
  parameter: Authorization
  sources:
  - openapi/scalable-infrastructure-openapi.yml
  type: apiKey
slug: scalable-infrastructure-authentication
source_filename: scalable-infrastructure-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/scalable-infrastructure-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: SigV4\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: AWS Signature Version 4 signed request (Authorization header).\n  sources:\n  - openapi/scalable-infrastructure-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/scalable-infrastructure/refs/heads/main/authentication/scalable-infrastructure-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Cloud Infrastructure
- Compute
- DevOps
- Infrastructure as Code
- Kubernetes
- Networking
- Scalability
- Storage
---
