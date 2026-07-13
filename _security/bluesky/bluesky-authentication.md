---
api_key_in: []
api_specs:
- filename: bluesky-openapi.yml
  format: yaml
  label: Bluesky API
  slug: bluesky-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bluesky/refs/heads/main/openapi/bluesky-openapi.yml
- filename: bluesky-asyncapi.yml
  format: yaml
  label: Bluesky Jetstream
  slug: bluesky-jetstream
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/bluesky/refs/heads/main/asyncapi/bluesky-asyncapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Bluesky Authentication
name_suffix: Authentication
oauth_flows: []
overview: Bluesky secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Bluesky
provider_slug: bluesky
scheme_count: 1
schemes:
- name: Bearer
  scheme: bearer
  sources:
  - openapi/bluesky-openapi.yml
  type: http
slug: bluesky-authentication
source_filename: bluesky-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/bluesky-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: Bearer\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/bluesky-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bluesky/refs/heads/main/authentication/bluesky-authentication.yml
summary_line: http · 1 scheme
tags:
- At-Protocol
- Decentralized
- Federated
- Open-Source
- Social Networks
- Social-Media
---
