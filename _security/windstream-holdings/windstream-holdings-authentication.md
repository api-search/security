---
anonymous_access: false
api_key_in: []
api_specs:
- filename: windstream-holdings-agents-api-openapi.yml
  format: yaml
  label: Windstream Holdings Agents API
  slug: windstream-holdings-agents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/windstream-holdings/refs/heads/main/openapi/windstream-holdings-agents-api-openapi.yml
- filename: windstream-holdings-auto-attendants-api-openapi.yml
  format: yaml
  label: Windstream Holdings Auto Attendants API
  slug: windstream-holdings-auto-attendants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/windstream-holdings/refs/heads/main/openapi/windstream-holdings-auto-attendants-api-openapi.yml
- filename: windstream-holdings-calls-api-openapi.yml
  format: yaml
  label: Windstream Holdings Calls API
  slug: windstream-holdings-calls-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/windstream-holdings/refs/heads/main/openapi/windstream-holdings-calls-api-openapi.yml
- filename: windstream-holdings-extensions-api-openapi.yml
  format: yaml
  label: Windstream Holdings Extensions API
  slug: windstream-holdings-extensions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/windstream-holdings/refs/heads/main/openapi/windstream-holdings-extensions-api-openapi.yml
- filename: windstream-holdings-products-api-openapi.yml
  format: yaml
  label: Windstream Holdings Products API
  slug: windstream-holdings-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/windstream-holdings/refs/heads/main/openapi/windstream-holdings-products-api-openapi.yml
- filename: windstream-holdings-roles-api-openapi.yml
  format: yaml
  label: Windstream Holdings Roles API
  slug: windstream-holdings-roles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/windstream-holdings/refs/heads/main/openapi/windstream-holdings-roles-api-openapi.yml
- filename: windstream-holdings-system-api-openapi.yml
  format: yaml
  label: Windstream Holdings System API
  slug: windstream-holdings-system-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/windstream-holdings/refs/heads/main/openapi/windstream-holdings-system-api-openapi.yml
- filename: windstream-holdings-tenants-api-openapi.yml
  format: yaml
  label: Windstream Holdings Tenants API
  slug: windstream-holdings-tenants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/windstream-holdings/refs/heads/main/openapi/windstream-holdings-tenants-api-openapi.yml
- filename: windstream-holdings-users-api-openapi.yml
  format: yaml
  label: Windstream Holdings Users API
  slug: windstream-holdings-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/windstream-holdings/refs/heads/main/openapi/windstream-holdings-users-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: Windstream Holdings Authentication
name_suffix: Authentication
oauth_flows: []
overview: Windstream Holdings secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Windstream Holdings
provider_slug: windstream-holdings
scheme_count: 2
schemes:
- description: Bearer token authentication for CCS API
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/windstream-contact-center-openapi.yml
  type: http
- description: 'HTTP Basic Authentication using extension@tenantId credentials. Username formats: ext@tenantId, ext@tenantId.ID, ext@tenantDID.DID, ext@tenantURI.URI'
  name: basicAuth
  scheme: basic
  sources:
  - openapi/windstream-voice-openapi.yml
  type: http
slug: windstream-holdings-authentication
source_filename: windstream-holdings-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/windstream-contact-center-openapi.yml, openapi/windstream-voice-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Bearer token authentication for CCS API\n  sources:\n  - openapi/windstream-contact-center-openapi.yml\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: 'HTTP Basic Authentication using extension@tenantId credentials. Username formats:\n    ext@tenantId, ext@tenantId.ID, ext@tenantDID.DID, ext@tenantURI.URI'\n  sources:\n  - openapi/windstream-voice-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/windstream-holdings/refs/heads/main/authentication/windstream-holdings-authentication.yml
summary_line: http · 2 schemes
tags:
- Broadband
- Contact Center
- Managed Service
- Network Communications
- SD-WAN
- Telecommunications
- UCaaS
- Unified Communications
- Fortune 500
---
