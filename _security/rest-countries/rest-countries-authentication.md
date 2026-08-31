---
api_key_in:
- query
api_specs:
- filename: rest-countries-all-api-openapi.yml
  format: yaml
  label: REST Countries All API
  slug: rest-countries-all-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rest-countries/refs/heads/main/openapi/rest-countries-all-api-openapi.yml
- filename: rest-countries-alpha-api-openapi.yml
  format: yaml
  label: REST Countries Alpha API
  slug: rest-countries-alpha-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rest-countries/refs/heads/main/openapi/rest-countries-alpha-api-openapi.yml
- filename: rest-countries-capital-api-openapi.yml
  format: yaml
  label: REST Countries Capital API
  slug: rest-countries-capital-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rest-countries/refs/heads/main/openapi/rest-countries-capital-api-openapi.yml
- filename: rest-countries-currency-api-openapi.yml
  format: yaml
  label: REST Countries Currency API
  slug: rest-countries-currency-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rest-countries/refs/heads/main/openapi/rest-countries-currency-api-openapi.yml
- filename: rest-countries-demonym-api-openapi.yml
  format: yaml
  label: REST Countries Demonym API
  slug: rest-countries-demonym-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rest-countries/refs/heads/main/openapi/rest-countries-demonym-api-openapi.yml
- filename: rest-countries-independent-api-openapi.yml
  format: yaml
  label: REST Countries Independent API
  slug: rest-countries-independent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rest-countries/refs/heads/main/openapi/rest-countries-independent-api-openapi.yml
- filename: rest-countries-language-api-openapi.yml
  format: yaml
  label: REST Countries Language API
  slug: rest-countries-language-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rest-countries/refs/heads/main/openapi/rest-countries-language-api-openapi.yml
- filename: rest-countries-name-api-openapi.yml
  format: yaml
  label: REST Countries Name API
  slug: rest-countries-name-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rest-countries/refs/heads/main/openapi/rest-countries-name-api-openapi.yml
- filename: rest-countries-region-api-openapi.yml
  format: yaml
  label: REST Countries Region API
  slug: rest-countries-region-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rest-countries/refs/heads/main/openapi/rest-countries-region-api-openapi.yml
- filename: rest-countries-subregion-api-openapi.yml
  format: yaml
  label: REST Countries Subregion API
  slug: rest-countries-subregion-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rest-countries/refs/heads/main/openapi/rest-countries-subregion-api-openapi.yml
- filename: rest-countries-translation-api-openapi.yml
  format: yaml
  label: REST Countries Translation API
  slug: rest-countries-translation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rest-countries/refs/heads/main/openapi/rest-countries-translation-api-openapi.yml
- filename: rest-countries-countries-api-openapi.yml
  format: yaml
  label: REST Countries Countries API
  slug: rest-countries-countries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rest-countries/refs/heads/main/openapi/rest-countries-countries-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Rest Countries Authentication
name_suffix: Authentication
oauth_flows: []
overview: REST Countries secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: REST Countries
provider_slug: rest-countries
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
slug: rest-countries-authentication
source_filename: rest-countries-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/restcountries-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - query\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Bearer token authentication. Obtain your API key from https://restcountries.com.\n    A demo key `rc_live_demo` is available for testing.\n  sources:\n  - openapi/restcountries-openapi.yml\n- name: apiKeyQuery\n  type: apiKey\n  in: query\n  parameter: api-key\n  description: API key passed as a query parameter (less secure)\n  sources:\n  - openapi/restcountries-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rest-countries/refs/heads/main/authentication/rest-countries-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Countries
- Geocoding
- Geography
- ISO 3166
- Open-Source
- Public APIs
- Reference Data
- Currency
- Language
- Capitals
- Regions
- Subregions
- Translations
---
