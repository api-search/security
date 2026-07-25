---
api_key_in:
- header
auth_types:
- http-bearer-apikey
description: Authentication model for the Forta GraphQL API. Requests are authenticated with a Bearer API key in the HTTP Authorization header. API keys are created in the Forta App (app.forta.network) after signing in with a wallet; up to 10 keys per account, and a key cannot be recovered once lost. For local bot development the key can be stored in forta.config.json under `fortaApiKey`. This is a static API-key (bearer) scheme, not OAuth 2.0 / OIDC, so there is no scope surface.
kind: authentication
layout: security
method: searched
name: Forta Authentication
name_suffix: Authentication
oauth_flows: []
overview: Forta secures its APIs with http-bearer-apikey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Forta
provider_slug: forta
scheme_count: 1
schemes:
- example: "curl POST --header \"Authorization: Bearer <api_key>\" \\\n  --header \"content-type: application/json\" \\\n  --url \"https://api.forta.network/graphql\"\n"
  format: Bearer <api_key>
  header: Authorization
  in: header
  key_management: https://docs.forta.network/en/latest/api-keys/
  name: BearerApiKey
  provisioning: Sign into the Forta App with a wallet, open "My API Keys", "Create new API key" (max 10). Keys are not recoverable if lost.
  scheme: bearer
  sources:
  - https://docs.forta.network/en/latest/api-keys/
  type: http
slug: forta-authentication
source_filename: forta-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://docs.forta.network/en/latest/api-keys/\ndocs: https://docs.forta.network/en/latest/api-keys/\ndescription: >-\n  Authentication model for the Forta GraphQL API. Requests are authenticated\n  with a Bearer API key in the HTTP Authorization header. API keys are created\n  in the Forta App (app.forta.network) after signing in with a wallet; up to 10\n  keys per account, and a key cannot be recovered once lost. For local bot\n  development the key can be stored in forta.config.json under `fortaApiKey`.\n  This is a static API-key (bearer) scheme, not OAuth 2.0 / OIDC, so there is no\n  scope surface.\nsummary:\n  types: [http-bearer-apikey]\n  api_key_in: [header]\n  oauth2_flows: []\nschemes:\n- name: BearerApiKey\n  type: http\n  scheme: bearer\n  in: header\n  header: Authorization\n  format: 'Bearer <api_key>'\n  key_management: https://docs.forta.network/en/latest/api-keys/\n  provisioning: >-\n    Sign into the Forta\
  \ App with a wallet, open \"My API Keys\", \"Create new API\n    key\" (max 10). Keys are not recoverable if lost.\n  example: |\n    curl POST --header \"Authorization: Bearer <api_key>\" \\\n      --header \"content-type: application/json\" \\\n      --url \"https://api.forta.network/graphql\"\n  sources: [https://docs.forta.network/en/latest/api-keys/]\nnotes: >-\n  GraphQL API access requires a paid plan. Bot-to-scanner and\n  scanner-to-network communication in the node software uses JWT tokens (the\n  SDKs expose generate/verify JWT helpers) — that is a separate, node-internal\n  trust model from the developer-facing API key documented here.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/forta/refs/heads/main/authentication/forta-authentication.yml
summary_line: http-bearer-apikey · 1 scheme
tags:
- Company
- Security
- Blockchain
- Web3
- Monitoring
- Threat Detection
- DeFi
- GraphQL
- Alerts
- Smart Contracts
---
