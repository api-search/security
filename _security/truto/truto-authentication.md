---
api_key_in: []
api_specs:
- filename: truto-admin-openapi.yml
  format: yaml
  label: Truto Admin API
  slug: truto-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truto/refs/heads/main/openapi/truto-admin-openapi.yml
- filename: truto-unified-hris-openapi.yml
  format: yaml
  label: Truto Unified HRIS API
  slug: truto-unified-hris-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truto/refs/heads/main/openapi/truto-unified-hris-openapi.yml
- filename: truto-unified-ats-openapi.yml
  format: yaml
  label: Truto Unified ATS API
  slug: truto-unified-ats-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truto/refs/heads/main/openapi/truto-unified-ats-openapi.yml
- filename: truto-unified-crm-openapi.yml
  format: yaml
  label: Truto Unified CRM API
  slug: truto-unified-crm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truto/refs/heads/main/openapi/truto-unified-crm-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Truto Authentication
name_suffix: Authentication
oauth_flows: []
overview: Truto secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Truto
provider_slug: truto
scheme_count: 1
schemes:
- description: Tenant Bearer token from the Truto dashboard.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/truto-admin-openapi.yml
  - openapi/truto-unified-ats-openapi.yml
  - openapi/truto-unified-crm-openapi.yml
  - openapi/truto-unified-hris-openapi.yml
  type: http
slug: truto-authentication
source_filename: truto-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/truto-admin-openapi.yml, openapi/truto-unified-ats-openapi.yml, openapi/truto-unified-crm-openapi.yml,\n  openapi/truto-unified-hris-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Tenant Bearer token from the Truto dashboard.\n  sources:\n  - openapi/truto-admin-openapi.yml\n  - openapi/truto-unified-ats-openapi.yml\n  - openapi/truto-unified-crm-openapi.yml\n  - openapi/truto-unified-hris-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/truto/refs/heads/main/authentication/truto-authentication.yml
summary_line: http · 1 scheme
tags:
- Unified API
- Integration Platform
- HRIS
- ATS
- CRM
- Embedded Integrations
- MCP
- AI Agents
- SaaS
---
