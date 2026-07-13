---
api_key_in:
- header
api_specs:
- filename: snyk-rest-openapi.json
  format: json
  label: Snyk REST API - Groups
  slug: rest-groups
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snyk/refs/heads/main/openapi/snyk-rest-openapi.json
- filename: snyk-rest-openapi.json
  format: json
  label: Snyk REST API - Organizations
  slug: rest-organizations
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snyk/refs/heads/main/openapi/snyk-rest-openapi.json
- filename: snyk-rest-openapi.json
  format: json
  label: Snyk REST API - Projects
  slug: rest-projects
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snyk/refs/heads/main/openapi/snyk-rest-openapi.json
- filename: snyk-rest-openapi.json
  format: json
  label: Snyk REST API - Issues
  slug: rest-issues
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snyk/refs/heads/main/openapi/snyk-rest-openapi.json
- filename: snyk-rest-openapi.json
  format: json
  label: Snyk REST API - Targets
  slug: rest-targets
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snyk/refs/heads/main/openapi/snyk-rest-openapi.json
- filename: snyk-rest-openapi.json
  format: json
  label: Snyk REST API - Integrations
  slug: rest-integrations
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snyk/refs/heads/main/openapi/snyk-rest-openapi.json
- filename: snyk-rest-openapi.json
  format: json
  label: Snyk REST API - Audit Logs
  slug: rest-audit-logs
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snyk/refs/heads/main/openapi/snyk-rest-openapi.json
- filename: snyk-rest-openapi.json
  format: json
  label: Snyk REST API - SBOMs
  slug: rest-sboms
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snyk/refs/heads/main/openapi/snyk-rest-openapi.json
- filename: snyk-rest-openapi.json
  format: json
  label: Snyk REST API - Container Images
  slug: rest-container-images
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snyk/refs/heads/main/openapi/snyk-rest-openapi.json
- filename: snyk-rest-openapi.json
  format: json
  label: Snyk REST API - Custom Base Images
  slug: rest-custom-base-images
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snyk/refs/heads/main/openapi/snyk-rest-openapi.json
- filename: snyk-rest-openapi.json
  format: json
  label: Snyk REST API - Webhooks
  slug: rest-webhooks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snyk/refs/heads/main/openapi/snyk-rest-openapi.json
- filename: snyk-rest-openapi.json
  format: json
  label: Snyk REST API - Export
  slug: rest-export
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/snyk/refs/heads/main/openapi/snyk-rest-openapi.json
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Snyk Authentication
name_suffix: Authentication
oauth_flows: []
overview: Snyk secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Snyk
provider_slug: snyk
scheme_count: 2
schemes:
- description: API key value must be prefixed with \"Token \".
  in: header
  name: APIToken
  parameter: Authorization
  sources:
  - openapi/snyk-rest-openapi.json
  type: apiKey
- name: BearerAuth
  scheme: bearer
  sources:
  - openapi/snyk-rest-openapi.json
  type: http
slug: snyk-authentication
source_filename: snyk-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/snyk-rest-openapi.json\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: APIToken\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: API key value must be prefixed with \\\"Token \\\".\n  sources:\n  - openapi/snyk-rest-openapi.json\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/snyk-rest-openapi.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/snyk/refs/heads/main/authentication/snyk-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Security
- DevSecOps
- Vulnerability Management
- Application Security
- SCA
- SAST
- Container Security
- IaC
---
