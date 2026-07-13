---
api_key_in: []
api_specs:
- filename: warner-bros-discovery-content-partner-openapi.yml
  format: yaml
  label: Warner Bros. Discovery Content Partner API
  slug: wbd-content-partner-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/warner-bros-discovery/refs/heads/main/openapi/warner-bros-discovery-content-partner-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Warner Bros Discovery Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Warner Bros. Discovery secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Warner Bros. Discovery
provider_slug: warner-bros-discovery
scheme_count: 1
schemes:
- description: OAuth 2.0 client credentials flow for partner authentication
  flows:
  - flow: clientCredentials
    scopes: 4
    tokenUrl: https://auth.warnermedia.com/oauth/token
  name: OAuth2
  sources:
  - openapi/warner-bros-discovery-content-partner-openapi.yml
  type: oauth2
slug: warner-bros-discovery-authentication
source_filename: warner-bros-discovery-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/warner-bros-discovery-content-partner-openapi.yml\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\nschemes:\n- name: OAuth2\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://auth.warnermedia.com/oauth/token\n    scopes: 4\n  description: OAuth 2.0 client credentials flow for partner authentication\n  sources:\n  - openapi/warner-bros-discovery-content-partner-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/warner-bros-discovery/refs/heads/main/authentication/warner-bros-discovery-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Entertainment
- Media
- Streaming
- Content
- Television
- Film
---
