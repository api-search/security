---
api_key_in: []
api_specs:
- filename: agl-energy-data-holder-customers-api-openapi.yml
  format: yaml
  label: AGL Energy Data Holder Customers API
  slug: agl-energy-data-holder-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agl-energy/refs/heads/main/openapi/agl-energy-data-holder-customers-api-openapi.yml
- filename: agl-energy-data-holder-operations-api-openapi.yml
  format: yaml
  label: AGL Energy Data Holder Operations API
  slug: agl-energy-data-holder-operations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agl-energy/refs/heads/main/openapi/agl-energy-data-holder-operations-api-openapi.yml
- filename: agl-energy-distributed-energy-resources-api-openapi.yml
  format: yaml
  label: AGL Energy Distributed Energy Resources API
  slug: agl-energy-distributed-energy-resources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agl-energy/refs/heads/main/openapi/agl-energy-distributed-energy-resources-api-openapi.yml
- filename: agl-energy-electricity-service-points-api-openapi.yml
  format: yaml
  label: AGL Energy Electricity Service Points API
  slug: agl-energy-electricity-service-points-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agl-energy/refs/heads/main/openapi/agl-energy-electricity-service-points-api-openapi.yml
- filename: agl-energy-electricity-usage-api-openapi.yml
  format: yaml
  label: AGL Energy Electricity Usage API
  slug: agl-energy-electricity-usage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agl-energy/refs/heads/main/openapi/agl-energy-electricity-usage-api-openapi.yml
- filename: agl-energy-energy-account-balances-api-openapi.yml
  format: yaml
  label: AGL Energy Energy Account Balances API
  slug: agl-energy-energy-account-balances-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agl-energy/refs/heads/main/openapi/agl-energy-energy-account-balances-api-openapi.yml
- filename: agl-energy-energy-account-billing-api-openapi.yml
  format: yaml
  label: AGL Energy Energy Account Billing API
  slug: agl-energy-energy-account-billing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agl-energy/refs/heads/main/openapi/agl-energy-energy-account-billing-api-openapi.yml
- filename: agl-energy-energy-accounts-api-openapi.yml
  format: yaml
  label: AGL Energy Energy Accounts API
  slug: agl-energy-energy-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agl-energy/refs/heads/main/openapi/agl-energy-energy-accounts-api-openapi.yml
- filename: agl-energy-energy-plans-api-openapi.yml
  format: yaml
  label: AGL Energy Energy Plans API
  slug: agl-energy-energy-plans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agl-energy/refs/heads/main/openapi/agl-energy-energy-plans-api-openapi.yml
auth_types:
- oauth2
- openIdConnect
- mutualTLS
- none
description: 'AGL''s authentication model is not AGL''s design — it is the Consumer Data Right security profile, which every designated data holder implements identically. The harvested Consumer Data Standards OpenAPI documents declare NO components.securitySchemes at all (verified: both cds_common and cds_energy ship an empty securitySchemes object), because the CDR carries its security contract in the Security Profile section of the standards and in the CDR Register''s certificate distribution, not inside the API specification. There are therefore three distinct auth postures across AGL''s three API surfaces, and only one of them is authenticated at all.'
kind: authentication
layout: security
method: searched
name: Agl Energy Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: AGL Energy secures its APIs with oauth2, openIdConnect, mutualTLS, and none across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: AGL Energy
provider_slug: agl-energy
scheme_count: 3
schemes:
- flow: authorizationCode
  name: CDR OAuth 2.0 / OpenID Connect (FAPI 1.0 Advanced)
  profile: FAPI 1.0 Advanced Security Profile
  requirements:
  - Pushed Authorization Requests (PAR, RFC 9126) — the authorisation request is pushed server-to-server
  - private_key_jwt client authentication
  - mTLS-bound (sender-constrained) access tokens, RFC 8705
  - request object signing (PS256 / ES256)
  - OIDC Hybrid or Authorization Code flow per the profile version in force
  - CDR Arrangement ID issued per consent, revocable by the consumer or the ADR
  scopes_artifact: scopes/agl-energy-scopes.yml
  source: https://consumerdatastandardsaustralia.github.io/standards/#security-profile
  type: oauth2
- detail: All consumer-data calls between an Accredited Data Recipient and AGL as data holder run over mutual TLS using transport certificates issued by the CDR Register certificate authority. Signing certificates are separately issued.
  name: CDR transport security
  source: https://consumerdatastandardsaustralia.github.io/standards/#security-profile
  type: mutualTLS
- detail: Discovery and Product Reference Data endpoints carry no authentication. The x-v version header is mandatory but is not a credential.
  name: Anonymous (public CDR surfaces)
  type: none
