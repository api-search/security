---
api_key_in:
- header
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Idwall Authentication
name_suffix: Authentication
oauth_flows: []
overview: IDwall secures its APIs with apiKey across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: IDwall
provider_slug: idwall
scheme_count: 1
schemes:
- description: Per-account API token. Obtained from https://dashboard.idwall.co/api-integration (menu "Integração da API"). Sent on every request in the Authorization header.
  in: header
  name: apiToken
  parameter_name: Authorization
  sources:
  - docs.idwall.co/reference/por-onde-comecar
  token_source: https://dashboard.idwall.co/api-integration
  type: apiKey
slug: idwall-authentication
source_filename: idwall-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://docs.idwall.co/docs/api-how-to-use\ndocs: https://docs.idwall.co/reference/por-onde-comecar\nsummary:\n  types: [apiKey]\n  api_key_in: [header]\n  api_key_name: Authorization\n  oauth2_flows: []\n  notes: >-\n    IDwall uses a single per-account API authentication token passed in the\n    Authorization request header. The token is issued from the account\n    dashboard (Integração da API) and is only available to users granted the\n    \"Escrita API\" permission. There is no OAuth flow and no public sandbox\n    environment; a contracted token always runs against production.\nschemes:\n  - name: apiToken\n    type: apiKey\n    in: header\n    parameter_name: Authorization\n    description: >-\n      Per-account API token. Obtained from https://dashboard.idwall.co/api-integration\n      (menu \"Integração da API\"). Sent on every request in the Authorization header.\n    token_source: https://dashboard.idwall.co/api-integration\n\
  \    sources: [docs.idwall.co/reference/por-onde-comecar]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/idwall/refs/heads/main/authentication/idwall-authentication.yml
summary_line: apiKey · 1 scheme
tags:
- Company
- Identity Verification
- KYC
- Fraud Prevention
- Background Checks
- Document Verification
- Compliance
- Onboarding
- Brazil
---
