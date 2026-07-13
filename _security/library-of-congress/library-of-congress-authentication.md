---
api_key_in:
- query
api_specs:
- filename: library-of-congress-loc-gov-json-api-openapi.yml
  format: yaml
  label: Library of Congress loc.gov JSON API
  slug: loc-gov-json-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/library-of-congress/refs/heads/main/openapi/library-of-congress-loc-gov-json-api-openapi.yml
- filename: library-of-congress-chronicling-america-api-openapi.yml
  format: yaml
  label: Library of Congress Chronicling America API
  slug: chronicling-america-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/library-of-congress/refs/heads/main/openapi/library-of-congress-chronicling-america-api-openapi.yml
- filename: library-of-congress-congress-gov-api-openapi.yml
  format: yaml
  label: Library of Congress Congress.gov API
  slug: congress-gov-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/library-of-congress/refs/heads/main/openapi/library-of-congress-congress-gov-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Library Of Congress Authentication
name_suffix: Authentication
oauth_flows: []
overview: Library of Congress secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Library of Congress
provider_slug: library-of-congress
scheme_count: 1
schemes:
- in: query
  name: ApiKeyAuth
  parameter: api_key
  sources:
  - openapi/library-of-congress-congress-gov-api-openapi.yml
  type: apiKey
slug: library-of-congress-authentication
source_filename: library-of-congress-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/library-of-congress-congress-gov-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: query\n  parameter: api_key\n  sources:\n  - openapi/library-of-congress-congress-gov-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/library-of-congress/refs/heads/main/authentication/library-of-congress-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Cultural Heritage
- Federal Government
- Library
- Legislative
- Newspapers
- Search
---
