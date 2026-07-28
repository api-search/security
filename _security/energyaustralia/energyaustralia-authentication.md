---
api_key_in: []
api_specs:
- filename: energyaustralia-cds-energy-api-openapi.yml
  format: yaml
  label: EnergyAustralia CDR Energy Plans API
  slug: energyaustralia-cdr-energy-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/energyaustralia/refs/heads/main/openapi/energyaustralia-cds-energy-api-openapi.yml
- filename: energyaustralia-cds-common-api-openapi.yml
  format: yaml
  label: EnergyAustralia CDR Discovery Status API
  slug: energyaustralia-cdr-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/energyaustralia/refs/heads/main/openapi/energyaustralia-cds-common-api-openapi.yml
- filename: energyaustralia-cds-energy-api-openapi.yml
  format: yaml
  label: EnergyAustralia CDR Energy Consumer Data Sharing API
  slug: energyaustralia-cdr-energy-consumer-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/energyaustralia/refs/heads/main/openapi/energyaustralia-cds-energy-api-openapi.yml
auth_types:
- none
- mutualTLS
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Energyaustralia Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: EnergyAustralia secures its APIs with none, mutualTLS, oauth2, and openIdConnect across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: EnergyAustralia
provider_slug: energyaustralia
scheme_count: 3
schemes:
- description: All resource and token requests are made over mutual TLS using client transport certificates issued through the ACCC CDR Register PKI. Holder-of-key is bound to the access token per FAPI 1.0 Advanced.
  name: CDR mutual TLS
  sources:
  - https://consumerdatastandardsaustralia.github.io/standards/#security-profile
  type: mutualTLS
- description: OpenID Connect identity layer. The data holder's discovery document is published at {publicBaseUri}/.well-known/openid-configuration but is reachable only over mTLS with a CDR Register-issued certificate.
  name: CDR OpenID Connect
  openIdConnectUrl: https://authncdr.energyaustralia.com.au/.well-known/openid-configuration
  reachable_anonymously: false
  sources:
  - https://consumerdatastandardsaustralia.github.io/standards/#security-profile
  type: openIdConnect
- description: Authorization code flow with PKCE, Pushed Authorization Requests (PAR), request object signing and private_key_jwt client authentication, per the CDR Information Security profile. Access tokens are consent-scoped and sharing-duration bound.
  flows:
  - flow: authorizationCode
    scopes_ref: scopes/energyaustralia-scopes.yml
  name: CDR OAuth2 (FAPI 1.0 Advanced)
  sources:
  - https://consumerdatastandardsaustralia.github.io/standards/#security-profile
  type: oauth2
