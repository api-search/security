---
api_key_in: []
api_specs:
- filename: powershop-cdr-energy-api-openapi.json
  format: json
  label: Powershop CDR Generic Tariff (Energy Plans) API
  slug: powershop-cdr-generic-tariff-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/powershop/refs/heads/main/openapi/powershop-cdr-energy-api-openapi.json
- filename: powershop-cdr-common-api-openapi.json
  format: json
  label: Powershop CDR Discovery API
  slug: powershop-cdr-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/powershop/refs/heads/main/openapi/powershop-cdr-common-api-openapi.json
- filename: powershop-cdr-energy-api-openapi.json
  format: json
  label: Powershop CDR Energy Consumer Data API
  slug: powershop-cdr-energy-consumer-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/powershop/refs/heads/main/openapi/powershop-cdr-energy-api-openapi.json
auth_types:
- oauth2
- openIdConnect
- mutualTLS
description: ''
kind: authentication
layout: security
method: searched
name: Powershop Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Powershop secures its APIs with oauth2, openIdConnect, and mutualTLS across 0 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Powershop
provider_slug: powershop
scheme_count: 0
schemes: []
slug: powershop-authentication
source_filename: powershop-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: searched\nsource: >-\n  openapi/powershop-cdr-energy-api-openapi.json +\n  openapi/powershop-cdr-common-api-openapi.json (no securitySchemes declared) and\n  the DSB Consumer Data Standards security profile\ndocs: https://consumerdatastandardsaustralia.github.io/standards/#security-profile\nsummary:\n  types: [oauth2, openIdConnect, mutualTLS]\n  api_key_in: []\n  oauth2_flows: [authorizationCode]\n  note: >-\n    Powershop's API surface is split cleanly in two, and the two halves have\n    opposite auth models. The public half — the CDS Discovery endpoints on\n    Powershop's own registered host, and the Generic Tariff (plan) endpoints the\n    Australian Energy Regulator serves on Powershop's behalf — requires NO\n    authentication at all: no API key, no registration, no terms click-through.\n    The only mandatory request signalling is the CDS x-v version header. The\n    consented half — accounts, balances, invoices, billing, payment schedules,\n\
  \    concessions, service points, usage and DER — is reachable only by an ACCC\n    accredited data recipient holding a valid consumer consent, over the CDR\n    Register's mutual-TLS-secured infrastructure.\nschemes: []\nschemes_note: >-\n  Neither Data Standards Body OpenAPI document declares components.securitySchemes\n  and no operation declares security[]. The CDR authorisation model is specified\n  out-of-band in the Consumer Data Standards security profile rather than inline\n  in the API definitions, so a mechanical derive over the specs yields zero\n  schemes. The profile below was captured from the published standards, not\n  invented.\nsurfaces:\n- name: CDS Discovery (Powershop's own registered CDR host)\n  base_url: https://public.cdr.powershop.com.au/cds-au/v1\n  authenticated: false\n  credential: none\n  required_headers:\n  - {name: x-v, required: true, description: 'CDS endpoint version. Confirmed live: omitting it returns HTTP 400 urn:au-cds:error:cds-all:Header/Missing\
  \ with detail \"x-v header is mandatory for CDR endpoint requests\".'}\n  - {name: x-min-v, required: false, description: Minimum acceptable endpoint version.}\n  operations: [getStatus, getOutages]\n  verified: '2026-07-27 — HTTP 200 with x-v:1 response header'\n- name: CDR Generic Tariff (AER Energy Made Easy host)\n  base_url: https://cdr.energymadeeasy.gov.au/powershop/cds-au/v1\n  authenticated: false\n  credential: none\n  required_headers:\n  - {name: x-v, required: true, description: 'Confirmed live: max supported version for listEnergyPlans is 1; x-v:9 returns HTTP 406 urn:au-cds:error:cds-all:Header/UnsupportedVersion.'}\n  operations: [listEnergyPlans, getEnergyPlanDetail]\n  verified: '2026-07-27 — HTTP 200, meta.totalRecords 482'\n- name: CDR Energy consumer data (accredited + consented)\n  base_url: null\n  base_url_note: >-\n    Not published anonymously. The authenticated data-holder base URI is resolved\n    through the CDR Register by accredited participants over mutual\
  \ TLS, so no\n    URL is asserted here.\n  authenticated: true\n  gate: accredited-only\n  operations:\n  - listEnergyAccounts\n  - getEnergyAccountDetail\n  - getEnergyAccountBalance\n  - listEnergyAccountBalancesBulk\n  - listEnergyAccountBalancesSpecificAccounts\n  - getEnergyAccountInvoices\n  - listEnergyAccountInvoicesBulk\n  - listEnergyInvoicesForSpecificAccounts\n  - getBillingForEnergyAccount\n  - listEnergyAccountBillingBulk\n  - listEnergyAccountBillingForSpecificAccounts\n  - getEnergyAccountPaymentSchedule\n  - getEnergyAccountConcessions\n  - listElectricityServicePoints\n  - getElectricityServicePointDetail\n  - getElectricityServicePointUsage\n  - listElectricityUsageBulk\n  - listElectricityUsageForServicePoints\n  - getElectricityDERForServicePoint\n  - listElectricityDERBulk\n  - listElectricityDERForSpecificServicePoints\n  - getCustomer\n  - getCustomerDetail\ncdr_security_profile:\n  regime: Consumer Data Right (Australia) — energy sector designation\n  standard:\
  \ CDR Consumer Data Standards v1.36.0 security profile\n  docs: https://consumerdatastandardsaustralia.github.io/standards/#security-profile\n  protocols:\n  - {name: OAuth 2.0, role: authorisation framework}\n  - {name: OpenID Connect, role: identity layer and authorisation code flow}\n  - {name: FAPI, role: financial-grade API hardening profile mandated by the CDS security profile}\n  - {name: Mutual TLS, role: client authentication and sender-constrained tokens using CDR Register-issued certificates}\n  - {name: PAR (RFC 9126), role: pushed authorisation requests}\n  - {name: JARM, role: signed authorisation responses}\n  grant: authorization_code\n  client_registration: >-\n    Dynamic client registration against the data holder, brokered by the CDR\n    Register; the accredited data recipient's software product must be listed on\n    the Register and hold Register-issued transport and signing certificates.\n  scopes: scopes/powershop-scopes.yml\nconsumer_authorisation_flow:\n  source:\
  \ https://www.powershop.com.au/privacy-policy/cdr-policy\n  steps:\n  - The consumer starts in the accredited data recipient's app and selects Powershop as their energy provider.\n  - The consumer is redirected to Powershop to authenticate.\n  - Powershop verifies identity with a one-time password sent to the email address on the account.\n  - The consumer selects which accounts, which data clusters, and the sharing duration.\n  - Powershop issues the authorisation; the ADR exchanges it for a mutual-TLS-bound access token.\n  dashboard: https://dashboard.cdr.powershop.com.au/\n  dashboard_note: Consumer-facing consent management UI (HTTP 200 on 2026-07-27), not a developer surface.\nwhat_a_developer_must_do:\n  public_data: Nothing. Send an x-v header. No signup, no key, no accreditation.\n  consumer_data: >-\n    Become an ACCC accredited data recipient (or operate as the authorised\n    representative or CDR representative of one), be listed on the CDR Register,\n    hold Register-issued\
  \ mutual-TLS certificates, and obtain an explicit,\n    time-bounded, scoped consent from each consumer. There is no commercial,\n    partner or sandbox path around this. Powershop issues no API key at any tier.\nno_first_party_program: >-\n  Powershop runs no developer portal, no API key issuance, no sandbox and no\n  partner API programme. It stated publicly in 2017 that it has no public API and\n  directed customers to download usage data from the account UI instead.\ncross_links:\n  scopes: scopes/powershop-scopes.yml\n  conventions: conventions/powershop-conventions.yml\n  conformance: conformance/powershop-conformance.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/powershop/refs/heads/main/authentication/powershop-authentication.yml
summary_line: oauth2/openIdConnect/mutualTLS · 0 schemes
tags:
- Energy
- Australia
- Utilities
- Electricity
- Gas
- Consumer Data Right
- Energy Retail
- Smart Metering
- Solar
- Tariffs
- Open Data
---
