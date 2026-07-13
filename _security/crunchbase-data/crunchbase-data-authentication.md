---
api_key_in: []
api_specs:
- filename: crunchbase-data-openapi.yml
  format: yaml
  label: Crunchbase Entity Lookup API
  slug: crunchbase-data-entity-lookup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crunchbase-data/refs/heads/main/openapi/crunchbase-data-openapi.yml
- filename: crunchbase-data-openapi.yml
  format: yaml
  label: Crunchbase Search API
  slug: crunchbase-data-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crunchbase-data/refs/heads/main/openapi/crunchbase-data-openapi.yml
- filename: crunchbase-data-openapi.yml
  format: yaml
  label: Crunchbase Autocomplete API
  slug: crunchbase-data-autocomplete-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crunchbase-data/refs/heads/main/openapi/crunchbase-data-openapi.yml
- filename: crunchbase-data-openapi.yml
  format: yaml
  label: Crunchbase Deleted Entities API
  slug: crunchbase-data-deleted-entities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crunchbase-data/refs/heads/main/openapi/crunchbase-data-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Crunchbase Data Authentication
name_suffix: Authentication
oauth_flows: []
overview: Crunchbase secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Crunchbase
provider_slug: crunchbase-data
scheme_count: 2
schemes:
- description: API key passed as the user_key query parameter, e.g. ?user_key=YOUR_API_KEY. Issued with a Crunchbase Enterprise, Applications, or Basic license.
  in: query
  name: userKeyQuery
  parameter: user_key
  sources:
  - openapi/crunchbase-data-openapi.yml
  - https://data.crunchbase.com/docs/using-the-api
  type: apiKey
- description: API key passed as the X-cb-user-key request header. Preferred over the query parameter to avoid leaking the key in logs and URLs.
  in: header
  name: userKeyHeader
  parameter: X-cb-user-key
  sources:
  - openapi/crunchbase-data-openapi.yml
  - https://data.crunchbase.com/docs/using-the-api
  type: apiKey
slug: crunchbase-data-authentication
source_filename: crunchbase-data-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/crunchbase-data-openapi.yml\nsummary:\n  types:\n  - apiKey\nschemes:\n- name: userKeyQuery\n  type: apiKey\n  in: query\n  parameter: user_key\n  description: >-\n    API key passed as the user_key query parameter, e.g.\n    ?user_key=YOUR_API_KEY. Issued with a Crunchbase Enterprise, Applications,\n    or Basic license.\n  sources:\n  - openapi/crunchbase-data-openapi.yml\n  - https://data.crunchbase.com/docs/using-the-api\n- name: userKeyHeader\n  type: apiKey\n  in: header\n  parameter: X-cb-user-key\n  description: >-\n    API key passed as the X-cb-user-key request header. Preferred over the\n    query parameter to avoid leaking the key in logs and URLs.\n  sources:\n  - openapi/crunchbase-data-openapi.yml\n  - https://data.crunchbase.com/docs/using-the-api\nnotes: >-\n  All requests must use HTTPS; non-HTTPS calls return HTTP 426. API keys are\n  license-gated - full API access requires a Crunchbase Enterprise\
  \ or\n  Applications license, with a reduced Basic API for Crunchbase Basic plan\n  holders. There is no OAuth or user-delegated flow; access is a single\n  account-level API key.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/crunchbase-data/refs/heads/main/authentication/crunchbase-data-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Company Data
- Web Intelligence
- Funding Data
- Firmographics
- B2B Data
- Investor Data
- Reference Data
- Fortune 1000
---