slug: energyaustralia-authentication
source_filename: energyaustralia-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: searched\nsource: >-\n  Consumer Data Standards 1.36.0 security profile, ACCC CDR Register brand entry, and\n  live probes of the EnergyAustralia CDR surfaces on 2026-07-27\ndocs: https://consumerdatastandardsaustralia.github.io/standards/#security-profile\nnote: >-\n  `derive-authentication.py` returns zero schemes for this provider: the Data Standards\n  Body CDS OpenAPI documents deliberately omit `components.securitySchemes`, because\n  authorisation is normatively specified in the separate CDR Information Security\n  profile rather than in the API contracts. This profile was therefore authored from the\n  published CDR security profile plus the live probe evidence in review.yml.\nsummary:\n  types: [none, mutualTLS, oauth2, openIdConnect]\n  api_key_in: []\n  oauth2_flows: [authorizationCode]\n  surfaces: 3\n  self_serve_signup: false\nsurfaces:\n- name: CDR Energy Plans (Product Reference Data)\n  host: https://cdr.energymadeeasy.gov.au/energyaustralia/cds-au/v1\n\
  \  auth: none\n  operations: [listEnergyPlans, getEnergyPlanDetail]\n  required_headers:\n  - name: x-v\n    required: true\n    description: >-\n      Requested payload version as a positive integer. Verified: /energy/plans answers\n      at x-v 1; /energy/plans/{planId} rejects x-v 1 with HTTP 406 and answers at x-v 3.\n  - name: x-min-v\n    required: false\n    description: Minimum acceptable payload version.\n  evidence: >-\n    GET https://cdr.energymadeeasy.gov.au/energyaustralia/cds-au/v1/energy/plans with\n    x-v 1 returned HTTP 200 anonymously on 2026-07-27 (re-verified; response carried\n    x-v 1, x-fapi-interaction-id and access-control-allow-origin *). No key, no\n    registration, no consent.\n- name: CDR Common Discovery\n  host: https://cdr.energymadeeasy.gov.au/energyaustralia/cds-au/v1\n  auth: none\n  operations: [getStatus, getOutages]\n  required_headers:\n  - name: x-v\n    required: true\n  evidence: >-\n    GET /discovery/status returned HTTP 200 with data.status\
  \ \"OK\"; GET\n    /discovery/outages returned HTTP 200 with an empty outages array (2026-07-27).\n- name: CDR Energy Consumer Data Sharing\n  host: https://authncdr.energyaustralia.com.au\n  auth: mutualTLS + oauth2 + openIdConnect\n  gated: accredited-only\n  operations:\n  - getCustomer\n  - getCustomerDetail\n  - listEnergyAccounts\n  - getEnergyAccountDetail\n  - getEnergyAccountPaymentSchedule\n  - getEnergyAccountConcessions\n  - getEnergyAccountBalance\n  - listEnergyAccountBalancesBulk\n  - listEnergyAccountBalancesSpecificAccounts\n  - getEnergyAccountInvoices\n  - listEnergyAccountInvoicesBulk\n  - listEnergyInvoicesForSpecificAccounts\n  - getBillingForEnergyAccount\n  - listEnergyAccountBillingBulk\n  - listEnergyAccountBillingForSpecificAccounts\n  - listElectricityServicePoints\n  - getElectricityServicePointDetail\n  - getElectricityServicePointUsage\n  - listElectricityUsageBulk\n  - listElectricityUsageForServicePoints\n  - getElectricityDERForServicePoint\n  - listElectricityDERBulk\n\
  \  - listElectricityDERForSpecificServicePoints\n  evidence: >-\n    ACCC CDR Register GET /cdr-register/v1/energy/data-holders/brands/summary returned\n    HTTP 200 listing EnergyAustralia (dataHolderBrandId\n    1cc7833a-b834-ed11-a832-000d3a8830d6, ABN 99086014968) with publicBaseUri\n    https://authncdr.energyaustralia.com.au. Anonymous GET of\n    https://authncdr.energyaustralia.com.au/.well-known/openid-configuration returned\n    HTTP 404 (re-verified 2026-07-27), so the live OIDC metadata is not readable without\n    accreditation.\nschemes:\n- name: CDR mutual TLS\n  type: mutualTLS\n  description: >-\n    All resource and token requests are made over mutual TLS using client transport\n    certificates issued through the ACCC CDR Register PKI. Holder-of-key is bound to the\n    access token per FAPI 1.0 Advanced.\n  sources: [https://consumerdatastandardsaustralia.github.io/standards/#security-profile]\n- name: CDR OpenID Connect\n  type: openIdConnect\n  description: >-\n \
  \   OpenID Connect identity layer. The data holder's discovery document is published at\n    {publicBaseUri}/.well-known/openid-configuration but is reachable only over mTLS\n    with a CDR Register-issued certificate.\n  openIdConnectUrl: https://authncdr.energyaustralia.com.au/.well-known/openid-configuration\n  reachable_anonymously: false\n  sources: [https://consumerdatastandardsaustralia.github.io/standards/#security-profile]\n- name: CDR OAuth2 (FAPI 1.0 Advanced)\n  type: oauth2\n  description: >-\n    Authorization code flow with PKCE, Pushed Authorization Requests (PAR), request\n    object signing and private_key_jwt client authentication, per the CDR Information\n    Security profile. Access tokens are consent-scoped and sharing-duration bound.\n  flows:\n  - flow: authorizationCode\n    scopes_ref: scopes/energyaustralia-scopes.yml\n  sources: [https://consumerdatastandardsaustralia.github.io/standards/#security-profile]\nonboarding:\n  self_serve: false\n  path: >-\n    There\
  \ is no developer signup. To read any EnergyAustralia consumer data a party must\n    be accredited by the ACCC as a Data Recipient (or operate as a CDR representative /\n    sponsored ADR under an accredited intermediary), onboard to the CDR Register, obtain\n    transport and signing certificates, register a software product, and then obtain\n    per-consumer consent through the authorisation flow.\n  docs: https://www.cdr.gov.au/\n  provider_faq: https://www.energyaustralia.com.au/home/help-support/faqs/consumer-data-right\nsecondary_data_holder:\n  name: AEMO\n  role: >-\n    Australian Energy Market Operator acts as secondary data holder for NMI standing\n    data, metering data and the DER register; the retailer proxies those requests.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/energyaustralia/refs/heads/main/authentication/energyaustralia-authentication.yml
summary_line: none/mutualTLS/oauth2/openIdConnect · 3 schemes
tags:
- Energy
- Australia
- Utilities
- Electricity
- Gas
- Energy Retailer
- Consumer Data Right
- CDR
- Product Reference Data
- Smart Metering
- Energy Markets
- Renewables
---
