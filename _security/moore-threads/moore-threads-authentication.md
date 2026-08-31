---
api_key_in: []
auth_types: []
description: 'Every public Moore Threads API surface is bearer/opaque-token authenticated. There is no OAuth 2.0 authorization server, no OpenID Connect discovery document, no scope model and no mTLS on any published surface. Two distinct token issuance paths exist and they are not interchangeable: the AIBook speech APIs issue an Access Token by human request to named Moore Threads staff, while the KUAE Cloud Coding Plan issues a self-service API Key from a console after a plan is redeemed.'
kind: authentication
layout: security
method: searched
name: Moore Threads Authentication
name_suffix: Authentication
oauth_flows: []
overview: Moore Threads declares 6 security scheme(s) across its OpenAPI definitions.
provider_name: Moore Threads
provider_slug: moore-threads
scheme_count: 6
schemes:
- api: Moore Threads AIBook Text-to-Speech API
  docs: https://docs.mthreads.com/tts/unary-tts/introduction
  format: 'Authorization: {ACCESS_TOKEN}'
  id: aibook-tts-authorization-header
  location: header
  note: The published curl sample sends the raw token in the Authorization header with no "Bearer" prefix. The streaming WebSocket variant instead carries an access_token field inside the JSON request body, documented as "not yet enforced — send the default value default_token".
  parameter: Authorization
  scheme: bearer-like
  type: http
- api: Moore Threads AIBook Text-to-Speech API
  docs: https://docs.mthreads.com/tts/stream-tts/introduction
  id: aibook-tts-stream-body-token
  location: body
  note: WebSocket /api/v2/tts/stream_generate. Docs state the field is currently inert and a literal placeholder value is accepted, which means the streaming TTS endpoint is documented as effectively unauthenticated at the protocol level.
  parameter: access_token
  type: apiKey
- api: Moore Threads AIBook Speech Recognition API
  docs: https://docs.mthreads.com/asr/recording-recognition/introduction
  format: 'Authorization: Bearer {your_access_token}'
  id: aibook-asr-bearer
  location: header
  note: The recording-file HTTP API is the only surface documenting a conventional RFC 6750 Bearer header.
  parameter: Authorization
  scheme: bearer
  type: http
- api: Moore Threads AIBook Speech Recognition API
  docs: https://docs.mthreads.com/asr/realtime-recognition/introduction
  format: wss://aibook-api.mthreads.com:62220/api/v1/asr?token=${your_token}
  id: aibook-asr-ws-query-token
  location: query
  note: Realtime ASR passes the credential in the URL query string. Tokens in URLs are logged by proxies and appear in browser/server history — a documented weakness of this surface.
  parameter: token
  type: apiKey
- api: Moore Threads AIBook Streaming Voice Conversion API
  docs: https://docs.mthreads.com/vc/stream-vc/introduction
  format: wss://aibook-api.mthreads.com:32314/api/v1/streaming_vc?token=${your_token}
  id: aibook-vc-ws-query-token
  location: query
  parameter: token
  type: apiKey
- api: KUAE Cloud Coding Plan API
  docs: https://docs.mthreads.com/kuaecloud/kuaecloud-doc-online/coding_plan/user_guide
  format: Supplied to clients as ANTHROPIC_AUTH_TOKEN (Anthropic protocol) or as the OpenAI-compatible API key. The wire header is whatever the client SDK sends; Moore Threads documents only the environment-variable name, not the header.
  id: kuae-coding-plan-api-key
  location: header
  note: Self-service. Created at https://coding-plan.kuaecloud.net/apikey after a plan is applied for or redeemed. Docs warn against embedding the key in source and recommend environment variables. An incorrect key returns a JSON error with type "Unauthorized" and code "AuthenticationError".
  parameter: Authorization / x-api-key
  type: apiKey
