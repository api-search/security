---
api_key_in:
- message-body
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Picfinder Authentication
name_suffix: Authentication
oauth_flows: []
overview: PicFinder secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: PicFinder
provider_slug: picfinder
scheme_count: 1
schemes:
- environment_param: ENVIRONMENT
  environments:
  - PRODUCTION
  - DEVELOPMENT
  in: message-body
  name: apiKey
  sources:
  - https://www.npmjs.com/package/picfinder-sdk
  type: apiKey
slug: picfinder-authentication
source_filename: picfinder-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://www.npmjs.com/package/picfinder-sdk\ndocs: https://picfinder.ai/support/en/collections/7944924-picfinder-api\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - message-body\n  transport: websocket\n  notes: >-\n    The PicFinder API is a persistent WebSocket connection to\n    wss://ws-api.diffusionmaster.com. The client obtains an API key by\n    requesting API access through the PicFinder support portal, then supplies\n    the key (plus an ENVIRONMENT of PRODUCTION or DEVELOPMENT) when\n    instantiating the SDK. The SDK opens the WebSocket and authenticates the\n    session with the API key over the connection; there is no OAuth or scope\n    surface. No published OpenAPI/Swagger document exists — the protocol is\n    documented via the first-party picfinder-sdk.\nschemes:\n- name: apiKey\n  type: apiKey\n  in: message-body\n  environment_param: ENVIRONMENT\n  environments:\n  - PRODUCTION\n  - DEVELOPMENT\n  sources:\n\
  \  - https://www.npmjs.com/package/picfinder-sdk\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/picfinder/refs/heads/main/authentication/picfinder-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Artificial Intelligence
- Machine Learning
- Image Generation
- Generative AI
- Text to Image
- Image to Image
- Developer Tools
- SDK
- WebSocket
---
