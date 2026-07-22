---
api_key_in:
- query
api_specs:
- filename: rasa-http-api-openapi.yml
  format: yaml
  label: Rasa HTTP API
  slug: rasa-http-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rasa/refs/heads/main/openapi/rasa-http-api-openapi.yml
- filename: rasa-action-server-openapi.yml
  format: yaml
  label: Rasa SDK Action Server
  slug: rasa-sdk-action-server
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rasa/refs/heads/main/openapi/rasa-action-server-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Rasa Authentication
name_suffix: Authentication
oauth_flows: []
overview: Rasa secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Rasa
provider_slug: rasa
scheme_count: 2
schemes:
- description: A plaintext token to secure your server, specified at startup in the argument `--auth-token thisismysecret`
  in: query
  name: TokenAuth
  parameter: token
  sources:
  - openapi/rasa-http-api-openapi.yml
  type: apiKey
- bearerFormat: JWT
  description: "A JWT token that is signed using the JWT secret specified at startup in the argument `--jwt-secret thisismysecret`,\nusing the `HS256` algorithm.\n\nThe token's payload must contain an object under the `user` key,\nwhich in turn must contain the `username` and `role` attributes.\nThe following is an example payload for a JWT token:\n\n```json\n{\n    \"user\": {\n        \"username\": \"<sender_id>\",\n        \"ro"
  name: JWT
  scheme: bearer
  sources:
  - openapi/rasa-http-api-openapi.yml
  type: http
slug: rasa-authentication
source_filename: rasa-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: derived\nsource: openapi/rasa-http-api-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - query\nschemes:\n- name: TokenAuth\n  type: apiKey\n  in: query\n  parameter: token\n  description: A plaintext token to secure your server, specified at startup in the argument\n    `--auth-token thisismysecret`\n  sources:\n  - openapi/rasa-http-api-openapi.yml\n- name: JWT\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: |-\n    A JWT token that is signed using the JWT secret specified at startup in the argument `--jwt-secret thisismysecret`,\n    using the `HS256` algorithm.\n\n    The token's payload must contain an object under the `user` key,\n    which in turn must contain the `username` and `role` attributes.\n    The following is an example payload for a JWT token:\n\n    ```json\n    {\n        \"user\": {\n            \"username\": \"<sender_id>\",\n            \"ro\n  sources:\n  - openapi/rasa-http-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rasa/refs/heads/main/authentication/rasa-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- Ai
- Conversational AI
- Chatbots
- Voice Assistants
- NLU
- LLM
- Machine Learning
- Agents
---
