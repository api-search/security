---
api_key_in: []
api_specs:
- filename: fivetran-connections-api-openapi.yml
  format: yaml
  label: Fivetran Connections API
  slug: fivetran-connections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fivetran/refs/heads/main/openapi/fivetran-connections-api-openapi.yml
- filename: fivetran-destinations-api-openapi.yml
  format: yaml
  label: Fivetran Destinations API
  slug: fivetran-destinations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fivetran/refs/heads/main/openapi/fivetran-destinations-api-openapi.yml
- filename: fivetran-groups-api-openapi.yml
  format: yaml
  label: Fivetran Groups API
  slug: fivetran-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fivetran/refs/heads/main/openapi/fivetran-groups-api-openapi.yml
- filename: fivetran-metadata-api-openapi.yml
  format: yaml
  label: Fivetran Metadata API
  slug: fivetran-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fivetran/refs/heads/main/openapi/fivetran-metadata-api-openapi.yml
- filename: fivetran-roles-api-openapi.yml
  format: yaml
  label: Fivetran Roles API
  slug: fivetran-roles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fivetran/refs/heads/main/openapi/fivetran-roles-api-openapi.yml
- filename: fivetran-teams-api-openapi.yml
  format: yaml
  label: Fivetran Teams API
  slug: fivetran-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fivetran/refs/heads/main/openapi/fivetran-teams-api-openapi.yml
- filename: fivetran-users-api-openapi.yml
  format: yaml
  label: Fivetran Users API
  slug: fivetran-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fivetran/refs/heads/main/openapi/fivetran-users-api-openapi.yml
- filename: fivetran-webhooks-api-openapi.yml
  format: yaml
  label: Fivetran Webhooks API
  slug: fivetran-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fivetran/refs/heads/main/openapi/fivetran-webhooks-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Fivetran Authentication
name_suffix: Authentication
oauth_flows: []
overview: Fivetran secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Fivetran
provider_slug: fivetran
scheme_count: 1
schemes:
- description: HTTP Basic auth using `<api_key>:<api_secret>`
  name: basicAuth
  scheme: basic
  sources:
  - openapi/fivetran-openapi.yml
  type: http
slug: fivetran-authentication
source_filename: fivetran-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/fivetran-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: HTTP Basic auth using `<api_key>:<api_secret>`\n  sources:\n  - openapi/fivetran-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fivetran/refs/heads/main/authentication/fivetran-authentication.yml
summary_line: http · 1 scheme
tags:
- Connectors
- Data Integration
- Data Pipeline
- ETL
- SaaS
- Unified API
---
