---
api_key_in: []
auth_types:
- oauth2
description: Nuance Mix runtime services (ASRaaS, NLUaaS, DLGaaS, TTSaaS, NRaaS) and the Mix V4 authoring API authenticate with OAuth 2.0 using the client-credentials grant. Developers generate a service-credentials client (client id + secret) in the Mix dashboard, exchange it for a short-lived bearer access token at the Nuance authorization server, and present the token to the gRPC runtime over a TLS-secured channel. Access is scoped per runtime service.
kind: authentication
layout: security
method: searched
name: Nuance Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Nuance secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Nuance
provider_slug: nuance
scheme_count: 1
schemes:
- description: OAuth 2.0 client-credentials grant. The access token is presented as a Bearer credential on the gRPC call metadata; tokens are short-lived and refreshed by the client. Service credentials are created and managed in the Mix dashboard (mix.nuance.com).
  flow: clientCredentials
  grant: client_credentials
  name: MixOAuth2
  scoped_services:
  - asr
  - nlu
  - dlg
  - tts
  - nr
  sources:
  - docs.nuance.com/mix
  token_style: bearer
  type: oauth2
slug: nuance-authentication
source_filename: nuance-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://docs.nuance.com/mix/apis/\ndocs: https://docs.nuance.com/mix/\ndescription: >-\n  Nuance Mix runtime services (ASRaaS, NLUaaS, DLGaaS, TTSaaS, NRaaS) and the\n  Mix V4 authoring API authenticate with OAuth 2.0 using the client-credentials\n  grant. Developers generate a service-credentials client (client id + secret)\n  in the Mix dashboard, exchange it for a short-lived bearer access token at the\n  Nuance authorization server, and present the token to the gRPC runtime over a\n  TLS-secured channel. Access is scoped per runtime service.\nsummary:\n  types: [oauth2]\n  oauth2_flows: [clientCredentials]\n  transport: grpc-tls\nschemes:\n  - name: MixOAuth2\n    type: oauth2\n    flow: clientCredentials\n    grant: client_credentials\n    token_style: bearer\n    description: >-\n      OAuth 2.0 client-credentials grant. The access token is presented as a\n      Bearer credential on the gRPC call metadata; tokens are\
  \ short-lived and\n      refreshed by the client. Service credentials are created and managed in\n      the Mix dashboard (mix.nuance.com).\n    scoped_services: [asr, nlu, dlg, tts, nr]\n    sources: [docs.nuance.com/mix]\nnotes: >-\n  Scope tokens are assigned per runtime service in the Mix dashboard; exact\n  scope strings are managed there and were not captured verbatim (the docs are\n  a client-rendered SPA). See scopes handling in docs.nuance.com/mix/apis/.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nuance/refs/heads/main/authentication/nuance-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Company
- Speech Recognition
- Conversational AI
- Natural Language Understanding
- Text to Speech
- Speech Synthesis
- Voice
- Dialog
- gRPC
- Healthcare AI
---
