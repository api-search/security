---
api_key_in: []
api_specs:
- filename: aisstream-asyncapi.yml
  format: yaml
  label: AISStream AIS Stream API
  slug: aisstream-ais-stream-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/aisstream/refs/heads/main/asyncapi/aisstream-asyncapi.yml
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: derived
name: Aisstream Authentication
name_suffix: Authentication
oauth_flows: []
overview: AISStream secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: AISStream
provider_slug: aisstream
scheme_count: 1
schemes:
- description: A single free API key obtained by registering at https://aisstream.io/. The key is placed in the `APIKey` field of the JSON subscription message sent over the open WebSocket (wss://stream.aisstream.io/v0/stream). It is NOT an HTTP header, bearer token, or OAuth flow - AISStream carries the credential inside the WebSocket message payload. A subscription message (with the key) must be sent within 3 seconds of connecting or the server closes the socket.
  fieldName: APIKey
  in: message
  name: api_key_in_payload
  sources:
  - https://aisstream.io/documentation
  - https://github.com/aisstream/ais-message-models
  type: apiKey
slug: aisstream-authentication
source_filename: aisstream-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-12'\nmethod: derived\nsource: asyncapi/aisstream-asyncapi.yml + https://aisstream.io/documentation\nsummary:\n  types:\n  - apiKey\nschemes:\n- name: api_key_in_payload\n  type: apiKey\n  in: message\n  fieldName: APIKey\n  description: >-\n    A single free API key obtained by registering at https://aisstream.io/. The\n    key is placed in the `APIKey` field of the JSON subscription message sent\n    over the open WebSocket (wss://stream.aisstream.io/v0/stream). It is NOT an\n    HTTP header, bearer token, or OAuth flow - AISStream carries the credential\n    inside the WebSocket message payload. A subscription message (with the key)\n    must be sent within 3 seconds of connecting or the server closes the socket.\n  sources:\n  - https://aisstream.io/documentation\n  - https://github.com/aisstream/ais-message-models\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aisstream/refs/heads/main/authentication/aisstream-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Vessel Tracking
- AIS
- Maritime
- Ship Tracking
- Real-Time Data
- WebSocket
- Streaming
- Ships
- Maritime Data
- Location
---
