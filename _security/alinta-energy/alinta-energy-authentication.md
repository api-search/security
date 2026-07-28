---
api_key_in: []
api_specs:
- filename: alinta-energy-cds-common-api-openapi.yml
  format: yaml
  label: Alinta Energy CDR Discovery API
  slug: alinta-energy-cdr-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alinta-energy/refs/heads/main/openapi/alinta-energy-cds-common-api-openapi.yml
- filename: alinta-energy-cds-energy-api-openapi.yml
  format: yaml
  label: Alinta Energy CDR Generic Plan Data API
  slug: alinta-energy-cdr-generic-plan-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alinta-energy/refs/heads/main/openapi/alinta-energy-cds-energy-api-openapi.yml
- filename: alinta-energy-cds-energy-api-openapi.yml
  format: yaml
  label: Alinta Energy CDR Energy API
  slug: alinta-energy-cdr-energy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alinta-energy/refs/heads/main/openapi/alinta-energy-cds-energy-api-openapi.yml
auth_types:
- none
- oauth2
- openIdConnect
- mutualTLS
description: ''
kind: authentication
layout: security
method: searched
name: Alinta Energy Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- hybrid
overview: Alinta Energy secures its APIs with none, oauth2, openIdConnect, and mutualTLS across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and hybrid flow(s).
provider_name: Alinta Energy
provider_slug: alinta-energy
scheme_count: 4
schemes:
- applies_to:
  - openapi/alinta-energy-cds-common-api-openapi.yml#getStatus
  - openapi/alinta-energy-cds-common-api-openapi.yml#getOutages
  - openapi/alinta-energy-cds-energy-api-openapi.yml#listEnergyPlans
  - openapi/alinta-energy-cds-energy-api-openapi.yml#getEnergyPlanDetail
  name: PublicNoAuth
  note: Version header x-v only (mandatory). Unsupported version returns HTTP 406.
  type: none
- flows:
  - flow: authorizationCode
    note: 'OIDC Hybrid Flow / Authorization Code Flow with Pushed Authorisation Requests (PAR), PKCE, signed request objects and JARM per the CDR Security Profile. The concrete authorisation, token, PAR, JWKS, introspection, revocation and CDR arrangement revocation endpoints are published per data holder through the CDR Register''s authenticated data holder brand detail record, not anonymously.

      '
  name: CDR-FAPI-OAuth2
  profile: FAPI 1.0 Advanced (Financial-grade API Security Profile 1.0 Part 2, March 2021)
  scopes_ref: scopes/alinta-energy-scopes.yml
  type: oauth2
- name: CDR-OIDC
  note: 'OpenID Connect 1.0. No anonymous /.well-known/openid-configuration is served by Alinta (confirmed HTTP 404 on public.cdr.alintaenergy.com.au, and the secure., idp. and cdr. subdomains of alintaenergy.com.au do not resolve). See well-known/alinta-energy-well-known.yml.

    '
  type: openIdConnect
- name: CDR-MTLS-HolderOfKey
  note: 'Mutual TLS with CDR Register CA-issued client certificates; access tokens are bound to the ADR client certificate under the holder-of-key mechanism. BCP195-recommended ciphers only (Data Standards obligation from 17 March 2025).

    '
  type: mutualTLS
