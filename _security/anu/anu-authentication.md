---
api_key_in:
- header
api_specs:
- filename: anu-quantum-numbers-openapi.yml
  format: yaml
  label: ANU Quantum Numbers (AQN) API
  slug: quantum-numbers
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anu/refs/heads/main/openapi/anu-quantum-numbers-openapi.yml
- filename: anu-qrng-legacy-openapi.yml
  format: yaml
  label: QRNG@ANU Legacy JSON API
  slug: qrng-legacy
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anu/refs/heads/main/openapi/anu-qrng-legacy-openapi.yml
- filename: anu-open-research-oai-pmh-openapi.yml
  format: yaml
  label: ANU Open Research OAI-PMH
  slug: openresearch-oai
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anu/refs/heads/main/openapi/anu-open-research-oai-pmh-openapi.yml
auth_types:
- apiKey
- none
- saml2
description: ''
kind: authentication
layout: security
method: derived
name: Anu Authentication
name_suffix: Authentication
oauth_flows: []
overview: Australian National University secures its APIs with apiKey, none, and saml2 across 5 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Australian National University
provider_slug: anu
scheme_count: 5
schemes:
- applies_to: https://api.quantumnumbers.anu.edu.au
  cost: free
  evidence: ANU's own documentation gives the call form as curl -X GET -H "x-api-key:${API_KEY}" "${API_URL}?length=..&type=..&size=..". A live request with no key returns HTTP 403 {"message":"Forbidden"} from the gateway.
  in: header
  issuance: Self-serve registration at https://quantumnumbers.anu.edu.au
  name: AqnApiKey
  parameter: x-api-key
  purpose: Authorize calls to the ANU Quantum Numbers service.
  rotation: Not documented.
  scopes: none
  type: apiKey
- applies_to: https://qrng.anu.edu.au/API/jsonI.php
  evidence: Live unauthenticated GET returned {"type":"uint8","length":4,"data":[74,205,98,159],"success":true} on 2026-08-19. Access control is replaced by a one-request-per-minute throttle.
  name: LegacyQrngAnonymous
  purpose: The deprecated legacy endpoint requires no credential of any kind.
  type: none
- applies_to: https://openresearch-repository.anu.edu.au/server/oai/request
  evidence: Live Identify and ListRecords calls succeeded unauthenticated on 2026-08-19.
  name: OaiPmhAnonymous
  purpose: OAI-PMH harvesting is open by design; no credential is required or accepted.
  type: none
- applies_to: https://openresearch-repository.anu.edu.au/server/api
  evidence: GET /server/api returns 200 application/hal+json; GET /server/api/core/items returns 401 application/json, so the surface is genuinely access-controlled rather than uniformly open.
  name: DSpaceRestAnonymous
  purpose: The DSpace REST root and its discovery/browse resources are readable anonymously; write and some core collections require a session.
  type: none
- applies_to: https://idp2.anu.edu.au/idp/shibboleth
  developer_note: This is an end-user login federation. There is no client registration path, no token endpoint and no consent surface an outside developer could integrate against.
  developer_usable: false
  evidence: Live IdP metadata publishes SAML 2.0 SSO endpoints for HTTP-POST, HTTP-Redirect and SOAP/ECP bindings with scope anu.edu.au.
  name: AafShibbolethSso
  purpose: Institutional single sign-on for staff and students, federated through the Australian Access Federation and interfederated via eduGAIN. Governs human access to Wattle, library resources and staff systems.
  type: saml2
slug: anu-authentication
source_filename: anu-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-19'\nmethod: derived\nsource: https://quantumnumbers.anu.edu.au/documentation\nx-operator: institution\nsummary:\n  types:\n  - apiKey\n  - none\n  - saml2\n  api_key_in:\n  - header\n  oauth2_flows: []\n  note: >-\n    ANU has no single institutional authorization surface. Its three publicly reachable,\n    institution-operated API surfaces authenticate three different ways, and one of them\n    does not authenticate at all. The identity surface that does the real work at ANU is\n    SAML 2.0 federation through the Australian Access Federation — it governs access to\n    Wattle, the library and staff systems, but it is a login federation, not an API\n    authorization layer, and no developer can obtain a token from it.\nschemes:\n- name: AqnApiKey\n  type: apiKey\n  in: header\n  parameter: x-api-key\n  applies_to: https://api.quantumnumbers.anu.edu.au\n  issuance: Self-serve registration at https://quantumnumbers.anu.edu.au\n  cost: free\n  purpose: Authorize\
  \ calls to the ANU Quantum Numbers service.\n  evidence: >-\n    ANU's own documentation gives the call form as\n    curl -X GET -H \"x-api-key:${API_KEY}\" \"${API_URL}?length=..&type=..&size=..\". A live\n    request with no key returns HTTP 403 {\"message\":\"Forbidden\"} from the gateway.\n  rotation: Not documented.\n  scopes: none\n- name: LegacyQrngAnonymous\n  type: none\n  applies_to: https://qrng.anu.edu.au/API/jsonI.php\n  purpose: The deprecated legacy endpoint requires no credential of any kind.\n  evidence: >-\n    Live unauthenticated GET returned {\"type\":\"uint8\",\"length\":4,\"data\":[74,205,98,159],\"success\":true}\n    on 2026-08-19. Access control is replaced by a one-request-per-minute throttle.\n- name: OaiPmhAnonymous\n  type: none\n  applies_to: https://openresearch-repository.anu.edu.au/server/oai/request\n  purpose: OAI-PMH harvesting is open by design; no credential is required or accepted.\n  evidence: Live Identify and ListRecords calls succeeded unauthenticated\
  \ on 2026-08-19.\n- name: DSpaceRestAnonymous\n  type: none\n  applies_to: https://openresearch-repository.anu.edu.au/server/api\n  purpose: >-\n    The DSpace REST root and its discovery/browse resources are readable anonymously; write\n    and some core collections require a session.\n  evidence: >-\n    GET /server/api returns 200 application/hal+json; GET /server/api/core/items returns 401\n    application/json, so the surface is genuinely access-controlled rather than uniformly open.\n- name: AafShibbolethSso\n  type: saml2\n  applies_to: https://idp2.anu.edu.au/idp/shibboleth\n  purpose: >-\n    Institutional single sign-on for staff and students, federated through the Australian\n    Access Federation and interfederated via eduGAIN. Governs human access to Wattle, library\n    resources and staff systems.\n  evidence: >-\n    Live IdP metadata publishes SAML 2.0 SSO endpoints for HTTP-POST, HTTP-Redirect and\n    SOAP/ECP bindings with scope anu.edu.au.\n  developer_usable: false\n\
  \  developer_note: >-\n    This is an end-user login federation. There is no client registration path, no token\n    endpoint and no consent surface an outside developer could integrate against.\nexcluded:\n- surface: https://researchportalplus.anu.edu.au\n  reason: >-\n    Elsevier Pure tenancy (CNAME anu2-portal.elsevierpure.com). Its authentication is\n    Elsevier's, and crediting it to ANU is exactly the misattribution this pipeline prevents.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/anu/refs/heads/main/authentication/anu-authentication.yml
summary_line: apiKey/none/saml2 · 5 schemes
tags:
- University
- Higher Education
- Education
- Research
- Australia
- Group of Eight
- Research Repository
- Identity Federation
- Open Access
- Quantum
- Random Numbers
- OAI-PMH
---
