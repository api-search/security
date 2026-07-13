---
api_key_in: []
api_specs:
- filename: peopledatalabs-openapi.yml
  format: yaml
  label: People Data Labs Person Enrichment API
  slug: peopledatalabs-person-enrichment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/peopledatalabs/refs/heads/main/openapi/peopledatalabs-openapi.yml
- filename: peopledatalabs-openapi.yml
  format: yaml
  label: People Data Labs Person Search API
  slug: peopledatalabs-person-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/peopledatalabs/refs/heads/main/openapi/peopledatalabs-openapi.yml
- filename: peopledatalabs-openapi.yml
  format: yaml
  label: People Data Labs Company Enrichment API
  slug: peopledatalabs-company-enrichment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/peopledatalabs/refs/heads/main/openapi/peopledatalabs-openapi.yml
- filename: peopledatalabs-openapi.yml
  format: yaml
  label: People Data Labs Company Search API
  slug: peopledatalabs-company-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/peopledatalabs/refs/heads/main/openapi/peopledatalabs-openapi.yml
- filename: peopledatalabs-openapi.yml
  format: yaml
  label: People Data Labs Cleaner and Enrichment Utilities API
  slug: peopledatalabs-cleaner-utilities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/peopledatalabs/refs/heads/main/openapi/peopledatalabs-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Peopledatalabs Authentication
name_suffix: Authentication
oauth_flows: []
overview: People Data Labs secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: People Data Labs
provider_slug: peopledatalabs
scheme_count: 1
schemes:
- description: People Data Labs authenticates every request with an API key issued in the PDL dashboard. The key is passed in the X-Api-Key request header. The key can also be supplied as an api_key query-string parameter, but the header is the recommended method. All requests must be made over HTTPS.
  in: header
  name: APIKeyHeader
  parameterName: X-Api-Key
  sources:
  - openapi/peopledatalabs-openapi.yml
  - https://docs.peopledatalabs.com/docs/authentication
  type: apiKey
slug: peopledatalabs-authentication
source_filename: peopledatalabs-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/peopledatalabs-openapi.yml\nsummary:\n  types:\n  - apiKey\nschemes:\n- name: APIKeyHeader\n  type: apiKey\n  in: header\n  parameterName: X-Api-Key\n  description: >-\n    People Data Labs authenticates every request with an API key issued in the\n    PDL dashboard. The key is passed in the X-Api-Key request header. The key can\n    also be supplied as an api_key query-string parameter, but the header is the\n    recommended method. All requests must be made over HTTPS.\n  sources:\n  - openapi/peopledatalabs-openapi.yml\n  - https://docs.peopledatalabs.com/docs/authentication\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/peopledatalabs/refs/heads/main/authentication/peopledatalabs-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Data Enrichment
- Web Intelligence
- Person Data
- Company Data
- B2B Data
- Contact Discovery
- Reference Data
- Firmographics
- Identity Resolution
---
