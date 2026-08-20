---
api_key_in:
- query
api_specs:
- filename: rasa-domain-api-openapi.yml
  format: yaml
  label: Rasa Domain API
  slug: rasa-domain-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rasa/refs/heads/main/openapi/rasa-domain-api-openapi.yml
- filename: rasa-model-api-openapi.yml
  format: yaml
  label: Rasa Model API
  slug: rasa-model-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rasa/refs/heads/main/openapi/rasa-model-api-openapi.yml
- filename: rasa-rasa-sdk-action-server-endpoint-api-openapi.yml
  format: yaml
  label: Rasa Rasa SDK Action Server Endpoint API
  slug: rasa-rasa-sdk-action-server-endpoint-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rasa/refs/heads/main/openapi/rasa-rasa-sdk-action-server-endpoint-api-openapi.yml
- filename: rasa-server-information-api-openapi.yml
  format: yaml
  label: Rasa Server Information API
  slug: rasa-server-information-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rasa/refs/heads/main/openapi/rasa-server-information-api-openapi.yml
- filename: rasa-tracker-api-openapi.yml
  format: yaml
  label: Rasa Tracker API
  slug: rasa-tracker-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rasa/refs/heads/main/openapi/rasa-tracker-api-openapi.yml
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
- Artificial Intelligence
- Conversational AI
- Chatbots
- Voice Assistants
- NLU
- LLM
- Machine-Learning
- Agents
---
