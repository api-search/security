---
api_key_in:
- header
api_specs:
- filename: metabase-cards-api-openapi.yml
  format: yaml
  label: Metabase Cards API
  slug: metabase-cards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metabase/refs/heads/main/openapi/metabase-cards-api-openapi.yml
- filename: metabase-collections-api-openapi.yml
  format: yaml
  label: Metabase Collections API
  slug: metabase-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metabase/refs/heads/main/openapi/metabase-collections-api-openapi.yml
- filename: metabase-dashboards-api-openapi.yml
  format: yaml
  label: Metabase Dashboards API
  slug: metabase-dashboards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metabase/refs/heads/main/openapi/metabase-dashboards-api-openapi.yml
- filename: metabase-databases-api-openapi.yml
  format: yaml
  label: Metabase Databases API
  slug: metabase-databases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metabase/refs/heads/main/openapi/metabase-databases-api-openapi.yml
- filename: metabase-datasets-api-openapi.yml
  format: yaml
  label: Metabase Datasets API
  slug: metabase-datasets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metabase/refs/heads/main/openapi/metabase-datasets-api-openapi.yml
- filename: metabase-permissions-api-openapi.yml
  format: yaml
  label: Metabase Permissions API
  slug: metabase-permissions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metabase/refs/heads/main/openapi/metabase-permissions-api-openapi.yml
- filename: metabase-search-api-openapi.yml
  format: yaml
  label: Metabase Search API
  slug: metabase-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metabase/refs/heads/main/openapi/metabase-search-api-openapi.yml
- filename: metabase-sessions-api-openapi.yml
  format: yaml
  label: Metabase Sessions API
  slug: metabase-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metabase/refs/heads/main/openapi/metabase-sessions-api-openapi.yml
- filename: metabase-settings-api-openapi.yml
  format: yaml
  label: Metabase Settings API
  slug: metabase-settings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metabase/refs/heads/main/openapi/metabase-settings-api-openapi.yml
- filename: metabase-users-api-openapi.yml
  format: yaml
  label: Metabase Users API
  slug: metabase-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/metabase/refs/heads/main/openapi/metabase-users-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Metabase Authentication
name_suffix: Authentication
oauth_flows: []
overview: Metabase secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Metabase
provider_slug: metabase
scheme_count: 2
schemes:
- in: header
  name: ApiKeyAuth
  parameter: x-api-key
  sources:
  - openapi/metabase-openapi.yml
  type: apiKey
- in: header
  name: SessionAuth
  parameter: X-Metabase-Session
  sources:
  - openapi/metabase-openapi.yml
  type: apiKey
slug: metabase-authentication
source_filename: metabase-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/metabase-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  sources:\n  - openapi/metabase-openapi.yml\n- name: SessionAuth\n  type: apiKey\n  in: header\n  parameter: X-Metabase-Session\n  sources:\n  - openapi/metabase-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/metabase/refs/heads/main/authentication/metabase-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Analytics
- Business Intelligence
- Dashboards
- Data Visualization
- Open Source
- SQL
---