slug: agl-energy-authentication
source_filename: agl-energy-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: searched\nsource: >-\n  Consumer Data Standards (CDR) Security Profile v1.36.0 —\n  https://consumerdatastandardsaustralia.github.io/standards/#security-profile —\n  plus live anonymous probes of AGL's CDR public base URI and the AER-operated\n  Product Reference Data host on 2026-07-27.\ndocs: https://consumerdatastandardsaustralia.github.io/standards/#security-profile\ndescription: >-\n  AGL's authentication model is not AGL's design — it is the Consumer Data Right\n  security profile, which every designated data holder implements identically.\n  The harvested Consumer Data Standards OpenAPI documents declare NO\n  components.securitySchemes at all (verified: both cds_common and cds_energy\n  ship an empty securitySchemes object), because the CDR carries its security\n  contract in the Security Profile section of the standards and in the CDR\n  Register's certificate distribution, not inside the API specification. There\n  are therefore three\
  \ distinct auth postures across AGL's three API surfaces, and\n  only one of them is authenticated at all.\nsummary:\n  types: [oauth2, openIdConnect, mutualTLS, none]\n  api_key_in: []\n  oauth2_flows: [authorizationCode]\n  spec_declared_security_schemes: 0\n  note: >-\n    types are sourced from the CDR Security Profile, NOT from the OpenAPI —\n    derive-authentication.py over openapi/ correctly returns zero schemes.\nsurfaces:\n- surface: AGL CDR Discovery (Common) API\n  base_url: https://public.cdr.agl.com.au/cds-au/v1\n  auth: none\n  detail: >-\n    GET /discovery/status and GET /discovery/outages are fully anonymous. The\n    only mandatory header is the Consumer Data Standards version header x-v: 1.\n    Verified 200 on 2026-07-27.\n  verified: {status: 200, date: '2026-07-27'}\n- surface: AGL Energy Product Reference Data (PRD) API\n  base_url: https://cdr.energymadeeasy.gov.au/agl/cds-au/v1\n  auth: none\n  detail: >-\n    Anonymous HTTP GET, no key, no accreditation, CORS\n\
  \    Access-Control-Allow-Origin *. Required header is x-v (1 for /energy/plans,\n    3 for /energy/plans/{planId}). Operated by the Australian Energy Regulator,\n    not by AGL.\n  verified: {status: 200, date: '2026-07-27'}\n- surface: AGL CDR Energy API (consumer data)\n  base_url: null\n  base_url_note: >-\n    Not published. The consumer-facing base URI is distributed to accredited\n    participants through the CDR Register.\n  auth: oauth2 + openIdConnect over mutualTLS (FAPI 1.0 Advanced)\n  detail: >-\n    Consumer-authorised. Only an Accredited Data Recipient, a CDR\n    representative or a sponsored/affiliate party holding CDR Register-issued\n    certificates can call these endpoints.\nschemes:\n- name: CDR OAuth 2.0 / OpenID Connect (FAPI 1.0 Advanced)\n  type: oauth2\n  flow: authorizationCode\n  profile: FAPI 1.0 Advanced Security Profile\n  source: https://consumerdatastandardsaustralia.github.io/standards/#security-profile\n  requirements:\n  - Pushed Authorization Requests\
  \ (PAR, RFC 9126) — the authorisation request is pushed server-to-server\n  - private_key_jwt client authentication\n  - mTLS-bound (sender-constrained) access tokens, RFC 8705\n  - request object signing (PS256 / ES256)\n  - OIDC Hybrid or Authorization Code flow per the profile version in force\n  - CDR Arrangement ID issued per consent, revocable by the consumer or the ADR\n  scopes_artifact: scopes/agl-energy-scopes.yml\n- name: CDR transport security\n  type: mutualTLS\n  source: https://consumerdatastandardsaustralia.github.io/standards/#security-profile\n  detail: >-\n    All consumer-data calls between an Accredited Data Recipient and AGL as data\n    holder run over mutual TLS using transport certificates issued by the CDR\n    Register certificate authority. Signing certificates are separately issued.\n- name: Anonymous (public CDR surfaces)\n  type: none\n  detail: >-\n    Discovery and Product Reference Data endpoints carry no authentication. The\n    x-v version header is\
  \ mandatory but is not a credential.\nrequest_headers:\n- {name: x-v, required: true, purpose: requested endpoint version (positive integer)}\n- {name: x-min-v, required: false, purpose: minimum acceptable endpoint version}\n- {name: x-fapi-interaction-id, required: false, purpose: RFC 4122 UUID correlation id; echoed by the data holder}\n- {name: x-fapi-auth-date, required: false, purpose: time the consumer last logged in to the ADR software product}\n- {name: x-fapi-customer-ip-address, required: false, purpose: consumer's original IP when they are present}\n- {name: x-cds-client-headers, required: false, purpose: consumer's original HTTP headers, base64 encoded}\nonboarding:\n  self_serve: false\n  path: >-\n    Accreditation by the ACCC as a Data Recipient under the Consumer Data Right,\n    or operating under an existing ADR as a CDR representative or\n    sponsored/affiliate. Meet CDR Rules Schedule 2 information-security\n    controls, obtain CDR Register transport and signing certificates,\
  \ register a\n    software product, then obtain the individual consumer's authorisation\n    through AGL's own CDR consent flow.\n  docs: https://www.cdr.gov.au/for-providers\n  sandbox: false\noidc_discovery:\n  anonymous_document_found: false\n  probes:\n  - {url: 'https://public.cdr.agl.com.au/.well-known/openid-configuration', status: 404}\n  - {url: 'https://public.cdr.agl.com.au/.well-known/oauth-authorization-server', status: 404}\n  - {url: 'https://public.cdr.agl.com.au/.well-known/oauth-protected-resource', status: 404}\n  - {url: 'https://www.agl.com.au/.well-known/openid-configuration', status: 403}\n  note: >-\n    Expected under the CDR — data holder authorisation-server metadata is\n    published to the CDR Register and retrieved by accredited recipients, not\n    served anonymously.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/agl-energy/refs/heads/main/authentication/agl-energy-authentication.yml
summary_line: oauth2/openIdConnect/mutualTLS/none · 3 schemes
tags:
- Energy
- Australia
- Utilities
- Electricity
- Gas
- Energy Retailer
- Consumer Data Right
- CDR
- Smart Metering
- Solar
- DER
- Renewables
- Energy Markets
---
