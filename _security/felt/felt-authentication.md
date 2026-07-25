---
api_key_in: []
api_specs:
- filename: felt-comments-api-openapi.yml
  format: yaml
  label: Felt Comments API
  slug: felt-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/felt/refs/heads/main/openapi/felt-comments-api-openapi.yml
- filename: felt-elements-api-openapi.yml
  format: yaml
  label: Felt Elements API
  slug: felt-elements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/felt/refs/heads/main/openapi/felt-elements-api-openapi.yml
- filename: felt-embed-tokens-api-openapi.yml
  format: yaml
  label: Felt Embed Tokens API
  slug: felt-embed-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/felt/refs/heads/main/openapi/felt-embed-tokens-api-openapi.yml
- filename: felt-layer-exports-api-openapi.yml
  format: yaml
  label: Felt Layer Exports API
  slug: felt-layer-exports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/felt/refs/heads/main/openapi/felt-layer-exports-api-openapi.yml
- filename: felt-layer-library-api-openapi.yml
  format: yaml
  label: Felt Layer Library API
  slug: felt-layer-library-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/felt/refs/heads/main/openapi/felt-layer-library-api-openapi.yml
- filename: felt-layer-uploads-api-openapi.yml
  format: yaml
  label: Felt Layer Uploads API
  slug: felt-layer-uploads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/felt/refs/heads/main/openapi/felt-layer-uploads-api-openapi.yml
- filename: felt-layers-api-openapi.yml
  format: yaml
  label: Felt Layers API
  slug: felt-layers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/felt/refs/heads/main/openapi/felt-layers-api-openapi.yml
- filename: felt-maps-api-openapi.yml
  format: yaml
  label: Felt Maps API
  slug: felt-maps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/felt/refs/heads/main/openapi/felt-maps-api-openapi.yml
- filename: felt-projects-api-openapi.yml
  format: yaml
  label: Felt Projects API
  slug: felt-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/felt/refs/heads/main/openapi/felt-projects-api-openapi.yml
- filename: felt-sources-api-openapi.yml
  format: yaml
  label: Felt Sources API
  slug: felt-sources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/felt/refs/heads/main/openapi/felt-sources-api-openapi.yml
- filename: felt-users-api-openapi.yml
  format: yaml
  label: Felt Users API
  slug: felt-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/felt/refs/heads/main/openapi/felt-users-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Felt Authentication
name_suffix: Authentication
oauth_flows: []
overview: Felt secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Felt
provider_slug: felt
scheme_count: 1
schemes:
- bearerFormat: YOUR_API_KEY
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/felt-felt-rest-api-openapi.yml
  type: http
slug: felt-authentication
source_filename: felt-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/felt-felt-rest-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: YOUR_API_KEY\n  sources:\n  - openapi/felt-felt-rest-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/felt/refs/heads/main/authentication/felt-authentication.yml
summary_line: http · 1 scheme
tags:
- Maps
- GIS
- Geospatial
- Collaborative
- Mapping
- Layers
- Embedding
---
