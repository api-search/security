---
api_key_in: []
api_specs:
- filename: relativityone-communications-api-openapi.yml
  format: yaml
  label: RelativityOne Communications API
  slug: relativityone-communications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/relativityone/refs/heads/main/openapi/relativityone-communications-api-openapi.yml
- filename: relativityone-custodians-api-openapi.yml
  format: yaml
  label: RelativityOne Custodians API
  slug: relativityone-custodians-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/relativityone/refs/heads/main/openapi/relativityone-custodians-api-openapi.yml
- filename: relativityone-entities-api-openapi.yml
  format: yaml
  label: RelativityOne Entities API
  slug: relativityone-entities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/relativityone/refs/heads/main/openapi/relativityone-entities-api-openapi.yml
- filename: relativityone-legal-hold-projects-api-openapi.yml
  format: yaml
  label: RelativityOne Legal Hold Projects API
  slug: relativityone-legal-hold-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/relativityone/refs/heads/main/openapi/relativityone-legal-hold-projects-api-openapi.yml
- filename: relativityone-preservation-api-openapi.yml
  format: yaml
  label: RelativityOne Preservation API
  slug: relativityone-preservation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/relativityone/refs/heads/main/openapi/relativityone-preservation-api-openapi.yml
- filename: relativityone-tasks-api-openapi.yml
  format: yaml
  label: RelativityOne Tasks API
  slug: relativityone-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/relativityone/refs/heads/main/openapi/relativityone-tasks-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Relativityone Authentication
name_suffix: Authentication
oauth_flows: []
overview: RelativityOne secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: RelativityOne
provider_slug: relativityone
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: Bearer token obtained via Microsoft Graph API OAuth flow.
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/relativityone-legal-hold-openapi.yml
  type: http
slug: relativityone-authentication
source_filename: relativityone-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/relativityone-legal-hold-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: Bearer token obtained via Microsoft Graph API OAuth flow.\n  sources:\n  - openapi/relativityone-legal-hold-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/relativityone/refs/heads/main/authentication/relativityone-authentication.yml
summary_line: http · 1 scheme
tags:
- eDiscovery
- Legal
- Legal Hold
- Document-Management
- Compliance
- Litigation
---
