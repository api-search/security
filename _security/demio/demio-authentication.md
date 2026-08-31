---
api_key_in:
- header
- query
api_specs:
- filename: demio-events-api-openapi.yml
  format: yaml
  label: Demio Events API
  slug: demio-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/demio/refs/heads/main/openapi/demio-events-api-openapi.yml
- filename: demio-intro-api-openapi.yml
  format: yaml
  label: Demio Intro API
  slug: demio-intro-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/demio/refs/heads/main/openapi/demio-intro-api-openapi.yml
- filename: demio-reports-api-openapi.yml
  format: yaml
  label: Demio Reports API
  slug: demio-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/demio/refs/heads/main/openapi/demio-reports-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Demio Authentication
name_suffix: Authentication
oauth_flows: []
overview: Demio secures its APIs with apiKey across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Demio
provider_slug: demio
scheme_count: 4
schemes:
- description: Account API Key, from Demio Settings > API.
  in: header
  name: ApiKeyHeader
  parameter: Api-Key
  sources:
  - openapi/demio-openapi.yml
  type: apiKey
- description: Account API Secret, from Demio Settings > API.
  in: header
  name: ApiSecretHeader
  parameter: Api-Secret
  sources:
  - openapi/demio-openapi.yml
  type: apiKey
- description: Account API Key supplied on the query string.
  in: query
  name: ApiKeyQuery
  parameter: api_key
  sources:
  - openapi/demio-openapi.yml
  type: apiKey
- description: Account API Secret supplied on the query string.
  in: query
  name: ApiSecretQuery
  parameter: api_secret
  sources:
  - openapi/demio-openapi.yml
  type: apiKey
slug: demio-authentication
source_filename: demio-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: derived\nsource: openapi/demio-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\n  - query\nschemes:\n- name: ApiKeyHeader\n  type: apiKey\n  in: header\n  parameter: Api-Key\n  description: Account API Key, from Demio Settings > API.\n  sources:\n  - openapi/demio-openapi.yml\n- name: ApiSecretHeader\n  type: apiKey\n  in: header\n  parameter: Api-Secret\n  description: Account API Secret, from Demio Settings > API.\n  sources:\n  - openapi/demio-openapi.yml\n- name: ApiKeyQuery\n  type: apiKey\n  in: query\n  parameter: api_key\n  description: Account API Key supplied on the query string.\n  sources:\n  - openapi/demio-openapi.yml\n- name: ApiSecretQuery\n  type: apiKey\n  in: query\n  parameter: api_secret\n  description: Account API Secret supplied on the query string.\n  sources:\n  - openapi/demio-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/demio/refs/heads/main/authentication/demio-authentication.yml
summary_line: apiKey · 4 schemes
tags:
- Company
- Webinars
- Virtual Events
- Event Management
- Marketing
- Marketing Technology
- Demand Generation
- Video
- Engagement Marketing
- Lead Generation
- Software-as-a-Service
---
