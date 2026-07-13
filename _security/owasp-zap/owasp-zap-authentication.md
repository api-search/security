---
api_key_in:
- header
- query
api_specs:
- filename: owasp-zap-openapi.yml
  format: yaml
  label: OWASP ZAP API
  slug: owasp-zap
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/owasp-zap/refs/heads/main/openapi/owasp-zap-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Owasp Zap Authentication
name_suffix: Authentication
oauth_flows: []
overview: OWASP ZAP secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: OWASP ZAP
provider_slug: owasp-zap
scheme_count: 2
schemes:
- in: header
  name: apiKeyHeader
  parameter: X-ZAP-API-Key
  sources:
  - openapi/owasp-zap-openapi.yml
  type: apiKey
- in: query
  name: apiKeyQuery
  parameter: apikey
  sources:
  - openapi/owasp-zap-openapi.yml
  type: apiKey
slug: owasp-zap-authentication
source_filename: owasp-zap-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/owasp-zap-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  - query\nschemes:\n- name: apiKeyHeader\n  type: apiKey\n  in: header\n  parameter: X-ZAP-API-Key\n  sources:\n  - openapi/owasp-zap-openapi.yml\n- name: apiKeyQuery\n  type: apiKey\n  in: query\n  parameter: apikey\n  sources:\n  - openapi/owasp-zap-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/owasp-zap/refs/heads/main/authentication/owasp-zap-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Security Testing
- Application Security
- Vulnerability Scanning
- Testing
- Open Source
---
