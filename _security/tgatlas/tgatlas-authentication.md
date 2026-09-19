---
anonymous_access: false
api_key_in: []
api_specs:
- filename: tgatlas-openapi.json
  format: json
  label: ChannelIndex Telegram Channel Data API
  slug: channelindex-telegram-channel-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tgatlas/refs/heads/main/openapi/tgatlas-openapi.json
auth_types: []
description: Authentication is delegated entirely to the RapidAPI marketplace gateway. The base OpenAPI document leaves securitySchemes empty on purpose (the gateway injects and validates credentials), and the provider's published overlay declares the two headers a generated client must send. There is no OAuth, no OpenID Connect and no per-request signing; a single subscriber key issued by RapidAPI (free tier, no card) authenticates every one of the 19 GET routes.
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Tgatlas Authentication
name_suffix: Authentication
oauth_flows: []
overview: ChannelIndex (tgAtlas) declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: ChannelIndex (tgAtlas)
provider_slug: tgatlas
scheme_count: 2
schemes:
- description: Subscriber key from RapidAPI. The free plan issues one without a card. Also accepted as x-rapidapi-key.
  id: RapidAPIKey
  in: header
  name: X-RapidAPI-Key
  required: true
  type: apiKey
- description: Host the key is scoped to. Both headers are required together on every request.
  id: RapidAPIHost
  in: header
  name: X-RapidAPI-Host
  required: true
  type: apiKey
  value: telegram155.p.rapidapi.com
slug: tgatlas-authentication
source_filename: tgatlas-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-16'\nmethod: searched\nsource: >-\n  https://channelindex.starnikovoleg.workers.dev/overlay.yaml (provider-published\n  Overlay declaring the two gateway headers) + https://channelindex.starnikovoleg.workers.dev/docs\nprovider: tgAtlas\napi: tgAtlas Telegram Channel Data API\ndescription: >-\n  Authentication is delegated entirely to the RapidAPI marketplace gateway. The\n  base OpenAPI document leaves securitySchemes empty on purpose (the gateway\n  injects and validates credentials), and the provider's published overlay\n  declares the two headers a generated client must send. There is no OAuth, no\n  OpenID Connect and no per-request signing; a single subscriber key issued by\n  RapidAPI (free tier, no card) authenticates every one of the 19 GET routes.\nsummary:\n  styles:\n    - apiKey\n  oauth2: false\n  openid_connect: false\n  mutual_tls: false\n  scope_model: none\nschemes:\n  - id: RapidAPIKey\n    type: apiKey\n    in: header\n    name: X-RapidAPI-Key\n\
  \    required: true\n    description: >-\n      Subscriber key from RapidAPI. The free plan issues one without a card.\n      Also accepted as x-rapidapi-key.\n  - id: RapidAPIHost\n    type: apiKey\n    in: header\n    name: X-RapidAPI-Host\n    required: true\n    value: telegram155.p.rapidapi.com\n    description: >-\n      Host the key is scoped to. Both headers are required together on every\n      request.\napplied_to: all 19 operations (gateway-enforced; not encoded per-operation in the base spec)\nsignup: https://rapidapi.com/starnikovoleg/api/telegram155\nnotes: >-\n  Because credentials are gateway headers rather than a spec-declared security\n  scheme, the base openapi.json cannot be used to generate a working client\n  as-is; the provider's overlay/tgatlas-overlay.yaml supplies the missing\n  securitySchemes and a security requirement so generated clients authenticate\n  without hand edits.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tgatlas/refs/heads/main/authentication/tgatlas-authentication.yml
summary_line: 2 schemes
tags:
- Telegram
- Public Channels
- Social-Media
- Social Monitoring
- Messaging
- Directory
- Search
- Analytics
- OSINT
- Market Research
- AI-agent context
---
