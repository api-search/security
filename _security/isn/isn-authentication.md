---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Isn Authentication
name_suffix: Authentication
oauth_flows: []
overview: ISN declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: ISN
provider_slug: isn
scheme_count: 2
schemes:
- credentials:
  - description: An API key unique to an individual ISNetworld user or application.
    name: UserKey
  - description: An API key unique to the subscribing company account.
    name: CompanyKey
  in: header
  name: ISNCompanyUserKeys
  type: apiKey
  used_for: 'Exchanged at the token endpoint only. Both headers are sent together with Content-Type: application/json to obtain a bearer token.'
- name: ISNBearer
  scheme: bearer
  type: http
  used_for: 'Every resource call after the token exchange. The token is passed using the standard Authorization: Bearer <token> header.'
slug: isn-authentication
source_filename: isn-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-23'\nmethod: searched\nsource: >-\n  ISN's own \"ISNetworld API - Developer Integration Guide\" (the customer-issued PDF,\n  whose endpoint list and authentication flow are quoted publicly), corroborated by\n  live unauthenticated probes of https://api.isnetworld.com on 2026-08-23.\napi: ISNetworld API\nbase_url: https://api.isnetworld.com\ntransport_requirement: >-\n  Clients must send requests using TLS 1.2 or later over HTTPS. Confirmed live: the\n  host negotiates TLSv1.2 and returns Strict-Transport-Security: max-age=31536000;\n  includeSubDomains.\nmodel: bearer-token-issued-from-static-key-pair\nschemes:\n- name: ISNCompanyUserKeys\n  type: apiKey\n  in: header\n  credentials:\n  - name: UserKey\n    description: An API key unique to an individual ISNetworld user or application.\n  - name: CompanyKey\n    description: An API key unique to the subscribing company account.\n  used_for: >-\n    Exchanged at the token endpoint only. Both headers are sent\
  \ together with\n    Content-Type: application/json to obtain a bearer token.\n- name: ISNBearer\n  type: http\n  scheme: bearer\n  used_for: >-\n    Every resource call after the token exchange. The token is passed using the\n    standard Authorization: Bearer <token> header.\nflow:\n- step: 1\n  operation: GET https://api.isnetworld.com/token\n  headers: [Content-Type, UserKey, CompanyKey]\n  returns: a bearer token\n  probed_status: 401\n  probed_content_type: application/problem+json\n- step: 2\n  operation: GET https://api.isnetworld.com/validate-token\n  headers: [Authorization]\n  returns: boolean validity of the presented bearer token\n  probed_status: 401\n  probed_note: >-\n    Answers with an application/json body of `false` when no valid bearer token is\n    presented.\n- step: 3\n  operation: any /1.0/ resource path\n  headers: [Authorization]\n  probed_status: 401\ntoken:\n  expires: true\n  renewal: >-\n    ISN documents that tokens expire and are renewed by repeating the\
  \ /token exchange\n    with the UserKey and CompanyKey pair. ISN publishes no token lifetime value, so\n    none is recorded here.\n  lifetime_seconds: null\noauth2: false\nopenid_connect: false\nmutual_tls: false\ncredential_provisioning: >-\n  UserKey and CompanyKey are issued to subscribers by ISN; there is no public\n  self-service key generation, no developer signup, and no public key-management page.\ndocs: null\ndocs_note: >-\n  ISN publishes no public authentication reference. The API's own help surface at\n  https://api.isnetworld.com/help is itself authentication-gated (HTTP 401 probed\n  2026-08-23), and the Developer Integration Guide is distributed to subscribers.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/isn/refs/heads/main/authentication/isn-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Contractor Management
- Supplier Management
- Health Safety and Environment
- Risk Management
- Compliance
- Supply Chain
- Sustainability
- Workforce
- Insurance
- Training
- Enterprise Software
---
