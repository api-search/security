---
api_key_in:
- header
auth_types:
- http-bearer
- apiKey
description: SuperOps GraphQL APIs authenticate with a personal API token passed as an HTTP Bearer token, combined with a mandatory CustomerSubDomain header that identifies the tenant. There is no OAuth 2.0 / OpenID Connect flow; the token is generated in the SuperOps app and a tenant may hold only one active token at a time.
kind: authentication
layout: security
method: searched
name: Superops Authentication
name_suffix: Authentication
oauth_flows: []
overview: SuperOps secures its APIs with http-bearer and apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: SuperOps
provider_slug: superops
scheme_count: 2
schemes:
- description: Personal API token generated at Settings > My Profile > API token tab. Only one token can be active per user at a time; regenerating invalidates the old token.
  format: Bearer <API_TOKEN>
  header: Authorization
  in: header
  name: BearerToken
  scheme: bearer
  sources:
  - docs
  type: http
- description: Mandatory tenant identifier header. The value is the MSP subdomain found at Settings > MSP Information under My MSP. Every request must send both the Authorization and CustomerSubDomain headers.
  header: CustomerSubDomain
  in: header
  name: CustomerSubDomain
  sources:
  - docs
  type: apiKey
slug: superops-authentication
source_filename: superops-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://support.superops.com/en/articles/6632215-how-to-integrate-applications-using-superops-ai-graphql-apis\ndocs: https://support.superops.com/en/collections/3666305-api-documentation\ndescription: >-\n  SuperOps GraphQL APIs authenticate with a personal API token passed as an\n  HTTP Bearer token, combined with a mandatory CustomerSubDomain header that\n  identifies the tenant. There is no OAuth 2.0 / OpenID Connect flow; the token\n  is generated in the SuperOps app and a tenant may hold only one active token\n  at a time.\nsummary:\n  types: [http-bearer, apiKey]\n  oauth2_flows: []\n  api_key_in: [header]\nschemes:\n- name: BearerToken\n  type: http\n  scheme: bearer\n  in: header\n  header: Authorization\n  format: 'Bearer <API_TOKEN>'\n  description: >-\n    Personal API token generated at Settings > My Profile > API token tab. Only\n    one token can be active per user at a time; regenerating invalidates the old\n\
  \    token.\n  sources: [docs]\n- name: CustomerSubDomain\n  type: apiKey\n  in: header\n  header: CustomerSubDomain\n  description: >-\n    Mandatory tenant identifier header. The value is the MSP subdomain found at\n    Settings > MSP Information under My MSP. Every request must send both the\n    Authorization and CustomerSubDomain headers.\n  sources: [docs]\ntoken_management:\n  location: Settings > My Profile > API token tab\n  one_active_token: true\n  invalid_token_error: 'HTTP 401 — \"The API token used is invalid or deleted.\"'\n  invalid_subdomain_error: 'HTTP 400 — invalid subdomain provided'\nendpoints:\n- surface: msp\n  us: https://api.superops.ai/msp\n  eu: https://euapi.superops.ai/msp\n- surface: it\n  us: https://api.superops.ai/it\n  eu: https://euapi.superops.ai/it\nnotes:\n  - Requests use UTC timezone with ISO date format, e.g. 2022-04-10T10:15:30.\n  - Rate limit is 800 requests per minute (see rate-limits/superops-rate-limits.yml).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/superops/refs/heads/main/authentication/superops-authentication.yml
summary_line: http-bearer/apiKey · 2 schemes
tags:
- Company
- It Management Software
- PSA
- RMM
- MSP
- Service Desk
- Endpoint Management
- IT Documentation
- GraphQL
---
