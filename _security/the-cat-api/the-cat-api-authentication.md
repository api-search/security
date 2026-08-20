---
api_key_in:
- header
api_specs:
- filename: the-cat-api-breeds-api-openapi.yml
  format: yaml
  label: The Cat API Breeds API
  slug: the-cat-api-breeds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/the-cat-api/refs/heads/main/openapi/the-cat-api-breeds-api-openapi.yml
- filename: the-cat-api-categories-api-openapi.yml
  format: yaml
  label: The Cat API Categories API
  slug: the-cat-api-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/the-cat-api/refs/heads/main/openapi/the-cat-api-categories-api-openapi.yml
- filename: the-cat-api-favourites-api-openapi.yml
  format: yaml
  label: The Cat API Favourites API
  slug: the-cat-api-favourites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/the-cat-api/refs/heads/main/openapi/the-cat-api-favourites-api-openapi.yml
- filename: the-cat-api-images-api-openapi.yml
  format: yaml
  label: The Cat API Images API
  slug: the-cat-api-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/the-cat-api/refs/heads/main/openapi/the-cat-api-images-api-openapi.yml
- filename: the-cat-api-votes-api-openapi.yml
  format: yaml
  label: The Cat API Votes API
  slug: the-cat-api-votes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/the-cat-api/refs/heads/main/openapi/the-cat-api-votes-api-openapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: The Cat Api Authentication
name_suffix: Authentication
oauth_flows: []
overview: The Cat API secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: The Cat API
provider_slug: the-cat-api
scheme_count: 1
schemes:
- description: API key obtained by registering at https://thecatapi.com/signup
  in: header
  name: ApiKeyHeader
  parameter: x-api-key
  sources:
  - openapi/the-cat-api-openapi.yml
  type: apiKey
slug: the-cat-api-authentication
source_filename: the-cat-api-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/the-cat-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - header\nschemes:\n- name: ApiKeyHeader\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: API key obtained by registering at https://thecatapi.com/signup\n  sources:\n  - openapi/the-cat-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/the-cat-api/refs/heads/main/authentication/the-cat-api-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Animals
- Cats
- Image
- Media
---
