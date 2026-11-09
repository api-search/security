---
anonymous_access: false
api_key_in: []
api_specs:
- filename: dejavoo-openapi-generated.yml
  format: yaml
  label: Dejavoo API
  slug: dejavoo-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dejavoo/openapi/_ae-authored/dejavoo-openapi-generated.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Dejavoo Authentication
name_suffix: Authentication
oauth_flows: []
overview: Dejavoo declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: Dejavoo
provider_slug: dejavoo
scheme_count: 3
schemes:
- credentials: apiKey and secretKey issued by iPOSpays via a Dejavoo representative (devsupport@dejavoo.io / support@dejavoo.io)
  description: '"The generated transaction token is valid for up to 24 hours. You may set a shorter expiry time in the request, but the validity period cannot exceed 24 hours." A 15-minute grace period follows expiry.'
  header: token
  in: header
  issuance:
  - 'Authentication Token API: "generate a new JWT-based access token using your API Key and Secret Key"'
  - 'Merchant portal: Settings > Generate Ecom/TOP Merchant Keys > select TPN > Generate Token'
  name: token
  scopes_documented:
  - Recurring
  type: apiKey
- description: Per-TPN Register ID and Auth Key copied from iPOSpays (S.T.E.A.M -> Edit Parameters -> Integrations -> SPIn, Cloud mode), sent with SPIn requests.
  name: SPIn Register ID + Auth Key
  type: apiKey
- description: '"The Tap to Pay API provides easy programmatic access for contactless transactions, using standard REST, JSON, and Basic Authentication protocols."'
  name: Tap to Pay Basic Authentication
  scheme: basic
  type: http
slug: dejavoo-authentication
source_filename: dejavoo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: searched\nsource:\n- https://app.theneo.io/dejavoo/authentication-token/authentication\n- https://app.theneo.io/dejavoo/ipospays-api/introduction\n- https://app.theneo.io/dejavoo/recurring-payments/recurring-payments/api-docs\n- https://app.theneo.io/dejavoo/transaction-status-check/api-docs\n- https://app.theneo.io/dejavoo/spin-specification/spin-specification-api\n- https://app.theneo.io/dejavoo/developer-central/tap-to-pay-on-android\ndocs: https://app.theneo.io/dejavoo/authentication-token/authentication\nsummary: The generated contract declares no securitySchemes; this profile is read from the docs. iPOSpays APIs send a JWT access token in a `token` request header. The token is either generated in the iPOSpays merchant portal (Settings > Generate Ecom/TOP Merchant Keys, per TPN; required for iPOS Transact v1/v2) or via the Authentication Token API from an apiKey + secretKey with a scope (v3, Recurring, Management). SPIn authenticates with\
  \ a Register ID and Auth Key copied from the portal per TPN. Tap to Pay API uses Basic Authentication per its overview page.\nschemes:\n- name: token\n  type: apiKey\n  in: header\n  header: token\n  description: '\"The generated transaction token is valid for up to 24 hours. You may set a shorter expiry time in the request, but the validity period cannot exceed 24 hours.\" A 15-minute grace period follows expiry.'\n  issuance:\n  - 'Authentication Token API: \"generate a new JWT-based access token using your API Key and Secret Key\"'\n  - 'Merchant portal: Settings > Generate Ecom/TOP Merchant Keys > select TPN > Generate Token'\n  credentials: apiKey and secretKey issued by iPOSpays via a Dejavoo representative (devsupport@dejavoo.io / support@dejavoo.io)\n  scopes_documented: [Recurring]\n- name: SPIn Register ID + Auth Key\n  type: apiKey\n  description: 'Per-TPN Register ID and Auth Key copied from iPOSpays (S.T.E.A.M -> Edit Parameters -> Integrations -> SPIn, Cloud mode), sent with\
  \ SPIn requests.'\n- name: Tap to Pay Basic Authentication\n  type: http\n  scheme: basic\n  description: '\"The Tap to Pay API provides easy programmatic access for contactless transactions, using standard REST, JSON, and Basic Authentication protocols.\"'\n"
source_yaml_url: https://artifacts.apis.io/dejavoo/authentication/dejavoo-authentication.yml
summary_line: 3 schemes
tags:
- Company
- Payments
- Payment Terminals
- Point-of-Sale
- Payment Gateway
- Semi-Integration
- Fintech
- Merchant Services
---