slug: moore-threads-authentication
source_filename: moore-threads-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: searched\nsource: https://docs.mthreads.com/asr/recording-recognition/introduction\nname: Moore Threads Authentication Profile\ndescription: >-\n  Every public Moore Threads API surface is bearer/opaque-token authenticated. There is no OAuth 2.0\n  authorization server, no OpenID Connect discovery document, no scope model and no mTLS on any\n  published surface. Two distinct token issuance paths exist and they are not interchangeable: the\n  AIBook speech APIs issue an Access Token by human request to named Moore Threads staff, while the\n  KUAE Cloud Coding Plan issues a self-service API Key from a console after a plan is redeemed.\nschemes:\n- id: aibook-tts-authorization-header\n  api: Moore Threads AIBook Text-to-Speech API\n  type: http\n  scheme: bearer-like\n  location: header\n  parameter: Authorization\n  format: 'Authorization: {ACCESS_TOKEN}'\n  note: >-\n    The published curl sample sends the raw token in the Authorization header\
  \ with no \"Bearer\"\n    prefix. The streaming WebSocket variant instead carries an access_token field inside the JSON\n    request body, documented as \"not yet enforced — send the default value default_token\".\n  docs: https://docs.mthreads.com/tts/unary-tts/introduction\n- id: aibook-tts-stream-body-token\n  api: Moore Threads AIBook Text-to-Speech API\n  type: apiKey\n  location: body\n  parameter: access_token\n  note: >-\n    WebSocket /api/v2/tts/stream_generate. Docs state the field is currently inert and a literal\n    placeholder value is accepted, which means the streaming TTS endpoint is documented as\n    effectively unauthenticated at the protocol level.\n  docs: https://docs.mthreads.com/tts/stream-tts/introduction\n- id: aibook-asr-bearer\n  api: Moore Threads AIBook Speech Recognition API\n  type: http\n  scheme: bearer\n  location: header\n  parameter: Authorization\n  format: 'Authorization: Bearer {your_access_token}'\n  note: The recording-file HTTP API is the only\
  \ surface documenting a conventional RFC 6750 Bearer header.\n  docs: https://docs.mthreads.com/asr/recording-recognition/introduction\n- id: aibook-asr-ws-query-token\n  api: Moore Threads AIBook Speech Recognition API\n  type: apiKey\n  location: query\n  parameter: token\n  format: wss://aibook-api.mthreads.com:62220/api/v1/asr?token=${your_token}\n  note: >-\n    Realtime ASR passes the credential in the URL query string. Tokens in URLs are logged by\n    proxies and appear in browser/server history — a documented weakness of this surface.\n  docs: https://docs.mthreads.com/asr/realtime-recognition/introduction\n- id: aibook-vc-ws-query-token\n  api: Moore Threads AIBook Streaming Voice Conversion API\n  type: apiKey\n  location: query\n  parameter: token\n  format: wss://aibook-api.mthreads.com:32314/api/v1/streaming_vc?token=${your_token}\n  docs: https://docs.mthreads.com/vc/stream-vc/introduction\n- id: kuae-coding-plan-api-key\n  api: KUAE Cloud Coding Plan API\n  type: apiKey\n\
  \  location: header\n  parameter: Authorization / x-api-key\n  format: >-\n    Supplied to clients as ANTHROPIC_AUTH_TOKEN (Anthropic protocol) or as the OpenAI-compatible\n    API key. The wire header is whatever the client SDK sends; Moore Threads documents only the\n    environment-variable name, not the header.\n  note: >-\n    Self-service. Created at https://coding-plan.kuaecloud.net/apikey after a plan is applied for\n    or redeemed. Docs warn against embedding the key in source and recommend environment\n    variables. An incorrect key returns a JSON error with type \"Unauthorized\" and code\n    \"AuthenticationError\".\n  docs: https://docs.mthreads.com/kuaecloud/kuaecloud-doc-online/coding_plan/user_guide\ntoken_issuance:\n- surface: AIBook speech APIs (TTS, ASR, VC)\n  model: contact-sales\n  detail: >-\n    \"访问令牌（Access Token）请联系我们获取\" — every AIBook API reference page names two Moore Threads\n    individuals as the issuance channel rather than a signup flow. There is no\
  \ self-service key page.\n  evidence: https://docs.mthreads.com/tts/unary-tts/introduction\n- surface: KUAE Cloud Coding Plan\n  model: self-service-after-purchase\n  detail: >-\n    Register on coding-plan.kuaecloud.net, claim a 30-day Free Trial or redeem a code purchased on\n    the JD storefront, then mint an API key in the console.\n  evidence: https://docs.mthreads.com/kuaecloud/kuaecloud-doc-online/coding_plan/user_guide\nnot_found:\n- oauth2\n- openid-connect\n- mutual-tls\n- api-key-rotation-policy\n- scopes\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/moore-threads/refs/heads/main/authentication/moore-threads-authentication.yml
summary_line: 6 schemes
tags:
- Company
- GPU
- Artificial Intelligence
- Machine-Learning
- Semiconductors
- Speech Recognition
- Text-to-Speech
- Voice
- LLM Inference
- Cloud Computing
- Developer Tools
- China
---
