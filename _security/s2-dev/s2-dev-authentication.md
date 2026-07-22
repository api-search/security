---
api_key_in: []
api_specs:
- filename: s2-dev-openapi-original.json
  format: json
  label: S2 Stream Store API
  slug: s2-stream-store-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/s2-dev/refs/heads/main/openapi/s2-dev-openapi-original.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: S2 Dev Authentication
name_suffix: Authentication
oauth_flows: []
overview: S2 Dev secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: S2 Dev
provider_slug: s2-dev
scheme_count: 1
schemes:
- description: 'Bearer authentication header of the form `Authorization: Bearer <token>`, where <token> is a scoped S2 access token. SDKs read S2_ACCESS_TOKEN from the environment. First use of a token on a connection adds tens of ms for verification.'
  name: access_token
  scheme: bearer
  sources:
  - openapi/s2-dev-openapi-original.json
  type: http
slug: s2-dev-authentication
source_filename: s2-dev-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: openapi/s2-dev-openapi-original.json\ndocs: https://s2.dev/docs/interface/rest\nsummary:\n  types:\n  - http\n  http_schemes:\n  - bearer\nschemes:\n- name: access_token\n  type: http\n  scheme: bearer\n  description: >-\n    Bearer authentication header of the form `Authorization: Bearer <token>`,\n    where <token> is a scoped S2 access token. SDKs read S2_ACCESS_TOKEN from\n    the environment. First use of a token on a connection adds tens of ms for\n    verification.\n  sources:\n  - openapi/s2-dev-openapi-original.json\ncapability_model:\n  description: >-\n    S2 access tokens are capability tokens, not OAuth2. A token carries an\n    AccessTokenScope constraining WHICH resources and WHICH operations it can\n    perform. There is no OAuth2 authorization/token flow and therefore no\n    scopes/ artifact.\n  scope_dimensions:\n    resource_sets: [basins, streams, access_tokens]\n    operation_groups:\n      account: [read,\
  \ write]\n      basin: [read, write]\n      stream: [read, write]\n    auto_prefix_streams: >-\n      Namespaces streams to a configured prefix; stream names are auto-prefixed\n      and the prefix is stripped on listing.\n    expiry: Optional expires_at (RFC 3339).\n  issue_operation: issue_access_token (POST /access-tokens)\n  revoke_operation: revoke_access_token (DELETE /access-tokens/{id})\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/s2-dev/refs/heads/main/authentication/s2-dev-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Streaming
- Real-Time
- Event Streaming
- Durable Storage
- Message Streaming
- Data Feeds
- Observability
- Developer Tools
- Infrastructure
---
