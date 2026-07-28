---
api_key_in: []
api_specs:
- filename: simply-energy-cds-energy-openapi.yml
  format: yaml
  label: Simply Energy (ENGIE) CDR Energy Generic Plans API
  slug: simply-energy-cdr-energy-generic-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simply-energy/refs/heads/main/openapi/simply-energy-cds-energy-openapi.yml
- filename: simply-energy-cds-common-openapi.yml
  format: yaml
  label: Simply Energy (ENGIE) CDR Discovery API
  slug: simply-energy-cdr-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simply-energy/refs/heads/main/openapi/simply-energy-cds-common-openapi.yml
- filename: simply-energy-cds-energy-openapi.yml
  format: yaml
  label: Simply Energy (ENGIE) CDR Energy Consumer Data API
  slug: simply-energy-cdr-energy-consumer-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/simply-energy/refs/heads/main/openapi/simply-energy-cds-energy-openapi.yml
auth_types:
- none
- oauth2
- openIdConnect
- mutualTLS
description: ''
kind: authentication
layout: security
method: searched
name: Simply Energy Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Simply Energy secures its APIs with none, oauth2, openIdConnect, and mutualTLS across 0 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Simply Energy
provider_slug: simply-energy
scheme_count: 0
schemes: []
slug: simply-energy-authentication
source_filename: simply-energy-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: searched\nsource: openapi/simply-energy-cds-common-openapi.yml, openapi/simply-energy-cds-energy-openapi.yml\ndocs: https://consumerdatastandardsaustralia.github.io/standards/#security-profile\nprovider_published: false\nprovenance_note: |\n  The Data Standards Body Consumer Data Standards OpenAPI documents this provider conforms to\n  declare NO components.securitySchemes at all - `derive-authentication.py` returned an empty\n  profile. That is a property of the shared specification, not evidence that the API is\n  unauthenticated. The real authentication model is normative and lives in the CDR Security\n  Profile, which is binding on this data holder (provider number DH002028). This profile was\n  therefore SEARCHED from the published standard rather than derived from the spec, and every\n  claim below is traceable to the Consumer Data Standards or to a live anonymous probe.\nsummary:\n  types: [none, oauth2, openIdConnect, mutualTLS]\n  api_key_in:\
  \ []\n  oauth2_flows: [authorizationCode]\n  surfaces_by_gate:\n    public_unauthenticated: 2\n    accredited_only: 1\nsurfaces:\n- name: CDR Energy Generic Plans (public tariff data)\n  api: simply-energy:simply-energy-cdr-energy-generic-plans-api\n  baseURL: https://cdr.energymadeeasy.gov.au/engie/cds-au/v1\n  auth: none\n  scheme_type: none\n  detail: |\n    Fully anonymous. No API key, no registration, no agreement. The only mandatory request\n    header is x-v (endpoint version). Confirmed live on 2026-07-27: an anonymous\n    GET /energy/plans?page-size=1 with x-v: 1 returned HTTP 200 with meta.totalRecords 2452.\n  required_headers: [x-v]\n  optional_headers: [x-min-v]\n- name: CDR Common Discovery (status and outages)\n  api: simply-energy:simply-energy-cdr-discovery-api\n  baseURL: https://public.cdr.engie.com.au/cds-au/v1\n  auth: none\n  scheme_type: none\n  detail: |\n    Fully anonymous. Confirmed live on 2026-07-27: GET /discovery/status with x-v: 1 returned\n    HTTP 200\
  \ with {\"data\":{\"status\":\"OK\",...}} and the response carried\n    strict-transport-security: max-age=63072000; includeSubDomains.\n  required_headers: [x-v]\n  optional_headers: [x-min-v]\n- name: CDR Energy Consumer Data (accredited only)\n  api: simply-energy:simply-energy-cdr-energy-consumer-data-api\n  baseURL: null\n  auth: oauth2 + openIdConnect + mutualTLS\n  scheme_type: oauth2\n  gate: accredited-only\n  detail: |\n    Not anonymously verifiable. The InfoSec and resource base URIs of an energy data holder\n    are published only through the authenticated portion of the CDR Register and are reachable\n    only by an ACCC-accredited data recipient presenting a CDR client certificate. Anonymous\n    probes for /.well-known/openid-configuration on public.cdr.engie.com.au and on\n    cdr.energymadeeasy.gov.au both returned HTTP 404 (see well-known/).\n  profile:\n    name: CDR Security Profile\n    based_on: FAPI 1.0 Advanced (Financial-grade API Advanced Profile) + OpenID Connect\
  \ 1.0\n    docs: https://consumerdatastandardsaustralia.github.io/standards/#security-profile\n    mechanisms:\n    - OAuth 2.0 authorization code flow with OpenID Connect\n    - Pushed Authorisation Requests (PAR)\n    - PKCE (Proof Key for Code Exchange)\n    - private_key_jwt client authentication\n    - Mutually Authenticated TLS (MTLS) with holder-of-key token binding\n    - JARM (JWT Secured Authorization Response Mode)\n    - Pairwise Pseudonymous Identifiers (PPID) as subject type\n    - Request objects signed as JWT\n    prerequisites:\n    - ACCC accreditation as a data recipient under the CDR Rules\n    - CDR client certificate issued under the CDR PKI\n    - Software product registered on the CDR Register (Dynamic Client Registration)\n    - Explicit, scoped, time-limited consumer consent (CDR consent model)\n    scopes: scopes/simply-energy-scopes.yml\nrequest_context_headers:\n- name: x-v\n  required: true\n  detail: Endpoint version requested. Must be a positive integer.\
  \ Mismatch returns HTTP 406\n    urn:au-cds:error:cds-all:Header/UnsupportedVersion.\n- name: x-min-v\n  required: false\n  detail: Minimum acceptable endpoint version.\n- name: x-fapi-interaction-id\n  required: false\n  detail: RFC 4122 UUID correlation id. The data holder MUST play it back in the response.\n    Confirmed present on live responses from both public hosts.\n- name: x-fapi-auth-date\n  required: conditional\n  detail: Time the customer last logged in to the data recipient software product. Required\n    for all authenticated resource calls. Not used on unauthenticated calls.\n- name: x-fapi-customer-ip-address\n  required: false\n  detail: Customer's original IP when the call is customer-present. Not to be included for\n    unauthenticated calls.\n- name: x-cds-client-headers\n  required: conditional\n  detail: Base64-encoded original customer HTTP headers. Mandatory for customer-present calls.\nevidence:\n- {source: 'live probe 2026-07-27', detail: 'GET https://cdr.energymadeeasy.gov.au/engie/cds-au/v1/energy/plans?page-size=1\
  \ (x-v 1) -> HTTP 200, no credential presented'}\n- {source: 'live probe 2026-07-27', detail: 'GET https://public.cdr.engie.com.au/cds-au/v1/discovery/status (x-v 1) -> HTTP 200, no credential presented'}\n- {source: 'live probe 2026-07-27', detail: 'GET https://public.cdr.engie.com.au/cds-au/v1/discovery/status (x-v 9) -> {\"errors\":[{\"code\":\"urn:au-cds:error:cds-all:Header/UnsupportedVersion\",...}]}'}\n- {source: https://consumerdatastandardsaustralia.github.io/standards/#security-profile, detail: CDR Security Profile - FAPI 1.0 Advanced, PAR, PKCE, private_key_jwt, MTLS, JARM}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/simply-energy/refs/heads/main/authentication/simply-energy-authentication.yml
summary_line: none/oauth2/openIdConnect/mutualTLS · 0 schemes
tags:
- Energy
- Australia
- Utilities
- Electricity
- Gas
- Energy Retail
- Consumer Data Right
- CDR
- Smart Metering
- Energy Markets
---
