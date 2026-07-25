---
api_key_in:
- header
api_specs:
- filename: prosci-adkar-assessments-api-openapi.yml
  format: yaml
  label: Prosci ADKAR Assessments API
  slug: prosci-adkar-assessments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prosci/refs/heads/main/openapi/prosci-adkar-assessments-api-openapi.yml
- filename: prosci-change-plans-api-openapi.yml
  format: yaml
  label: Prosci Change Plans API
  slug: prosci-change-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prosci/refs/heads/main/openapi/prosci-change-plans-api-openapi.yml
- filename: prosci-organizations-api-openapi.yml
  format: yaml
  label: Prosci Organizations API
  slug: prosci-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prosci/refs/heads/main/openapi/prosci-organizations-api-openapi.yml
- filename: prosci-pct-assessments-api-openapi.yml
  format: yaml
  label: Prosci PCT Assessments API
  slug: prosci-pct-assessments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prosci/refs/heads/main/openapi/prosci-pct-assessments-api-openapi.yml
- filename: prosci-projects-api-openapi.yml
  format: yaml
  label: Prosci Projects API
  slug: prosci-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prosci/refs/heads/main/openapi/prosci-projects-api-openapi.yml
- filename: prosci-risk-assessment-api-openapi.yml
  format: yaml
  label: Prosci Risk Assessment API
  slug: prosci-risk-assessment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prosci/refs/heads/main/openapi/prosci-risk-assessment-api-openapi.yml
- filename: prosci-stakeholders-api-openapi.yml
  format: yaml
  label: Prosci Stakeholders API
  slug: prosci-stakeholders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prosci/refs/heads/main/openapi/prosci-stakeholders-api-openapi.yml
- filename: prosci-training-api-openapi.yml
  format: yaml
  label: Prosci Training API
  slug: prosci-training-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/prosci/refs/heads/main/openapi/prosci-training-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Prosci Authentication
name_suffix: Authentication
oauth_flows: []
overview: Prosci secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Prosci
provider_slug: prosci
scheme_count: 2
schemes:
- bearerFormat: JWT
  description: JWT token obtained from the Prosci authentication endpoint.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/prosci-change-management-openapi.yml
  type: http
- description: API key provided by Prosci for application access.
  in: header
  name: apiKeyAuth
  parameter: X-API-Key
  sources:
  - openapi/prosci-change-management-openapi.yml
  type: apiKey
slug: prosci-authentication
source_filename: prosci-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/prosci-change-management-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: JWT token obtained from the Prosci authentication endpoint.\n  sources:\n  - openapi/prosci-change-management-openapi.yml\n- name: apiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: API key provided by Prosci for application access.\n  sources:\n  - openapi/prosci-change-management-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/prosci/refs/heads/main/authentication/prosci-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Change Management
- Methodology
- Training
---
