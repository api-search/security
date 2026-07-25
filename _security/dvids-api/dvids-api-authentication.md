---
api_key_in:
- query
api_specs:
- filename: dvids-api-asset-api-openapi.yml
  format: yaml
  label: DVIDS API Asset API
  slug: dvids-api-asset-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dvids-api/refs/heads/main/openapi/dvids-api-asset-api-openapi.yml
- filename: dvids-api-search-api-openapi.yml
  format: yaml
  label: DVIDS API Search API
  slug: dvids-api-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dvids-api/refs/heads/main/openapi/dvids-api-search-api-openapi.yml
- filename: dvids-api-unit-api-openapi.yml
  format: yaml
  label: DVIDS API Unit API
  slug: dvids-api-unit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dvids-api/refs/heads/main/openapi/dvids-api-unit-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Dvids Api Authentication
name_suffix: Authentication
oauth_flows: []
overview: DVIDS API secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: DVIDS API
provider_slug: dvids-api
scheme_count: 1
schemes:
- in: query
  name: apiKey
  parameter: api_key
  sources:
  - openapi/dvids-api-openapi.yml
  type: apiKey
slug: dvids-api-authentication
source_filename: dvids-api-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/dvids-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: apiKey\n  type: apiKey\n  in: query\n  parameter: api_key\n  sources:\n  - openapi/dvids-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dvids-api/refs/heads/main/authentication/dvids-api-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Media
- Defense
- Government
- Search
---
