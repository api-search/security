---
api_key_in: []
api_specs:
- filename: cdr-energy-api-openapi.json
  format: json
  label: AER Energy Product Reference Data - Get Generic Plans
  slug: aer-energy-product-reference-data-get-generic-plans
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aer/refs/heads/main/openapi/cdr-energy-api-openapi.json
- filename: cdr-energy-api-openapi.json
  format: json
  label: AER Energy Product Reference Data - Get Generic Plan Detail
  slug: aer-energy-product-reference-data-get-generic-plan-detail
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aer/refs/heads/main/openapi/cdr-energy-api-openapi.json
- filename: cds-common-api-openapi.json
  format: json
  label: AER CDR Discovery - Get Status and Get Outages
  slug: aer-cdr-discovery-status-and-outages
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aer/refs/heads/main/openapi/cds-common-api-openapi.json
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Aer Authentication
name_suffix: Authentication
oauth_flows: []
overview: Australian Energy Regulator declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Australian Energy Regulator
provider_slug: aer
scheme_count: 0
schemes: []
slug: aer-authentication
source_filename: aer-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: searched\nsource: openapi/cdr-energy-api-openapi.json + openapi/cds-common-api-openapi.json\ndocs: https://www.aer.gov.au/energy-product-reference-data\nsummary:\n  types: []\n  api_key_in: []\n  oauth2_flows: []\n  model: anonymous\n  statement: >-\n    The AER's public surface requires no credential of any kind. The Consumer Data\n    Standards classify Product Reference Data and the Common discovery endpoints as\n    unauthenticated (\"Public\") endpoints, and the harvested specifications carry no\n    securitySchemes and no security requirement on the operations the AER serves. The\n    AER's own FAQ states it plainly: \"Our APIs are public, so they don't require\n    accreditation.\" There is no portal, no registration, no API key, no OAuth client\n    and no mTLS certificate involved in calling GET /energy/plans,\n    GET /energy/plans/{planId}, GET /discovery/status or GET /discovery/outages.\nschemes: []\nrequired_headers:\n- name: x-v\n\
  \  in: header\n  required: true\n  description: >-\n    Mandatory version header. Omitting it returns HTTP 400 with\n    urn:au-cds:error:cds-all:Header/Missing (\"Header x-v must be provided\").\n  verified: '2026-07-27'\n- name: x-min-v\n  in: header\n  required: false\n  description: >-\n    Optional minimum acceptable version. Version-range negotiation works on this host:\n    GET /energy/plans/{planId} with x-v 5 and x-min-v 1 returned HTTP 200 with response\n    header x-v 3 (the highest version the AER supports for that operation) rather than\n    406.\n  verified: '2026-07-27'\nresponse_headers:\n- name: x-v\n  description: Echoes the version actually served.\n- name: x-fapi-interaction-id\n  description: >-\n    FAPI correlation identifier returned on every response; a server-generated UUID\n    when the caller does not supply one. This is the request-tracing handle to quote\n    in a support email.\n- name: access-control-allow-origin\n  description: \"* — CORS is fully open,\
  \ so browser-side calls work without a proxy.\"\n- name: access-control-expose-headers\n  description: \"x-v, Retry-After, x-fapi-interaction-id\"\ngated_surface:\n  note: >-\n    The authenticated half of the CDR energy regime is NOT the AER's. Consumer usage,\n    billing, account and service-point endpoints exist in the same specification but\n    return 404 on the AER host — retailers are the primary data holders and AEMO is\n    the secondary data holder gateway. Reaching those endpoints requires ACCC\n    accreditation as a data recipient, consumer consent, and the CDS information\n    security profile (OAuth 2.0 / OpenID Connect with mTLS-bound client\n    authentication, FAPI 1.0 Advanced). No OpenID configuration is served on any AER\n    host — /.well-known/openid-configuration returns 404 on\n    cdr.energymadeeasy.gov.au, www.energymadeeasy.gov.au and www.aer.gov.au.\n  accreditation: https://www.cdr.gov.au/for-providers/become-accredited-data-recipient\n  infosec_profile:\
  \ https://consumerdatastandardsaustralia.github.io/standards/#security-profile\nsupport_contact: cdr-support@aer.gov.au\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aer/refs/heads/main/authentication/aer-authentication.yml
summary_line: 0 schemes
tags:
- Energy
- Australia
- Utilities
- Electricity
- Gas
- Energy Markets
- Consumer Data Right
- Retail Energy
- Regulations
- Government
- Open Data
- Smart Metering
---
