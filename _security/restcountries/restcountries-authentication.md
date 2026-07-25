---
api_key_in:
- query
api_specs:
- filename: restcountries-countries-api-openapi.yml
  format: yaml
  label: REST Countries Countries API
  slug: restcountries-countries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/restcountries/refs/heads/main/openapi/restcountries-countries-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Restcountries Authentication
name_suffix: Authentication
oauth_flows: []
overview: REST Countries secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: REST Countries
provider_slug: restcountries
scheme_count: 2
schemes:
- description: Bearer token authentication. Obtain your API key from https://restcountries.com. A demo key `rc_live_demo` is available for testing.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/restcountries-openapi.yml
  type: http
- description: API key passed as a query parameter (less secure)
  in: query
  name: apiKeyQuery
  parameter: api-key
  sources:
  - openapi/restcountries-openapi.yml
  type: apiKey
slug: restcountries-authentication
source_filename: restcountries-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/restcountries-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - query\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Bearer token authentication. Obtain your API key from https://restcountries.com.\n    A demo key `rc_live_demo` is available for testing.\n  sources:\n  - openapi/restcountries-openapi.yml\n- name: apiKeyQuery\n  type: apiKey\n  in: query\n  parameter: api-key\n  description: API key passed as a query parameter (less secure)\n  sources:\n  - openapi/restcountries-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/restcountries/refs/heads/main/authentication/restcountries-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Countries
- Geography
- World Data
- Flags
- Currencies
- Languages
- Population
---
