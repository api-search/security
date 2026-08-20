---
api_key_in: []
api_specs:
- filename: truto-accounts-api-openapi.yml
  format: yaml
  label: Truto Accounts API
  slug: truto-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truto/refs/heads/main/openapi/truto-accounts-api-openapi.yml
- filename: truto-applications-api-openapi.yml
  format: yaml
  label: Truto Applications API
  slug: truto-applications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truto/refs/heads/main/openapi/truto-applications-api-openapi.yml
- filename: truto-candidates-api-openapi.yml
  format: yaml
  label: Truto Candidates API
  slug: truto-candidates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truto/refs/heads/main/openapi/truto-candidates-api-openapi.yml
- filename: truto-companies-api-openapi.yml
  format: yaml
  label: Truto Companies API
  slug: truto-companies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truto/refs/heads/main/openapi/truto-companies-api-openapi.yml
- filename: truto-contacts-api-openapi.yml
  format: yaml
  label: Truto Contacts API
  slug: truto-contacts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truto/refs/heads/main/openapi/truto-contacts-api-openapi.yml
- filename: truto-departments-api-openapi.yml
  format: yaml
  label: Truto Departments API
  slug: truto-departments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truto/refs/heads/main/openapi/truto-departments-api-openapi.yml
- filename: truto-employees-api-openapi.yml
  format: yaml
  label: Truto Employees API
  slug: truto-employees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truto/refs/heads/main/openapi/truto-employees-api-openapi.yml
- filename: truto-employments-api-openapi.yml
  format: yaml
  label: Truto Employments API
  slug: truto-employments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truto/refs/heads/main/openapi/truto-employments-api-openapi.yml
- filename: truto-groups-api-openapi.yml
  format: yaml
  label: Truto Groups API
  slug: truto-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truto/refs/heads/main/openapi/truto-groups-api-openapi.yml
- filename: truto-integrated-accounts-api-openapi.yml
  format: yaml
  label: Truto Integrated Accounts API
  slug: truto-integrated-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truto/refs/heads/main/openapi/truto-integrated-accounts-api-openapi.yml
- filename: truto-jobs-api-openapi.yml
  format: yaml
  label: Truto Jobs API
  slug: truto-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truto/refs/heads/main/openapi/truto-jobs-api-openapi.yml
- filename: truto-link-tokens-api-openapi.yml
  format: yaml
  label: Truto Link Tokens API
  slug: truto-link-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truto/refs/heads/main/openapi/truto-link-tokens-api-openapi.yml
- filename: truto-mcp-servers-api-openapi.yml
  format: yaml
  label: Truto MCP Servers API
  slug: truto-mcp-servers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truto/refs/heads/main/openapi/truto-mcp-servers-api-openapi.yml
- filename: truto-offers-api-openapi.yml
  format: yaml
  label: Truto Offers API
  slug: truto-offers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truto/refs/heads/main/openapi/truto-offers-api-openapi.yml
- filename: truto-opportunities-api-openapi.yml
  format: yaml
  label: Truto Opportunities API
  slug: truto-opportunities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truto/refs/heads/main/openapi/truto-opportunities-api-openapi.yml
- filename: truto-stages-api-openapi.yml
  format: yaml
  label: Truto Stages API
  slug: truto-stages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truto/refs/heads/main/openapi/truto-stages-api-openapi.yml
- filename: truto-tasks-api-openapi.yml
  format: yaml
  label: Truto Tasks API
  slug: truto-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truto/refs/heads/main/openapi/truto-tasks-api-openapi.yml
- filename: truto-timeoff-api-openapi.yml
  format: yaml
  label: Truto Timeoff API
  slug: truto-timeoff-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/truto/refs/heads/main/openapi/truto-timeoff-api-openapi.yml
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
- Unified-API
- Integration Platform
- HRIS
- ATS
- CRM
- Embedded Integrations
- MCP
- AI Agents
- Software-as-a-Service
---
