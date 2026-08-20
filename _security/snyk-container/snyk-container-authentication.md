---
api_key_in: []
api_specs:
- filename: snyk-container-container-projects-api-openapi.yml
  format: yaml
  label: Snyk Container Container Projects API
  slug: snyk-container-container-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snyk-container/refs/heads/main/openapi/snyk-container-container-projects-api-openapi.yml
- filename: snyk-container-issues-api-openapi.yml
  format: yaml
  label: Snyk Container Issues API
  slug: snyk-container-issues-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snyk-container/refs/heads/main/openapi/snyk-container-issues-api-openapi.yml
- filename: snyk-container-targets-api-openapi.yml
  format: yaml
  label: Snyk Container Targets API
  slug: snyk-container-targets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snyk-container/refs/heads/main/openapi/snyk-container-targets-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Snyk Container Authentication
name_suffix: Authentication
oauth_flows: []
overview: Snyk Container secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Snyk Container
provider_slug: snyk-container
scheme_count: 1
schemes:
- description: Snyk API token obtained from your Snyk account settings
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/snyk-container-openapi.yml
  type: http
slug: snyk-container-authentication
source_filename: snyk-container-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/snyk-container-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: Snyk API token obtained from your Snyk account settings\n  sources:\n  - openapi/snyk-container-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/snyk-container/refs/heads/main/authentication/snyk-container-authentication.yml
summary_line: http · 1 scheme
tags:
- Container Images
- Containers
- Kubernetes
- Security
- Vulnerability Management
- DevSecOps
- Open-Source
---
