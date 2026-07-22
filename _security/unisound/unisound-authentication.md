---
api_key_in:
- header
auth_types:
- apiKey
- signature
description: ''
kind: authentication
layout: security
method: searched
name: Unisound Authentication
name_suffix: Authentication
oauth_flows: []
overview: Unisound secures its APIs with apiKey and signature across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Unisound
provider_slug: unisound
scheme_count: 3
schemes:
- description: 'Unisound Token Hub API keys, created in the console under 按量计费&资源包 > API Key 管理 (pay-as-you-go / resource packs) or 订阅管理 > Token Plan (Token Plan subscriptions). Sent as Authorization: Bearer <api_key> on OpenAI-compatible and REST endpoints.'
  docs: https://maas.unisound.com/docs/guide/quickstart
  name: TokenHubBearer
  scheme: bearer
  type: http
- description: The Anthropic-compatible messages endpoint (POST /anthropic/v1/messages on maas-api.unisound.com) authenticates with the same Token Hub API key sent in the x-api-key header, mirroring the Anthropic Messages API convention.
  docs: https://maas.unisound.com/docs/api/text/anthropic-compatible
  in: header
  name: TokenHubAnthropicApiKey
  parameter: x-api-key
  type: apiKey
- description: 'The AI Open Platform WebSocket and REST APIs (ws-osasr.hivoice.cn, unigpt-api.hivoice.cn) use signature authentication: a SHA-256 digest over appkey + timestamp + secret (WebSocket ASR) or appkey + udid + timestamp + secret (UniGPT WebAPI), passed as time/appkey/sign query or body parameters. The appkey and secret are issued per product on the open platform.'
  docs: https://ai.unisound.com/doc/asronesentence/WebAPI.html
  in: query
  name: OpenPlatformSignature
  type: signature
slug: unisound-authentication
source_filename: unisound-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://maas.unisound.com/docs/guide/quickstart\ndocs: https://maas.unisound.com/docs/api/overview\nsummary:\n  types:\n  - apiKey\n  - signature\n  api_key_in:\n  - header\n  oauth2_flows: []\nschemes:\n- name: TokenHubBearer\n  type: http\n  scheme: bearer\n  description: 'Unisound Token Hub API keys, created in the console under 按量计费&资源包\n    > API Key 管理 (pay-as-you-go / resource packs) or 订阅管理 > Token Plan (Token Plan\n    subscriptions). Sent as Authorization: Bearer <api_key> on OpenAI-compatible and\n    REST endpoints.'\n  docs: https://maas.unisound.com/docs/guide/quickstart\n- name: TokenHubAnthropicApiKey\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  description: 'The Anthropic-compatible messages endpoint (POST /anthropic/v1/messages\n    on maas-api.unisound.com) authenticates with the same Token Hub API key sent in\n    the x-api-key header, mirroring the Anthropic Messages API convention.'\n  docs:\
  \ https://maas.unisound.com/docs/api/text/anthropic-compatible\n- name: OpenPlatformSignature\n  type: signature\n  in: query\n  description: 'The AI Open Platform WebSocket and REST APIs (ws-osasr.hivoice.cn,\n    unigpt-api.hivoice.cn) use signature authentication: a SHA-256 digest over appkey\n    + timestamp + secret (WebSocket ASR) or appkey + udid + timestamp + secret (UniGPT\n    WebAPI), passed as time/appkey/sign query or body parameters. The appkey and secret\n    are issued per product on the open platform.'\n  docs: https://ai.unisound.com/doc/asronesentence/WebAPI.html\nnotes:\n- No OAuth 2.0 or OpenID Connect surface is documented on either platform.\n- Token Hub warns keys must never be embedded in browser/client code and should be\n  rotated immediately if leaked.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/unisound/refs/heads/main/authentication/unisound-authentication.yml
summary_line: apiKey/signature · 3 schemes
tags:
- Company
- Artificial Intelligence
- Speech Recognition
- Text-to-Speech
- Voice Cloning
- Large Language Models
- OCR
- Healthcare
- Machine Learning
- Voice
---
