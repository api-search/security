---
api_key_in: []
api_specs:
- filename: bannerbear-animated-gifs-api-openapi.yml
  format: yaml
  label: Bannerbear Animated GIFs API
  slug: bannerbear-animated-gifs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bannerbear/refs/heads/main/openapi/bannerbear-animated-gifs-api-openapi.yml
- filename: bannerbear-auth-api-openapi.yml
  format: yaml
  label: Bannerbear Auth API
  slug: bannerbear-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bannerbear/refs/heads/main/openapi/bannerbear-auth-api-openapi.yml
- filename: bannerbear-collections-api-openapi.yml
  format: yaml
  label: Bannerbear Collections API
  slug: bannerbear-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bannerbear/refs/heads/main/openapi/bannerbear-collections-api-openapi.yml
- filename: bannerbear-fonts-api-openapi.yml
  format: yaml
  label: Bannerbear Fonts API
  slug: bannerbear-fonts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bannerbear/refs/heads/main/openapi/bannerbear-fonts-api-openapi.yml
- filename: bannerbear-images-api-openapi.yml
  format: yaml
  label: Bannerbear Images API
  slug: bannerbear-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bannerbear/refs/heads/main/openapi/bannerbear-images-api-openapi.yml
- filename: bannerbear-screenshots-api-openapi.yml
  format: yaml
  label: Bannerbear Screenshots API
  slug: bannerbear-screenshots-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bannerbear/refs/heads/main/openapi/bannerbear-screenshots-api-openapi.yml
- filename: bannerbear-templates-api-openapi.yml
  format: yaml
  label: Bannerbear Templates API
  slug: bannerbear-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bannerbear/refs/heads/main/openapi/bannerbear-templates-api-openapi.yml
- filename: bannerbear-videos-api-openapi.yml
  format: yaml
  label: Bannerbear Videos API
  slug: bannerbear-videos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bannerbear/refs/heads/main/openapi/bannerbear-videos-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Bannerbear Authentication
name_suffix: Authentication
oauth_flows: []
overview: Bannerbear secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Bannerbear
provider_slug: bannerbear
scheme_count: 1
schemes:
- description: Project or master API key passed as a Bearer token.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/bannerbear-openapi.yml
  type: http
slug: bannerbear-authentication
source_filename: bannerbear-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/bannerbear-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Project or master API key passed as a Bearer token.\n  sources:\n  - openapi/bannerbear-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bannerbear/refs/heads/main/authentication/bannerbear-authentication.yml
summary_line: http · 1 scheme
tags:
- Image-Generation
- Video Generation
- Templates
- Media
- Automation
---
