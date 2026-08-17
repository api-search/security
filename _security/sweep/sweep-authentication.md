---
api_key_in: []
api_specs:
- filename: sweep-api-openapi.yml
  format: yaml
  label: Sweep API
  slug: sweep-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sweep/refs/heads/main/openapi/sweep-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Sweep Authentication
name_suffix: Authentication
oauth_flows: []
overview: Sweep secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Sweep
provider_slug: sweep
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: bearer
  scheme: bearer
  sources:
  - openapi/sweep-api-openapi.yml
  type: http
slug: sweep-authentication
source_filename: sweep-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: derived\nsource: openapi/sweep-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearer\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/sweep-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sweep/refs/heads/main/authentication/sweep-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Cloud
- Salesforce
- RevOps
- Metadata
- Governance
- AI Agents
- Model Context Protocol
- Automation
- Documentation
- API
- REST API
- OpenAPI
- Enterprise Systems
- Snowflake
- ServiceNow
- Data Governance
---
