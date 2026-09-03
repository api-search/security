---
api_key_in:
- header
auth_types:
- apiKey
- oauth2
- openIdConnect
- hmac
- totp
description: ''
kind: authentication
layout: security
method: searched
name: Api Dynamics Authentication
name_suffix: Authentication
oauth_flows: []
overview: API Dynamics secures its APIs with apiKey, oauth2, openIdConnect, hmac, and totp across 5 declared security schemes, as derived from its OpenAPI definitions.
provider_name: API Dynamics
provider_slug: api-dynamics
scheme_count: 5
schemes:
- confidence: medium
  description: The API provider's public key, sent by the protected service on every call it makes to the APIDynamics adaptive-authentication service. Identifies the tenant.
  evidence:
    file: src/main/java/com/apidynamics/test/server_demo/service/AdaptiveAuthenticationService.java
    kind: third-party-integration-demo
    url: https://github.com/gitguru/adaptive-auth-java-server
  in: header
  name: X-API-Dynamics-Provider-Id
  type: apiKey
- confidence: medium
  description: The calling API client's public key, forwarded from the inbound request so APIDynamics can score and validate that specific client.
  evidence:
    file: src/main/java/com/apidynamics/test/server_demo/filter/AdaptiveAuthenticationFilter.java
    kind: third-party-integration-demo
    url: https://github.com/gitguru/adaptive-auth-java-server
  in: header
  name: X-API-Dynamics-Client-Id
  type: apiKey
- confidence: high
  description: Time-based one-time password issued and validated by APIDynamics as the step-up factor for API-to-API multi-factor authentication.
  evidence:
    kind: provider-docs
    quote: Step-up MFA via TOTP, token headers, or HMAC-based authentication
    url: https://www.apidynamics.com/platform
  name: TOTP step-up
  type: totp
- confidence: high
  description: HMAC request signing for service-to-service authentication, offered as an alternative to header-token enforcement.
  evidence:
    kind: provider-docs
    url: https://www.apidynamics.com/hmac-api-to-api-authentication
  name: HMAC API-to-API
  type: hmac
- confidence: low
  description: APIDynamics markets an OAuth 2.0 / OIDC authentication surface for the APIs it protects. No authorization or token endpoint, and no scope list, is published anywhere public — so no flow could be recorded and scopes/ was deliberately not written.
  evidence:
    kind: provider-docs
    url: https://www.apidynamics.com/oauth-oidc-apidynamics-api-authentication
  name: OAuth 2.0 / OpenID Connect
  type: oauth2
