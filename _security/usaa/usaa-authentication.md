---
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Usaa Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: USAA secures its APIs with oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: USAA
provider_slug: usaa
scheme_count: 2
schemes:
- description: Members grant scoped, tokenized access to an authorized third party via an OAuth 2.0 authorization flow; the third party receives a token, never USAA credentials. Aligned to the FDX API authorization model.
  name: MemberPermissionedOAuth
  scheme: authorizationCode
  sources:
  - docs
  type: oauth2
- description: The developer-facing credential is issued and managed by the chosen aggregator (Plaid client_id/secret, Mastercard Open Banking, BankSync), not by USAA. USAA exposes no direct developer API key.
  name: AggregatorApiKey
  scheme: aggregator-managed
  sources:
  - docs
  type: apiKey
slug: usaa-authentication
source_filename: usaa-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: searched\nsource: https://plaid.com/institutions/usaa/\ndocs: https://www.financialdataexchange.org/FDX/FDX/News/Spotlights/Member%20Spotlight%20USAA.aspx\nnote: >-\n  USAA publishes no first-party OpenAPI, so this profile is captured from\n  documented open-banking behavior rather than derived from a spec. Member\n  financial data is reached only through consumer-permissioned aggregators\n  (Plaid, Mastercard Open Banking, BankSync); each aggregator holds its own\n  developer credentials, and the member-facing authorization to USAA follows the\n  OAuth 2.0 / FDX tokenized pattern (no shared USAA username/password).\nsummary:\n  types: [oauth2]\n  api_key_in: []\n  oauth2_flows: [authorizationCode]\n  first_party_developer_credentials: false\n  consumer_permissioned: true\nschemes:\n- name: MemberPermissionedOAuth\n  type: oauth2\n  scheme: authorizationCode\n  description: >-\n    Members grant scoped, tokenized access to an authorized third\
  \ party via an\n    OAuth 2.0 authorization flow; the third party receives a token, never USAA\n    credentials. Aligned to the FDX API authorization model.\n  sources: [docs]\n- name: AggregatorApiKey\n  type: apiKey\n  scheme: aggregator-managed\n  description: >-\n    The developer-facing credential is issued and managed by the chosen\n    aggregator (Plaid client_id/secret, Mastercard Open Banking, BankSync), not\n    by USAA. USAA exposes no direct developer API key.\n  sources: [docs]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/usaa/refs/heads/main/authentication/usaa-authentication.yml
summary_line: oauth2 · 2 schemes
tags:
- Financial-Services
- Banking
- Insurance
- Military Finance
- Open Banking
- Open Finance
- Financial Data Exchange
- United States
- Fortune 100
---
