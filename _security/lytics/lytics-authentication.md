---
api_key_in:
- header
- query
api_specs:
- filename: lytics-accounts-api-openapi.yml
  format: yaml
  label: Lytics Accounts API
  slug: lytics-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lytics/refs/heads/main/openapi/lytics-accounts-api-openapi.yml
- filename: lytics-connections-api-openapi.yml
  format: yaml
  label: Lytics Connections API
  slug: lytics-connections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lytics/refs/heads/main/openapi/lytics-connections-api-openapi.yml
- filename: lytics-datamodels-api-openapi.yml
  format: yaml
  label: Lytics Datamodels API
  slug: lytics-datamodels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lytics/refs/heads/main/openapi/lytics-datamodels-api-openapi.yml
- filename: lytics-entity-api-openapi.yml
  format: yaml
  label: Lytics Entity API
  slug: lytics-entity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lytics/refs/heads/main/openapi/lytics-entity-api-openapi.yml
- filename: lytics-jobs-api-openapi.yml
  format: yaml
  label: Lytics Jobs API
  slug: lytics-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lytics/refs/heads/main/openapi/lytics-jobs-api-openapi.yml
- filename: lytics-segments-api-openapi.yml
  format: yaml
  label: Lytics Segments API
  slug: lytics-segments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lytics/refs/heads/main/openapi/lytics-segments-api-openapi.yml
- filename: lytics-work-api-openapi.yml
  format: yaml
  label: Lytics Work API
  slug: lytics-work-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lytics/refs/heads/main/openapi/lytics-work-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Lytics Authentication
name_suffix: Authentication
oauth_flows: []
overview: Lytics secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Lytics
provider_slug: lytics
scheme_count: 2
schemes:
- description: Lytics API key passed as a query parameter. Obtain your API key from the Lytics account settings.
  in: query
  name: ApiKeyQuery
  parameter: key
  sources:
  - openapi/lytics-rest-api-openapi.yml
  type: apiKey
- description: Lytics API key passed as an Authorization header value.
  in: header
  name: ApiKeyHeader
  parameter: Authorization
  sources:
  - openapi/lytics-rest-api-openapi.yml
  type: apiKey
slug: lytics-authentication
source_filename: lytics-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/lytics-rest-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  - query\nschemes:\n- name: ApiKeyQuery\n  type: apiKey\n  in: query\n  parameter: key\n  description: Lytics API key passed as a query parameter. Obtain your API key from the Lytics\n    account settings.\n  sources:\n  - openapi/lytics-rest-api-openapi.yml\n- name: ApiKeyHeader\n  type: apiKey\n  in: header\n  parameter: Authorization\n  description: Lytics API key passed as an Authorization header value.\n  sources:\n  - openapi/lytics-rest-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lytics/refs/heads/main/authentication/lytics-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Customer Data Platform
- CDP
- Personalization
- Segmentation
- User Profiles
- Behavioral Analytics
- Content Affinity
- Real-Time Data
- Marketing Automation
- Audience Activation
---
