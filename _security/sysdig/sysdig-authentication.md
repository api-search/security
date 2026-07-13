---
api_key_in: []
api_specs:
- filename: sysdig-monitor-openapi.yml
  format: yaml
  label: Sysdig Monitor
  slug: sysdig-monitor
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sysdig/refs/heads/main/openapi/sysdig-monitor-openapi.yml
- filename: sysdig-secure-openapi.yml
  format: yaml
  label: Sysdig Secure
  slug: sysdig-secure
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sysdig/refs/heads/main/openapi/sysdig-secure-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Sysdig Authentication
name_suffix: Authentication
oauth_flows: []
overview: Sysdig secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Sysdig
provider_slug: sysdig
scheme_count: 1
schemes:
- description: Authenticate using a Sysdig API Token, Team-Based Service Account, or Global Service Account token as a Bearer token.
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/sysdig-monitor-openapi.yml
  - openapi/sysdig-secure-openapi.yml
  type: http
slug: sysdig-authentication
source_filename: sysdig-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/sysdig-monitor-openapi.yml, openapi/sysdig-secure-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: Authenticate using a Sysdig API Token, Team-Based Service Account, or Global\n    Service Account token as a Bearer token.\n  sources:\n  - openapi/sysdig-monitor-openapi.yml\n  - openapi/sysdig-secure-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sysdig/refs/heads/main/authentication/sysdig-authentication.yml
summary_line: http · 1 scheme
tags:
- Cloud Security
- Containers
- Kubernetes
- Runtime Security
- Security
- Vulnerability Management
- Monitoring
- Observability
- CSPM
- Compliance
---
