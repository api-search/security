---
api_key_in: []
api_specs:
- filename: yelp-ai-api-openapi.yml
  format: yaml
  label: Yelp AI API
  slug: yelp-ai-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yelp/refs/heads/main/openapi/yelp-ai-api-openapi.yml
- filename: yelp-businesses-api-openapi.yml
  format: yaml
  label: Yelp Businesses API
  slug: yelp-businesses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yelp/refs/heads/main/openapi/yelp-businesses-api-openapi.yml
- filename: yelp-categories-api-openapi.yml
  format: yaml
  label: Yelp Categories API
  slug: yelp-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yelp/refs/heads/main/openapi/yelp-categories-api-openapi.yml
- filename: yelp-events-api-openapi.yml
  format: yaml
  label: Yelp Events API
  slug: yelp-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yelp/refs/heads/main/openapi/yelp-events-api-openapi.yml
- filename: yelp-reviews-api-openapi.yml
  format: yaml
  label: Yelp Reviews API
  slug: yelp-reviews-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yelp/refs/heads/main/openapi/yelp-reviews-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Yelp Authentication
name_suffix: Authentication
oauth_flows: []
overview: Yelp secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Yelp
provider_slug: yelp
scheme_count: 1
schemes:
- description: Yelp Fusion API key passed as a bearer token in the Authorization header.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/yelp-openapi.yml
  type: http
slug: yelp-authentication
source_filename: yelp-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/yelp-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Yelp Fusion API key passed as a bearer token in the Authorization header.\n  sources:\n  - openapi/yelp-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/yelp/refs/heads/main/authentication/yelp-authentication.yml
summary_line: http · 1 scheme
tags:
- Restaurant
- Local Search
- Reviews
- Business Data
- Location
---
