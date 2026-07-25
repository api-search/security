---
api_key_in:
- query
api_specs:
- filename: fred-categories-api-openapi.yml
  format: yaml
  label: FRED Categories API
  slug: fred-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fred/refs/heads/main/openapi/fred-categories-api-openapi.yml
- filename: fred-observations-api-openapi.yml
  format: yaml
  label: FRED Observations API
  slug: fred-observations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fred/refs/heads/main/openapi/fred-observations-api-openapi.yml
- filename: fred-regional-data-api-openapi.yml
  format: yaml
  label: FRED Regional Data API
  slug: fred-regional-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fred/refs/heads/main/openapi/fred-regional-data-api-openapi.yml
- filename: fred-releases-api-openapi.yml
  format: yaml
  label: FRED Releases API
  slug: fred-releases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fred/refs/heads/main/openapi/fred-releases-api-openapi.yml
- filename: fred-series-api-openapi.yml
  format: yaml
  label: FRED Series API
  slug: fred-series-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fred/refs/heads/main/openapi/fred-series-api-openapi.yml
- filename: fred-series-data-api-openapi.yml
  format: yaml
  label: FRED Series Data API
  slug: fred-series-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fred/refs/heads/main/openapi/fred-series-data-api-openapi.yml
- filename: fred-series-group-api-openapi.yml
  format: yaml
  label: FRED Series Group API
  slug: fred-series-group-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fred/refs/heads/main/openapi/fred-series-group-api-openapi.yml
- filename: fred-shapes-api-openapi.yml
  format: yaml
  label: FRED Shapes API
  slug: fred-shapes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fred/refs/heads/main/openapi/fred-shapes-api-openapi.yml
- filename: fred-sources-api-openapi.yml
  format: yaml
  label: FRED Sources API
  slug: fred-sources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fred/refs/heads/main/openapi/fred-sources-api-openapi.yml
- filename: fred-tags-api-openapi.yml
  format: yaml
  label: FRED Tags API
  slug: fred-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fred/refs/heads/main/openapi/fred-tags-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Fred Authentication
name_suffix: Authentication
oauth_flows: []
overview: FRED secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: FRED
provider_slug: fred
scheme_count: 1
schemes:
- description: 32-character lower-case alphanumeric FRED API key (same key used for the FRED API).
  in: query
  name: ApiKeyAuth
  parameter: api_key
  sources:
  - openapi/fred-geofred-openapi.yml
  - openapi/fred-openapi.yml
  type: apiKey
slug: fred-authentication
source_filename: fred-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/fred-geofred-openapi.yml, openapi/fred-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: query\n  parameter: api_key\n  description: 32-character lower-case alphanumeric FRED API key (same key used for the FRED\n    API).\n  sources:\n  - openapi/fred-geofred-openapi.yml\n  - openapi/fred-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fred/refs/heads/main/authentication/fred-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Finance
- Government
- Economic Data
- Federal Reserve
- Time Series
- Open Data
- Public APIs
---
