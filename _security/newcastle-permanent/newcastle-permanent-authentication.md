---
api_key_in: []
api_specs:
- filename: newcastle-permanent-products-openapi.json
  format: json
  label: Newcastle Permanent Building Society CDR Product Reference Data API
  slug: newcastle-permanent-cds-banking-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/newcastle-permanent/refs/heads/main/openapi/newcastle-permanent-products-openapi.json
- filename: newcastle-permanent-customer-data-openapi.json
  format: json
  label: Newcastle Permanent Building Society CDR Accounts & Balances API
  slug: newcastle-permanent-cdr-accounts-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/newcastle-permanent/refs/heads/main/openapi/newcastle-permanent-customer-data-openapi.json
- filename: newcastle-permanent-customer-data-openapi.json
  format: json
  label: Newcastle Permanent Building Society CDR Transactions API
  slug: newcastle-permanent-cdr-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/newcastle-permanent/refs/heads/main/openapi/newcastle-permanent-customer-data-openapi.json
- filename: newcastle-permanent-customer-data-openapi.json
  format: json
  label: Newcastle Permanent Building Society CDR Direct Debits & Scheduled Payments API
  slug: newcastle-permanent-cdr-direct-debits-scheduled-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/newcastle-permanent/refs/heads/main/openapi/newcastle-permanent-customer-data-openapi.json
- filename: newcastle-permanent-customer-data-openapi.json
  format: json
  label: Newcastle Permanent Building Society CDR Payees API
  slug: newcastle-permanent-cdr-payees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/newcastle-permanent/refs/heads/main/openapi/newcastle-permanent-customer-data-openapi.json
- filename: newcastle-permanent-customer-data-openapi.json
  format: json
  label: Newcastle Permanent Building Society CDR Common Customer API
  slug: newcastle-permanent-cdr-common-customer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/newcastle-permanent/refs/heads/main/openapi/newcastle-permanent-customer-data-openapi.json
auth_types:
- none
- oauth2
- openIdConnect
- mutualTLS
description: ''
kind: authentication
layout: security
method: searched
name: Newcastle Permanent Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Newcastle Permanent Building Society secures its APIs with none, oauth2, openIdConnect, and mutualTLS across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Newcastle Permanent Building Society
provider_slug: newcastle-permanent
scheme_count: 4
schemes:
- name: none
  sources:
  - openapi/newcastle-permanent-cds-banking-products-openapi.yml
  tier: public-prd
  type: none
- authorizationUrl: https://openbank.newcastlepermanent.com.au/oauth2/authorize
  flow: authorizationCode
  name: cdr-oauth2
  parEndpoint: https://openbank-secure.newcastlepermanent.com.au/api/openbanking/push-authorization/par
  pkce: true
  sources:
  - https://openbank.newcastlepermanent.com.au/.well-known/openid-configuration
  tier: cdr-consumer-data-sharing
  tokenEndpointAuthMethods:
  - private_key_jwt
  tokenUrl: https://openbank-secure.newcastlepermanent.com.au/oauth2/token
  type: oauth2
- issuer: https://openbank.newcastlepermanent.com.au
  jwksUri: https://openbank.newcastlepermanent.com.au/oauth2/jwks
  name: cdr-oidc
  openIdConnectUrl: https://openbank.newcastlepermanent.com.au/.well-known/openid-configuration
  profile: FAPI
  registrationEndpoint: https://openbank-secure.newcastlepermanent.com.au/open-banking/0.2/register
  sources:
  - https://openbank.newcastlepermanent.com.au/.well-known/openid-configuration
  tier: cdr-consumer-data-sharing
  type: openIdConnect
- detail: Sender-constrained tokens per FAPI; the MTLS server host is documented in the shared CDS contract.
  name: cdr-mtls
  sources:
  - docs
  tier: cdr-consumer-data-sharing
  type: mutualTLS