slug: api-dynamics-authentication
source_filename: api-dynamics-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: searched\nsource: https://www.apidynamics.com/platform\ndocs: https://www.apidynamics.com/documentation\nnote: >-\n  APIDynamics publishes no OpenAPI, so this profile could not be derived mechanically.\n  It is assembled from two sources, kept separate below: (a) what APIDynamics states on\n  its own product pages, and (b) header and endpoint names observed in a public\n  third-party integration demo that is configured against the APIDynamics developer host.\n  Nothing here is invented; every scheme carries its evidence and its confidence.\nsummary:\n  types: [apiKey, oauth2, openIdConnect, hmac, totp]\n  api_key_in: [header]\n  oauth2_flows: []\n  spec_backed: false\n  confidence: medium\nschemes:\n- name: X-API-Dynamics-Provider-Id\n  type: apiKey\n  in: header\n  description: >-\n    The API provider's public key, sent by the protected service on every call it makes to\n    the APIDynamics adaptive-authentication service. Identifies the tenant.\n\
  \  confidence: medium\n  evidence:\n    kind: third-party-integration-demo\n    url: https://github.com/gitguru/adaptive-auth-java-server\n    file: src/main/java/com/apidynamics/test/server_demo/service/AdaptiveAuthenticationService.java\n- name: X-API-Dynamics-Client-Id\n  type: apiKey\n  in: header\n  description: >-\n    The calling API client's public key, forwarded from the inbound request so APIDynamics\n    can score and validate that specific client.\n  confidence: medium\n  evidence:\n    kind: third-party-integration-demo\n    url: https://github.com/gitguru/adaptive-auth-java-server\n    file: src/main/java/com/apidynamics/test/server_demo/filter/AdaptiveAuthenticationFilter.java\n- name: TOTP step-up\n  type: totp\n  description: >-\n    Time-based one-time password issued and validated by APIDynamics as the step-up factor\n    for API-to-API multi-factor authentication.\n  confidence: high\n  evidence:\n    kind: provider-docs\n    url: https://www.apidynamics.com/platform\n\
  \    quote: 'Step-up MFA via TOTP, token headers, or HMAC-based authentication'\n- name: HMAC API-to-API\n  type: hmac\n  description: >-\n    HMAC request signing for service-to-service authentication, offered as an alternative\n    to header-token enforcement.\n  confidence: high\n  evidence:\n    kind: provider-docs\n    url: https://www.apidynamics.com/hmac-api-to-api-authentication\n- name: OAuth 2.0 / OpenID Connect\n  type: oauth2\n  description: >-\n    APIDynamics markets an OAuth 2.0 / OIDC authentication surface for the APIs it protects.\n    No authorization or token endpoint, and no scope list, is published anywhere public —\n    so no flow could be recorded and scopes/ was deliberately not written.\n  confidence: low\n  evidence:\n    kind: provider-docs\n    url: https://www.apidynamics.com/oauth-oidc-apidynamics-api-authentication\nobserved_surface:\n  note: >-\n    OWNERSHIP AND PROVENANCE. These endpoints were NOT harvested from an APIDynamics-published\n    contract\
  \ — no such contract exists publicly. They were read out of a public Spring Boot\n    integration demo (gitguru/adaptive-auth-java-server, package com.apidynamics.test) whose\n    application.properties is configured against the APIDynamics developer host that\n    APIDynamics itself links from https://www.apidynamics.com/developers and /platform.\n    They are recorded as OBSERVED, not as a specification, and no OpenAPI was authored from\n    them. The base host does not currently resolve, so none of them could be probed live.\n  base_url: https://developer.apidynamics.sevenhills.ai/api/dynamics\n  base_url_status: unreachable\n  base_url_dns: NOERROR, no A record (probed 2026-09-02)\n  operations:\n  - method: GET\n    path: /totp/client/generate\n    query: [tid]\n    headers: [X-API-Dynamics-Provider-Id, X-API-Dynamics-Client-Id]\n    purpose: Ask APIDynamics to issue a TOTP for a named API client within a transaction.\n  - method: GET\n    path: /totp/server/validate\n    query: [tid,\
  \ totp]\n    headers: [X-API-Dynamics-Provider-Id]\n    purpose: Validate a TOTP against a transaction id.\n  - method: POST\n    path: /adaptive/server/validate\n    headers: [X-API-Dynamics-Provider-Id]\n    request_fields: [client_id, client_request_headers, client_request_endpoint, client_request_method]\n    purpose: Score an inbound API call and return an allow/step-up/deny decision.\n  response_envelope:\n    success: '{ transaction_id, validation_result: { score, decision } }'\n    error: '{ error, detail }'\nx-evidence:\n  fetched: '2026-09-02'\n  probes:\n  - url: https://www.apidynamics.com/platform\n    status: 200\n  - url: https://www.apidynamics.com/documentation\n    status: 200\n  - url: https://developer.apidynamics.sevenhills.ai/api/dynamics/adaptive/server/validate\n    status: '<no response> (host does not resolve)'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/api-dynamics/refs/heads/main/authentication/api-dynamics-authentication.yml
summary_line: apiKey/oauth2/openIdConnect/hmac/totp · 5 schemes
tags:
- API Security
- API Discovery
- API Observability
- Zero Trust
- API Intelligence
---
