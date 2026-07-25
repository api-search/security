---
api_key_in:
- cookie
api_specs:
- filename: cybereason-authentication-api-openapi.yml
  format: yaml
  label: Cybereason Authentication API
  slug: cybereason-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cybereason/refs/heads/main/openapi/cybereason-authentication-api-openapi.yml
- filename: cybereason-customdetectionrules-api-openapi.yml
  format: yaml
  label: Cybereason CustomDetectionRules API
  slug: cybereason-customdetectionrules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cybereason/refs/heads/main/openapi/cybereason-customdetectionrules-api-openapi.yml
- filename: cybereason-isolationrules-api-openapi.yml
  format: yaml
  label: Cybereason IsolationRules API
  slug: cybereason-isolationrules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cybereason/refs/heads/main/openapi/cybereason-isolationrules-api-openapi.yml
- filename: cybereason-malops-api-openapi.yml
  format: yaml
  label: Cybereason Malops API
  slug: cybereason-malops-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cybereason/refs/heads/main/openapi/cybereason-malops-api-openapi.yml
- filename: cybereason-remediation-api-openapi.yml
  format: yaml
  label: Cybereason Remediation API
  slug: cybereason-remediation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cybereason/refs/heads/main/openapi/cybereason-remediation-api-openapi.yml
- filename: cybereason-reputation-api-openapi.yml
  format: yaml
  label: Cybereason Reputation API
  slug: cybereason-reputation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cybereason/refs/heads/main/openapi/cybereason-reputation-api-openapi.yml
- filename: cybereason-sensors-api-openapi.yml
  format: yaml
  label: Cybereason Sensors API
  slug: cybereason-sensors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cybereason/refs/heads/main/openapi/cybereason-sensors-api-openapi.yml
- filename: cybereason-threatintel-api-openapi.yml
  format: yaml
  label: Cybereason ThreatIntel API
  slug: cybereason-threatintel-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cybereason/refs/heads/main/openapi/cybereason-threatintel-api-openapi.yml
- filename: cybereason-visualsearch-api-openapi.yml
  format: yaml
  label: Cybereason VisualSearch API
  slug: cybereason-visualsearch-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cybereason/refs/heads/main/openapi/cybereason-visualsearch-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Cybereason Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cybereason secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Cybereason
provider_slug: cybereason
scheme_count: 2
schemes:
- description: Session cookie returned by POST /login.html.
  in: cookie
  name: SessionCookie
  parameter: JSESSIONID
  sources:
  - openapi/cybereason-openapi.yml
  type: apiKey
- bearerFormat: JWT
  description: Available on Cybereason 20.1+ for token-based access.
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/cybereason-openapi.yml
  type: http
slug: cybereason-authentication
source_filename: cybereason-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/cybereason-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - cookie\nschemes:\n- name: SessionCookie\n  type: apiKey\n  in: cookie\n  parameter: JSESSIONID\n  description: Session cookie returned by POST /login.html.\n  sources:\n  - openapi/cybereason-openapi.yml\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: Available on Cybereason 20.1+ for token-based access.\n  sources:\n  - openapi/cybereason-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cybereason/refs/heads/main/authentication/cybereason-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Cybersecurity
- XDR
- EDR
- NGAV
- MDR
- Endpoint Security
- Threat Detection
---
