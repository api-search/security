---
api_key_in: []
auth_types:
- http
- token
description: ''
kind: authentication
layout: security
method: documented
name: Spire Maritime Authentication
name_suffix: Authentication
oauth_flows: []
overview: Spire Maritime secures its APIs with http and token across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Spire Maritime
provider_slug: spire-maritime
scheme_count: 2
schemes:
- bearerFormat: token
  headerName: Authorization
  in: header
  name: bearer_token
  note: 'GraphQL requests to https://api.spire.com/graphql carry an ''Authorization: Bearer <token>'' header. Tokens are issued to contract customers (enterprise / contact-sales).'
  scheme: bearer
  sources:
  - https://documentation.spire.com/maritime-2-0/
  - https://github.com/spireglobal/maritime/blob/main/spire-graphql-postman-collection.json
  type: http
- in: stream
  name: tcp_stream_token
  note: The raw TCP AIS stream (streamingv2.ais.spire.com:56784) authenticates by sending the authorization token on the socket after connecting; the same account token authorizes both GraphQL and the TCP stream. This is NOT an HTTP Authorization header - it is an application-layer token exchange over the TCP socket.
  scheme: token
  sources:
  - https://documentation.spire.com/tcp-stream-v2/using-the-tcp-stream/
  type: token
slug: spire-maritime-authentication
source_filename: spire-maritime-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-12'\nmethod: documented\nsource: https://documentation.spire.com/maritime-2-0/\nsummary:\n  types:\n  - http\n  - token\nschemes:\n- name: bearer_token\n  type: http\n  scheme: bearer\n  bearerFormat: token\n  in: header\n  headerName: Authorization\n  note: >-\n    GraphQL requests to https://api.spire.com/graphql carry an\n    'Authorization: Bearer <token>' header. Tokens are issued to\n    contract customers (enterprise / contact-sales).\n  sources:\n  - https://documentation.spire.com/maritime-2-0/\n  - https://github.com/spireglobal/maritime/blob/main/spire-graphql-postman-collection.json\n- name: tcp_stream_token\n  type: token\n  scheme: token\n  in: stream\n  note: >-\n    The raw TCP AIS stream (streamingv2.ais.spire.com:56784) authenticates by\n    sending the authorization token on the socket after connecting; the same\n    account token authorizes both GraphQL and the TCP stream. This is NOT an\n    HTTP Authorization header - it is an application-layer\
  \ token exchange over\n    the TCP socket.\n  sources:\n  - https://documentation.spire.com/tcp-stream-v2/using-the-tcp-stream/\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/spire-maritime/refs/heads/main/authentication/spire-maritime-authentication.yml
summary_line: http/token · 2 schemes
tags:
- Vessel Tracking
- AIS
- Maritime
- Satellite AIS
- Ship Tracking
- Real-Time Data
- Maritime Data
- Predicted ETA
- Port Events
- Location
- GraphQL
---
