---
api_key_in:
- cookie
api_specs:
- filename: infinidat-infinibox-openapi.yml
  format: yaml
  label: InfiniBox REST API (InfiniAPI)
  slug: infinibox-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/infinidat/refs/heads/main/openapi/infinidat-infinibox-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Infinidat Authentication
name_suffix: Authentication
oauth_flows: []
overview: Infinidat secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Infinidat
provider_slug: infinidat
scheme_count: 2
schemes:
- description: HTTP Basic authentication with an InfiniBox user, as used by InfiniSDK.
  name: basicAuth
  scheme: basic
  sources:
  - openapi/infinidat-infinibox-openapi.yml
  type: http
- description: Session established by POST /users/login and torn down by POST /users/logout.
  in: cookie
  name: sessionCookie
  parameter: sessionid
  sources:
  - openapi/infinidat-infinibox-openapi.yml
  type: apiKey
slug: infinidat-authentication
source_filename: infinidat-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-01'\nmethod: derived\nsource: openapi/infinidat-infinibox-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - cookie\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic authentication with an InfiniBox user, as used by InfiniSDK.\n  sources:\n  - openapi/infinidat-infinibox-openapi.yml\n- name: sessionCookie\n  type: apiKey\n  in: cookie\n  parameter: sessionid\n  description: Session established by POST /users/login and torn down by POST /users/logout.\n  sources:\n  - openapi/infinidat-infinibox-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/infinidat/refs/heads/main/authentication/infinidat-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- Storage
- Enterprise Storage
- Data Infrastructure
- Data Protection
- Cyber Resilience
- Backup and Recovery
- Kubernetes
- Infrastructure
- On-Premises
---
