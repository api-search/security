---
api_key_in:
- query
api_specs:
- filename: mediastack-openapi.yml
  format: yaml
  label: Mediastack News API
  slug: mediastack-news-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mediastack/refs/heads/main/openapi/mediastack-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Mediastack Authentication
name_suffix: Authentication
oauth_flows: []
overview: Mediastack secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Mediastack
provider_slug: mediastack
scheme_count: 1
schemes:
- description: 'Mediastack uses a single static API access key passed as a query parameter

    (`access_key=YOUR_KEY`). Keys are issued from the mediastack dashboard.'
  in: query
  name: ApiKeyAuth
  parameter: access_key
  sources:
  - openapi/mediastack-openapi.yml
  type: apiKey
slug: mediastack-authentication
source_filename: mediastack-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/mediastack-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - query\nschemes:\n- name: ApiKeyAuth\n  type: apiKey\n  in: query\n  parameter: access_key\n  description: |-\n    Mediastack uses a single static API access key passed as a query parameter\n    (`access_key=YOUR_KEY`). Keys are issued from the mediastack dashboard.\n  sources:\n  - openapi/mediastack-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mediastack/refs/heads/main/authentication/mediastack-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- News
- News Aggregation
- Media
- Apilayer
- Public APIs
---
