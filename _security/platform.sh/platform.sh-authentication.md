---
api_key_in: []
api_specs:
- filename: platform.sh-rest-api-openapi.json
  format: json
  label: Platform.sh REST API
  slug: platform.sh-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/platform.sh/refs/heads/main/openapi/platform.sh-rest-api-openapi.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Platform.Sh Authentication
name_suffix: Authentication
oauth_flows: []
overview: Platform.sh secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Platform.sh
provider_slug: platform.sh
scheme_count: 1
schemes:
- name: BearerAuth
  scheme: bearer
  sources:
  - openapi/platform.sh-rest-api-openapi.json
  type: http
slug: platform.sh-authentication
source_filename: platform.sh-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: derived\nsource: openapi/platform.sh-rest-api-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/platform.sh-rest-api-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/platform.sh/refs/heads/main/authentication/platform.sh-authentication.yml
summary_line: http · 1 scheme
tags:
- Platform as a Service
- Cloud Hosting
- Application Hosting
- Deployment
- DevOps
- Continuous Deployment
- Containers
- Managed Services
- Developer Tools
- Infrastructure
- Multicloud
- Web Hosting
---
