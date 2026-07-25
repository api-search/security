---
api_key_in:
- header
api_specs:
- filename: sorsa-community-api-openapi.yml
  format: yaml
  label: Sorsa Community API
  slug: sorsa-community-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sorsa/refs/heads/main/openapi/sorsa-community-api-openapi.yml
- filename: sorsa-lists-api-openapi.yml
  format: yaml
  label: Sorsa Lists API
  slug: sorsa-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sorsa/refs/heads/main/openapi/sorsa-lists-api-openapi.yml
- filename: sorsa-search-api-openapi.yml
  format: yaml
  label: Sorsa Search API
  slug: sorsa-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sorsa/refs/heads/main/openapi/sorsa-search-api-openapi.yml
- filename: sorsa-sorsa-info-crypto-related-api-openapi.yml
  format: yaml
  label: Sorsa Sorsa Info Crypto Related API
  slug: sorsa-sorsa-info-crypto-related-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sorsa/refs/heads/main/openapi/sorsa-sorsa-info-crypto-related-api-openapi.yml
- filename: sorsa-technical-endpoints-api-openapi.yml
  format: yaml
  label: Sorsa Technical Endpoints API
  slug: sorsa-technical-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sorsa/refs/heads/main/openapi/sorsa-technical-endpoints-api-openapi.yml
- filename: sorsa-tweets-api-openapi.yml
  format: yaml
  label: Sorsa Tweets API
  slug: sorsa-tweets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sorsa/refs/heads/main/openapi/sorsa-tweets-api-openapi.yml
- filename: sorsa-users-data-api-openapi.yml
  format: yaml
  label: Sorsa Users Data API
  slug: sorsa-users-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sorsa/refs/heads/main/openapi/sorsa-users-data-api-openapi.yml
- filename: sorsa-verification-api-openapi.yml
  format: yaml
  label: Sorsa Verification API
  slug: sorsa-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sorsa/refs/heads/main/openapi/sorsa-verification-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Sorsa Authentication
name_suffix: Authentication
oauth_flows: []
overview: Sorsa secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Sorsa
provider_slug: sorsa
scheme_count: 1
schemes:
- description: Include your API key in the `ApiKey` header with every request.
  in: header
  name: ApiKey
  parameter: ApiKey
  sources:
  - openapi/sorsa-openapi.yml
  type: apiKey
slug: sorsa-authentication
source_filename: sorsa-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/sorsa-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKey\n  type: apiKey\n  in: header\n  parameter: ApiKey\n  description: Include your API key in the `ApiKey` header with every request.\n  sources:\n  - openapi/sorsa-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sorsa/refs/heads/main/authentication/sorsa-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Twitter
- X
- Social Media
- Data Extraction
- Real-Time
---
