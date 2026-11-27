---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: israbase-com-companies-api-openapi.yml
  format: yaml
  label: IsraBase Companies API
  slug: israbase-com-companies-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/israbase-com/openapi/israbase-com-companies-api-openapi.yml
- filename: israbase-com-company-api-openapi.yml
  format: yaml
  label: IsraBase Company API
  slug: israbase-com-company-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/israbase-com/openapi/israbase-com-company-api-openapi.yml
- filename: israbase-com-marketplace-api-openapi.yml
  format: yaml
  label: IsraBase Marketplace API
  slug: israbase-com-marketplace-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/israbase-com/openapi/israbase-com-marketplace-api-openapi.yml
- filename: israbase-com-nonprofit-api-openapi.yml
  format: yaml
  label: IsraBase Nonprofit API
  slug: israbase-com-nonprofit-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/israbase-com/openapi/israbase-com-nonprofit-api-openapi.yml
- filename: israbase-com-partnership-api-openapi.yml
  format: yaml
  label: IsraBase Partnership API
  slug: israbase-com-partnership-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/israbase-com/openapi/israbase-com-partnership-api-openapi.yml
- filename: israbase-com-search-api-openapi.yml
  format: yaml
  label: IsraBase Search API
  slug: israbase-com-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/israbase-com/openapi/israbase-com-search-api-openapi.yml
- filename: israbase-com-stats-api-openapi.yml
  format: yaml
  label: IsraBase Stats API
  slug: israbase-com-stats-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/israbase-com/openapi/israbase-com-stats-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: derived
name: IsraBase Authentication
name_suffix: Authentication
oauth_flows: []
overview: IsraBase secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: IsraBase
provider_slug: israbase-com
scheme_count: 2
schemes:
- description: Optional free API key. An invalid key returns 401.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/israbase-com-openapi.yml
  type: http
- description: Optional API key. Same key as bearerAuth.
  in: header
  name: apiKeyHeader
  parameter: X-API-Key
  sources:
  - openapi/israbase-com-openapi.yml
  type: apiKey
slug: israbase-com-authentication
source_filename: israbase-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-13'\nmethod: derived\nsource: openapi/israbase-com-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Optional free API key. An invalid key returns 401.\n  sources:\n  - openapi/israbase-com-openapi.yml\n- name: apiKeyHeader\n  type: apiKey\n  in: header\n  parameter: X-API-Key\n  description: Optional API key. Same key as bearerAuth.\n  sources:\n  - openapi/israbase-com-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/israbase-com/authentication/israbase-com-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Data
- Israel
- Companies
- Registry
- Open Data
---
