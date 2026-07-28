---
api_key_in: []
api_specs:
- filename: alectra-utilities-green-button-espi-openapi.json
  format: json
  label: Alectra Utilities Green Button Connect My Data (CMD) API
  slug: alectra-green-button-connect-my-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/alectra-utilities/refs/heads/main/openapi/alectra-utilities-green-button-espi-openapi.json
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: derived
name: Alectra Utilities Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: Alectra Utilities secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: Alectra Utilities
provider_slug: alectra-utilities
scheme_count: 1
schemes:
- applied_to_operations: all
  flows:
  - authorizationUrl: https://sandbox.greenbuttonalliance.org:8443/oauth/authorize
    flow: authorizationCode
    note: The Green Button Connect My Data consent flow — a retail customer authorises a registered, approved third party to receive their ESPI resources. The scopes map is empty in the source spec; ESPI's scope grammar is not enumerated there and Alectra publishes none, so none are recorded.
    scope_count: 0
    tokenUrl: https://sandbox.greenbuttonalliance.org:8443/oauth/token
  - flow: clientCredentials
    note: Used by a registered third party for its own ApplicationInformation and bulk registration-level calls rather than for customer data.
    scope_count: 0
    tokenUrl: https://sandbox.greenbuttonalliance.org:8443/oauth/token
  name: oauth2
  sources:
  - openapi/alectra-utilities-green-button-espi-openapi.json
  type: oauth2
slug: alectra-utilities-authentication
source_filename: alectra-utilities-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: derived\nsource: openapi/alectra-utilities-green-button-espi-openapi.json\nprovenance_warning: >-\n  Derived from the Green Button Alliance OpenAPI harvested into openapi/, NOT from\n  an Alectra-published authentication reference. Alectra Utilities publishes no OAuth\n  metadata, no client registration surface, no scope list and no token endpoint. The\n  authorization and token URLs below are the Green Button Alliance public sandbox's,\n  carried verbatim from the spec's securitySchemes; Alectra's own endpoints are\n  disclosed to third parties only after registration and approval. Probes on\n  2026-07-27 recorded https://alectrautilities.com/.well-known/openid-configuration\n  HTTP 403 and every /DataCustodian/oauth/* path on\n  https://alectrautilitiesgbportal.savagedata.com/ HTTP 302 to /Connect/Authorize\n  (a catch-all auth wall confirmed with a bogus control path) — see review.yml.\nsummary:\n  types:\n  - oauth2\n  api_key_in: []\n \
  \ oauth2_flows:\n  - authorizationCode\n  - clientCredentials\n  applied_globally: true\n  scopes_declared: 0\nschemes:\n- name: oauth2\n  type: oauth2\n  sources:\n  - openapi/alectra-utilities-green-button-espi-openapi.json\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://sandbox.greenbuttonalliance.org:8443/oauth/authorize\n    tokenUrl: https://sandbox.greenbuttonalliance.org:8443/oauth/token\n    scope_count: 0\n    note: >-\n      The Green Button Connect My Data consent flow — a retail customer authorises a\n      registered, approved third party to receive their ESPI resources. The scopes\n      map is empty in the source spec; ESPI's scope grammar is not enumerated there\n      and Alectra publishes none, so none are recorded.\n  - flow: clientCredentials\n    tokenUrl: https://sandbox.greenbuttonalliance.org:8443/oauth/token\n    scope_count: 0\n    note: >-\n      Used by a registered third party for its own ApplicationInformation and bulk\n      registration-level\
  \ calls rather than for customer data.\n  applied_to_operations: all\ntoken:\n  type: Bearer\n  carrier: Authorization header\n  evidence: >-\n    components.schemas.Authorization declares token_type (Bearer), expires_at,\n    grant_type, scope, resourceURI and authorizationURI — the ESPI authorization\n    record a data custodian returns to an approved third party.\nonboarding:\n  self_serve: false\n  gate: application-approval\n  registration_url: https://alectrautilitiesonboarding.savagedata.com/\n  terms_url: https://alectrautilities.com/green-button-connect-my-data-terms-and-conditions-access-and-use\n  steps:\n  - Register as a third party at the Alectra onboarding site (hosted by Savage Data Systems).\n  - Accept the Green Button Connect My Data Terms and Conditions of Access and Use.\n  - Be approved by Alectra as an authorised third-party provider.\n  - A customer then authorises the connection in the Green Button portal, selecting data and period.\n  accreditation_body: none\n\
  \  note: >-\n    Ontario has no accredited data recipient regime (unlike the Australian CDR), so\n    approval is Alectra's own commercial and compliance decision.\ncustomer_facing_auth:\n  green_button_portal: Account name from the bill plus phone-number validation.\n  commercial_industrial_dataview: Email and password registration with account linking.\nverified_on_alectra: false\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/alectra-utilities/refs/heads/main/authentication/alectra-utilities-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Energy
- Canada
- Utilities
- Electricity
- Ontario
- Green Button
- Smart Metering
- Energy Data
- Grid
- Municipal Utility
- ESPI
---
