---
api_key_in: []
api_specs:
- filename: amadeus-media-hotel-content-openapi.yaml
  format: yaml
  label: Hotel Content API
  slug: hotel-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amadeus-media/refs/heads/main/openapi/amadeus-media-hotel-content-openapi.yaml
- filename: amadeus-media-hotel-list-openapi.yaml
  format: yaml
  label: Hotel List API
  slug: hotel-list-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amadeus-media/refs/heads/main/openapi/amadeus-media-hotel-list-openapi.yaml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Amadeus Media Authentication
name_suffix: Authentication
oauth_flows: []
overview: Amadeus Media secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Amadeus Media
provider_slug: amadeus-media
scheme_count: 1
schemes:
- description: OAuth2 Bearer token. Obtain a token using the Amadeus Authorization API at https://test.api.amadeus.com/v1/security/oauth2/token.
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/amadeus-media-hotel-content-openapi.yaml
  type: http
slug: amadeus-media-authentication
source_filename: amadeus-media-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/amadeus-media-hotel-content-openapi.yaml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  description: OAuth2 Bearer token. Obtain a token using the Amadeus Authorization API at https://test.api.amadeus.com/v1/security/oauth2/token.\n  sources:\n  - openapi/amadeus-media-hotel-content-openapi.yaml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amadeus-media/refs/heads/main/authentication/amadeus-media-authentication.yml
summary_line: http · 1 scheme
tags:
- Content
- Hotels
- Images
- Media
- Travel
---
