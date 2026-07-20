---
api_key_in:
- config
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Argmax Authentication
name_suffix: Authentication
oauth_flows: []
overview: Argmax secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Argmax
provider_slug: argmax
scheme_count: 1
schemes:
- description: Argmax API key that unlocks Pro SDK features and models. For the Local Server it is passed at init time (replacing a Deepgram credential in Deepgram-compatible clients).
  in: config
  key_format: ax_***
  name: argmaxApiKey
  source: https://app.argmaxinc.com/docs/guides/using-local-server
  type: apiKey
slug: argmax-authentication
source_filename: argmax-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://app.argmaxinc.com/docs/guides/using-local-server + https://app.argmaxinc.com/docs/guides/counting-active-licenses\ndocs: https://app.argmaxinc.com/docs\nsummary:\n  types: [apiKey]\n  api_key_in: [config]\n  api_key_prefix: \"ax_\"\n  notes: >-\n    Argmax authenticates via an Argmax API key (ax_ prefix) issued from the\n    Argmax Console. The key licenses the ArgmaxSDK and, for the Local Server, is\n    supplied during server initialization rather than as a per-request HTTP\n    header. There is no documented OAuth2/OIDC surface; there is no published\n    OpenAPI, so this profile is captured from the developer docs.\nschemes:\n- name: argmaxApiKey\n  type: apiKey\n  in: config\n  key_format: \"ax_***\"\n  description: >-\n    Argmax API key that unlocks Pro SDK features and models. For the Local\n    Server it is passed at init time (replacing a Deepgram credential in\n    Deepgram-compatible clients).\n  source:\
  \ https://app.argmaxinc.com/docs/guides/using-local-server\nlicensing:\n  model: device-based\n  identifier: licenseId\n  activation: first successful initialization of ArgmaxSDK per device per calendar month\n  retrieval: \"await ArgmaxSDK.licenseInfo().licenseId\"\n  console: https://app.argmaxinc.com\n  renewal: internet connection required at least once every 30 days for license renewal\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/argmax/refs/heads/main/authentication/argmax-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Enterprise
- Artificial Intelligence
- Machine Learning
- On-Device Inference
- Speech Recognition
- Speech to Text
- Transcription
- Speaker Diarization
- Image Generation
- SDKs
- Apple Silicon
- Edge AI
---