slug: alinta-energy-authentication
source_filename: alinta-energy-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: searched\nsource: https://consumerdatastandardsaustralia.github.io/standards/#security-profile\ndocs: https://www.alintaenergy.com.au/help-and-support/terms-and-conditions/consumer-data-right-cdr\nnote: >\n  The mechanical derive-authentication.py pass found no formal securitySchemes: the\n  harvested contracts are the shared DSB Consumer Data Standards documents, which\n  express per-operation authorisation via the x-scopes vendor extension rather than a\n  components.securitySchemes block. The model below is captured from the Consumer Data\n  Standards Security Profile (which binds Alinta as a designated CDR energy data holder)\n  and from Alinta's own published CDR page.\nsummary:\n  types: [none, oauth2, openIdConnect, mutualTLS]\n  api_key_in: []\n  oauth2_flows: [authorizationCode, hybrid]\n  tiers:\n  - name: Public CDR discovery (Alinta-hosted)\n    auth: none\n    note: >\n      GET /cds-au/v1/discovery/status and GET /cds-au/v1/discovery/outages\
  \ on\n      https://public.cdr.alintaenergy.com.au require NO authentication — only the\n      mandatory x-v version header. Both re-confirmed HTTP 200 on 2026-07-27.\n  - name: Generic plan data (AER-hosted on Alinta's behalf)\n    auth: none\n    note: >\n      GET /alinta/cds-au/v1/energy/plans and /energy/plans/{planId} on\n      https://cdr.energymadeeasy.gov.au are public and unauthenticated (x-v header only).\n      493 Alinta plans re-confirmed HTTP 200 on 2026-07-27. This host is operated by the\n      Australian Energy Regulator, not by Alinta.\n  - name: Consumer data sharing (CDR accredited-data-recipient model)\n    auth: [oauth2, openIdConnect, mutualTLS]\n    note: >\n      Every energy resource endpoint (accounts, balances, invoices, billing, payment\n      schedule, concessions, service points, usage, DER) and the common customer\n      endpoints are gated behind the CDR security profile. Access requires ACCC\n      accreditation (or a CDR representative/sponsorship arrangement),\
  \ CDR\n      Register-issued credentials, dynamic client registration with Alinta's\n      authorisation server, and an explicit, time-bound, revocable consumer consent.\nschemes:\n- name: PublicNoAuth\n  type: none\n  applies_to:\n  - openapi/alinta-energy-cds-common-api-openapi.yml#getStatus\n  - openapi/alinta-energy-cds-common-api-openapi.yml#getOutages\n  - openapi/alinta-energy-cds-energy-api-openapi.yml#listEnergyPlans\n  - openapi/alinta-energy-cds-energy-api-openapi.yml#getEnergyPlanDetail\n  note: Version header x-v only (mandatory). Unsupported version returns HTTP 406.\n- name: CDR-FAPI-OAuth2\n  type: oauth2\n  profile: FAPI 1.0 Advanced (Financial-grade API Security Profile 1.0 Part 2, March 2021)\n  flows:\n  - flow: authorizationCode\n    note: >\n      OIDC Hybrid Flow / Authorization Code Flow with Pushed Authorisation Requests (PAR),\n      PKCE, signed request objects and JARM per the CDR Security Profile. The concrete\n      authorisation, token, PAR, JWKS, introspection,\
  \ revocation and CDR arrangement\n      revocation endpoints are published per data holder through the CDR Register's\n      authenticated data holder brand detail record, not anonymously.\n  scopes_ref: scopes/alinta-energy-scopes.yml\n- name: CDR-OIDC\n  type: openIdConnect\n  note: >\n    OpenID Connect 1.0. No anonymous /.well-known/openid-configuration is served by\n    Alinta (confirmed HTTP 404 on public.cdr.alintaenergy.com.au, and the secure., idp.\n    and cdr. subdomains of alintaenergy.com.au do not resolve). See\n    well-known/alinta-energy-well-known.yml.\n- name: CDR-MTLS-HolderOfKey\n  type: mutualTLS\n  note: >\n    Mutual TLS with CDR Register CA-issued client certificates; access tokens are bound\n    to the ADR client certificate under the holder-of-key mechanism. BCP195-recommended\n    ciphers only (Data Standards obligation from 17 March 2025).\ncustomer_authentication:\n  flow: Redirect to Web with One Time Password (OTP)\n  evidence: >\n    Alinta's published\
  \ CDR page states that when a consumer consents through an\n    accredited third party, \"Alinta Energy will ask you to verify your identity using a\n    One Time Password sent to the mobile number connected to your Alinta Energy account.\"\n    (Page body returns HTTP 403 to automated clients; text retrieved from the public\n    search index on 2026-07-27.)\n  standard: https://consumerdatastandardsaustralia.github.io/standards/#authentication-flows\npolicy:\n  cdr_policy: https://www.alintaenergy.com.au/help-and-support/terms-and-conditions/consumer-data-right-cdr/consumer-data-right-policy\n  cdr_page: https://www.alintaenergy.com.au/help-and-support/terms-and-conditions/consumer-data-right-cdr\nonboarding:\n  self_serve: false\n  gate: ACCC accreditation (Accredited Data Recipient) + consumer consent\n  note: No developer portal, no sandbox, no key request page, no commercial partner track outside the regulated scheme.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/alinta-energy/refs/heads/main/authentication/alinta-energy-authentication.yml
summary_line: none/oauth2/openIdConnect/mutualTLS · 4 schemes
tags:
- Energy
- Australia
- Utilities
- Electricity
- Gas
- Energy Retail
- Consumer Data Right
- CDR
- Open Energy Data
- Smart Metering
- Renewables
- Generation
---
