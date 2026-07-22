---
api_key_in:
- body
api_specs:
- filename: zkme-openapi.yml
  format: yaml
  label: zkMe Protocol API
  slug: zkme-protocol-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zkme/refs/heads/main/openapi/zkme-openapi.yml
auth_types:
- apiKey
- bearerToken
description: The zkMe Open API authenticates every request with an AppID + API key pair issued from the zkMe dashboard. Unusually, the credentials are passed as request-body fields (mchNo = AppID, apiKey = API key) rather than as an Authorization header, so they are not expressible as a standard OpenAPI securityScheme. The zkKYB endpoint and all SDK-initialized flows instead use a short-lived accessToken (valid 30 minutes) minted server-side via POST https://nest-api.zk.me/api/token/get.
kind: authentication
layout: security
method: searched
name: Zkme Authentication
name_suffix: Authentication
oauth_flows: []
overview: zkMe secures its APIs with apiKey and bearerToken across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: zkMe
provider_slug: zkme
scheme_count: 2
schemes:
- applies_to:
  - zkKYC
  - zkOBS
  - KYT
  description: AppID (mchNo) + API key, both from the dashboard, sent in the JSON body.
  fields:
  - mchNo
  - apiKey
  in: body
  name: apiKeyPair
  sources:
  - openapi/zkme-openapi.yml
  type: apiKey
- applies_to:
  - zkKYB
  - widget
  description: Short-lived token obtained during SDK integration; used by zkKYB and widget flows.
  field: accessToken
  in: body
  mint_endpoint: https://nest-api.zk.me/api/token/get
  name: accessToken
  sources:
  - openapi/zkme-openapi.yml
  ttl_seconds: 1800
  type: bearerToken
slug: zkme-authentication
source_filename: zkme-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://docs.zk.me/hub/start/onboarding/integration/api\ndocs: https://docs.zk.me/hub/start/onboarding/integration/api\ndescription: >-\n  The zkMe Open API authenticates every request with an AppID + API key pair\n  issued from the zkMe dashboard. Unusually, the credentials are passed as\n  request-body fields (mchNo = AppID, apiKey = API key) rather than as an\n  Authorization header, so they are not expressible as a standard OpenAPI\n  securityScheme. The zkKYB endpoint and all SDK-initialized flows instead use a\n  short-lived accessToken (valid 30 minutes) minted server-side via\n  POST https://nest-api.zk.me/api/token/get.\nsummary:\n  types: [apiKey, bearerToken]\n  api_key_in: [body]\n  credential_pair: [mchNo, apiKey]\nschemes:\n  - name: apiKeyPair\n    type: apiKey\n    in: body\n    fields: [mchNo, apiKey]\n    description: AppID (mchNo) + API key, both from the dashboard, sent in the JSON body.\n    applies_to:\
  \ [zkKYC, zkOBS, KYT]\n    sources: [openapi/zkme-openapi.yml]\n  - name: accessToken\n    type: bearerToken\n    in: body\n    field: accessToken\n    ttl_seconds: 1800\n    mint_endpoint: https://nest-api.zk.me/api/token/get\n    description: Short-lived token obtained during SDK integration; used by zkKYB and widget flows.\n    applies_to: [zkKYB, widget]\n    sources: [openapi/zkme-openapi.yml]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zkme/refs/heads/main/authentication/zkme-authentication.yml
summary_line: apiKey/bearerToken · 2 schemes
tags:
- Company
- Crypto Web3
- Identity
- KYC
- KYB
- Compliance
- Zero Knowledge
- Decentralized Identity
- Anti-Sybil
- Transaction Monitoring
---
