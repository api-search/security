---
api_key_in:
- header
auth_types:
- apiKey
- oauth2
- mutualTLS
description: ''
kind: authentication
layout: security
method: searched
name: Despegarcom Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Despegar.com secures its APIs with apiKey, oauth2, and mutualTLS across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Despegar.com
provider_slug: despegarcom
scheme_count: 3
schemes:
- description: Per-partner API key required on all B2B REST endpoints (HotelDo, Decolar, AfterSales, Activities). Distinct keys exist for the test and production environments; provisioned and scoped by the Despegar team during onboarding.
  in: header
  name: ApiKey
  source: docs
  type: apiKey
- description: Used by the hosted B2B MCP servers (flights/hotels). Authentication is performed server-side; partner credentials are never exposed to the model.
  flow: clientCredentials
  name: OAuth2ClientCredentials
  source: docs
  type: oauth2
- description: Despegar's Security API documents mTLS (Mutual TLS) as a standard for securing B2B transactions.
  name: MutualTLS
  source: docs
  type: mutualTLS
slug: despegarcom-authentication
source_filename: despegarcom-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://api-docs.despegar.com/docs/security-scheme.md\ndocs: https://api-docs.despegar.com/docs/security-scheme\nsummary:\n  types: [apiKey, oauth2, mutualTLS]\n  api_key_in: [header]\n  oauth2_flows: [clientCredentials]\n  note: >-\n    The REST B2B API uses a per-partner API key provisioned by the Despegar\n    onboarding team (separate keys for test and production). The hosted MCP\n    servers use OAuth 2.0 client_credentials handled server-side. Despegar also\n    documents a Security API offering mutual TLS (mTLS) for B2B transactions.\nschemes:\n- name: ApiKey\n  type: apiKey\n  in: header\n  description: >-\n    Per-partner API key required on all B2B REST endpoints (HotelDo, Decolar,\n    AfterSales, Activities). Distinct keys exist for the test and production\n    environments; provisioned and scoped by the Despegar team during onboarding.\n  source: docs\n- name: OAuth2ClientCredentials\n  type: oauth2\n  flow: clientCredentials\n\
  \  description: >-\n    Used by the hosted B2B MCP servers (flights/hotels). Authentication is\n    performed server-side; partner credentials are never exposed to the model.\n  source: docs\n- name: MutualTLS\n  type: mutualTLS\n  description: >-\n    Despegar's Security API documents mTLS (Mutual TLS) as a standard for\n    securing B2B transactions.\n  source: docs\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/despegarcom/refs/heads/main/authentication/despegarcom-authentication.yml
summary_line: apiKey/oauth2/mutualTLS · 3 schemes
tags:
- Company
- Consumer
- Travel
- Hotels
- Flights
- Activities
- Booking
- Latin America
- B2B
- MCP
- Webhooks
---
