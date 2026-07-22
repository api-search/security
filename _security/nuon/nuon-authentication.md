---
api_key_in:
- header
api_specs:
- filename: nuon-oapi-v3-openapi.json
  format: json
  label: Nuon Control Plane API
  slug: nuon-control-plane-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nuon/refs/heads/main/openapi/nuon-oapi-v3-openapi.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Nuon Authentication
name_suffix: Authentication
oauth_flows: []
overview: Nuon secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Nuon
provider_slug: nuon
scheme_count: 2
schemes:
- description: Type "Bearer" followed by a space and token.
  in: header
  name: APIKey
  parameter: Authorization
  sources:
  - openapi/nuon-oapi-v2-openapi.json
  - openapi/nuon-oapi-v3-openapi.json
  type: apiKey
- description: Nuon org ID
  in: header
  name: OrgID
  parameter: X-Nuon-Org-ID
  sources:
  - openapi/nuon-oapi-v2-openapi.json
  - openapi/nuon-oapi-v3-openapi.json
  type: apiKey
slug: nuon-authentication
source_filename: nuon-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: derived\nsource: openapi/nuon-oapi-v2-openapi.json, openapi/nuon-oapi-v3-openapi.json\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: APIKey\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Type \"Bearer\" followed by a space and token.\n  sources:\n  - openapi/nuon-oapi-v2-openapi.json\n  - openapi/nuon-oapi-v3-openapi.json\n- name: OrgID\n  type: apiKey\n  in: header\n  parameter: X-Nuon-Org-ID\n  description: Nuon org ID\n  sources:\n  - openapi/nuon-oapi-v2-openapi.json\n  - openapi/nuon-oapi-v3-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nuon/refs/heads/main/authentication/nuon-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Company
- BYOC
- Deployment
- Continuous Delivery
- DevOps
- Infrastructure
- Cloud
- Multi-Cloud
- Kubernetes
- Terraform
- Platform Engineering
---
