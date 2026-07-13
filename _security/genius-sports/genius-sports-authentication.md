---
api_key_in:
- header
api_specs:
- filename: swagger-latest.json
  format: json
  label: Genius Sports Fixtures API v2
  slug: fixtures-api-v2
  spec_type: OpenAPI
  url: https://explorer.api.geniussports.com/Fixtures/v2/Production/swagger-latest.json
- filename: swagger-latest.json
  format: json
  label: Genius Sports Matching API v2
  slug: matching-api-v2
  spec_type: OpenAPI
  url: https://explorer.api.geniussports.com/fixtures-matching/v2/Production/swagger-latest.json
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Genius Sports Authentication
name_suffix: Authentication
oauth_flows: []
overview: Genius Sports secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Genius Sports
provider_slug: genius-sports
scheme_count: 2
schemes:
- in: header
  name: Auth0
  parameter: Authorization
  sources:
  - openapi/genius-sports-fixtures-v2-openapi.yml
  - openapi/genius-sports-matching-v2-openapi.yml
  type: apiKey
- in: header
  name: api_key
  parameter: x-api-key
  sources:
  - openapi/genius-sports-fixtures-v2-openapi.yml
  - openapi/genius-sports-matching-v2-openapi.yml
  - openapi/genius-sports-openapi.yml
  type: apiKey
slug: genius-sports-authentication
source_filename: genius-sports-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/genius-sports-fixtures-v2-openapi.yml, openapi/genius-sports-matching-v2-openapi.yml,\n  openapi/genius-sports-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: Auth0\n  type: apiKey\n  in: header\n  parameter: Authorization\n  sources:\n  - openapi/genius-sports-fixtures-v2-openapi.yml\n  - openapi/genius-sports-matching-v2-openapi.yml\n- name: api_key\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  sources:\n  - openapi/genius-sports-fixtures-v2-openapi.yml\n  - openapi/genius-sports-matching-v2-openapi.yml\n  - openapi/genius-sports-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/genius-sports/refs/heads/main/authentication/genius-sports-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Sports
- Statistics
- Live Data
- Fixtures
---
