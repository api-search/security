---
api_key_in:
- header
api_specs:
- filename: apis-io-apis-api-openapi.yml
  format: yaml
  label: APIs.io APIs API
  slug: apis-io-apis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apis-io/refs/heads/main/openapi/apis-io-apis-api-openapi.yml
- filename: apis-io-areas-api-openapi.yml
  format: yaml
  label: APIs.io Areas API
  slug: apis-io-areas-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apis-io/refs/heads/main/openapi/apis-io-areas-api-openapi.yml
- filename: apis-io-artifact-types-api-openapi.yml
  format: yaml
  label: APIs.io Artifact Types API
  slug: apis-io-artifact-types-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apis-io/refs/heads/main/openapi/apis-io-artifact-types-api-openapi.yml
- filename: apis-io-industries-api-openapi.yml
  format: yaml
  label: APIs.io Industries API
  slug: apis-io-industries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apis-io/refs/heads/main/openapi/apis-io-industries-api-openapi.yml
- filename: apis-io-insights-api-openapi.yml
  format: yaml
  label: APIs.io Insights API
  slug: apis-io-insights-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apis-io/refs/heads/main/openapi/apis-io-insights-api-openapi.yml
- filename: apis-io-providers-api-openapi.yml
  format: yaml
  label: APIs.io Providers API
  slug: apis-io-providers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apis-io/refs/heads/main/openapi/apis-io-providers-api-openapi.yml
- filename: apis-io-ratings-api-openapi.yml
  format: yaml
  label: APIs.io Ratings API
  slug: apis-io-ratings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apis-io/refs/heads/main/openapi/apis-io-ratings-api-openapi.yml
- filename: apis-io-regions-api-openapi.yml
  format: yaml
  label: APIs.io Regions API
  slug: apis-io-regions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apis-io/refs/heads/main/openapi/apis-io-regions-api-openapi.yml
- filename: apis-io-search-api-openapi.yml
  format: yaml
  label: APIs.io Search API
  slug: apis-io-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apis-io/refs/heads/main/openapi/apis-io-search-api-openapi.yml
- filename: apis-io-synthesis-api-openapi.yml
  format: yaml
  label: APIs.io Synthesis API
  slug: apis-io-synthesis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apis-io/refs/heads/main/openapi/apis-io-synthesis-api-openapi.yml
- filename: apis-io-tags-api-openapi.yml
  format: yaml
  label: APIs.io Tags API
  slug: apis-io-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/apis-io/refs/heads/main/openapi/apis-io-tags-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Apis Io Authentication
name_suffix: Authentication
oauth_flows: []
overview: APIs.io secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: APIs.io
provider_slug: apis-io
scheme_count: 2
schemes:
- in: header
  name: api_key
  parameter: x-api-key
  sources:
  - openapi/apis-io-search-openapi.yaml
  type: apiKey
- description: Optional in v1. Defined so metering/rate-tiers can be enabled later without a breaking change.
  in: header
  name: ApiKeyAuth
  parameter: X-API-Key
  sources:
  - openapi/apis-io-v1-openapi.yml
  type: apiKey
slug: apis-io-authentication
source_filename: apis-io-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/apis-io-search-openapi.yaml, openapi/apis-io-v1-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: api_key\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  sources:\n  - openapi/apis-io-search-openapi.yaml\n- name: ApiKeyAuth\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: Optional in v1. Defined so metering/rate-tiers can be enabled later without a\n    breaking change.\n  sources:\n  - openapi/apis-io-v1-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/apis-io/refs/heads/main/authentication/apis-io-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- API Aggregation
- API Directory
- API Discovery
- API Indexing
- API Rating
- API Search
- APIs.json
- Search Engine
---