slug: newcastle-permanent-authentication
source_filename: newcastle-permanent-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: https://openbank.newcastlepermanent.com.au/.well-known/openid-configuration\ndocs: https://consumerdatastandardsaustralia.github.io/standards/#security-profile\nnotes: >-\n  Newcastle Permanent is a Consumer Data Right (CDR) data holder. Its public API\n  surface has two distinct authentication tiers. The OpenAPI in this repo (the\n  shared DSB CDR Banking API v1.36.0) declares NO securitySchemes because the\n  standard defers the security profile to the CDS \"Security Profile\" and the\n  ADR/InfoSec conformance regime rather than in-spec securitySchemes. The\n  data-sharing tier below was confirmed by harvesting the bank's live OpenID\n  Connect discovery document (issuer/PAR/registration endpoints, private_key_jwt),\n  cross-referenced with the confirmed live public PRD behaviour.\nsummary:\n  tiers: [public-prd, cdr-consumer-data-sharing]\n  types: [none, oauth2, openIdConnect, mutualTLS]\n  oauth2_flows: [authorizationCode]\n\
  tiers:\n  - name: public-prd\n    scope: Product Reference Data (GET /banking/products, GET /banking/products/{productId})\n    auth: none\n    detail: >-\n      Public, unauthenticated. Confirmed live: HTTP 200 JSON with x-v: 4 and an\n      x-fapi-interaction-id. No credentials, tokens, or client registration are\n      required. An F5 web application firewall requires a browser-like User-Agent\n      and Referer to return the JSON payload (bot mitigation, not authentication).\n  - name: cdr-consumer-data-sharing\n    scope: Consumer data (accounts, balances, transactions, direct debits, scheduled payments, payees) — NOT publicly exposed\n    auth: oauth2 + openIdConnect + mutualTLS\n    security_profile: FAPI (Financial-grade API) as mandated by the CDS Security Profile\n    detail: >-\n      Access requires accreditation as a CDR Accredited Data Recipient (ADR). Uses\n      OAuth2 Authorization Code flow with PKCE, OpenID Connect (with the CDR\n      Consent + Authorisation model /\
  \ PAR + request objects), and mutual TLS for\n      sender-constrained tokens. Scopes are the standardised CDR banking scopes\n      (e.g. bank:accounts.basic:read, bank:transactions:read) governed by the DSB,\n      not bank-specific. This tier is gated by the CDR register and is not open to\n      unaccredited public callers.\nschemes:\n  - name: none\n    type: none\n    tier: public-prd\n    sources: [openapi/newcastle-permanent-cds-banking-products-openapi.yml]\n  - name: cdr-oauth2\n    type: oauth2\n    flow: authorizationCode\n    pkce: true\n    tier: cdr-consumer-data-sharing\n    authorizationUrl: https://openbank.newcastlepermanent.com.au/oauth2/authorize\n    tokenUrl: https://openbank-secure.newcastlepermanent.com.au/oauth2/token\n    parEndpoint: https://openbank-secure.newcastlepermanent.com.au/api/openbanking/push-authorization/par\n    tokenEndpointAuthMethods: [private_key_jwt]\n    sources: [https://openbank.newcastlepermanent.com.au/.well-known/openid-configuration]\n\
  \  - name: cdr-oidc\n    type: openIdConnect\n    profile: FAPI\n    tier: cdr-consumer-data-sharing\n    issuer: https://openbank.newcastlepermanent.com.au\n    openIdConnectUrl: https://openbank.newcastlepermanent.com.au/.well-known/openid-configuration\n    jwksUri: https://openbank.newcastlepermanent.com.au/oauth2/jwks\n    registrationEndpoint: https://openbank-secure.newcastlepermanent.com.au/open-banking/0.2/register\n    sources: [https://openbank.newcastlepermanent.com.au/.well-known/openid-configuration]\n  - name: cdr-mtls\n    type: mutualTLS\n    tier: cdr-consumer-data-sharing\n    detail: Sender-constrained tokens per FAPI; the MTLS server host is documented in the shared CDS contract.\n    sources: [docs]\nscopes_reference: scopes/newcastle-permanent-scopes.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/newcastle-permanent/refs/heads/main/authentication/newcastle-permanent-authentication.yml
summary_line: none/oauth2/openIdConnect/mutualTLS · 4 schemes
tags:
- Financial
- Banks
- Open Banking
- CDR
- Consumer Banking
- Building Society
- Mutual
- Australia
---
