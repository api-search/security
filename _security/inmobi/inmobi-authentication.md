---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Inmobi Authentication
name_suffix: Authentication
oauth_flows: []
overview: InMobi declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: InMobi
provider_slug: inmobi
scheme_count: 3
schemes:
- api: InMobi Publisher Reporting API 3.0
  credentials:
  - description: Account email address registered on the InMobi publisher platform.
    location: header
    name: userName
  - description: API key generated from the InMobi publisher dashboard.
    location: header
    name: secretKey
  - description: InMobi account identifier.
    location: header
    name: accountId
  - description: Session token returned by the session-generation call; may exceed 1000 characters.
    location: header
    name: sessionId
  docs: https://support.inmobi.com/monetize/inmobi-apis/reporting-api
  evidence:
    body: '{"error":true,"errorList":[{"code":1004,"message":"Secret Key is missing"}]}'
    http_status: 400
    method: POST
    note: Unauthenticated POST is rejected with the documented error code 1004, confirming the secretKey header is the enforced credential. A POST to the documented session endpoint https://api.inmobi.com/v1.0/generatesession/generate returned HTTP 404 with a JSON error envelope on 2026-08-12 — the host routes the path but the documented generatesession route did not answer, which may mean the documentation is ahead of or behind the deployed route.
    probed: '2026-08-12'
    url: https://api.inmobi.com/v3.0/reporting/publisher
  id: publisher-reporting-session
  in: header
  session:
    endpoint: https://api.inmobi.com/v1.0/generatesession/generate
    max_sessions: 15 per 8-hour window per API key
    method: POST
    request_headers:
    - userName
    - secretKey
    validity: 8 hours from issuance
  style: two-step-session
  type: apiKey
- api: InMobi Ad Management API
  credentials:
  - description: API key generated from the InMobi publisher platform (same key issuance flow as the Reporting API).
    location: header
    name: x-client-secret
  - description: Account ID, found under Payment Settings on the Finance tab of the InMobi platform.
    location: header
    name: x-account-id
  - description: Email address of the account.
    location: header
    name: x-client-id
  docs: https://support.inmobi.com/monetize/inmobi-apis/ad-management-api/authentication-and-request-protocol
  evidence:
    body: '{"error":true,"errors":[{"errorCode":"[ERROR_MISSING_HEADERS]","reason":"[x-account-id] header is missing"}]}'
    http_status: 401
    method: GET
    note: Anonymous GET names the missing header explicitly; supplying placeholder values for all three headers returned 401 {"errorCode":"AUTHENTICATION_ERROR"} — the triplet is enforced server-side.
    probed: '2026-08-12'
    url: https://publisher.inmobi.com/rest/api/v2/apps
  id: ad-management-static-headers
  in: header
  style: static-header-triplet
  transport: https only (stated in the provider docs)
  type: apiKey
- api: InMobi DSP Cost API
  credentials:
  - description: Token issued by the token endpoint; sent as the raw token value per the provider docs.
    location: header
    name: Authorization
  docs: https://support.inmobi.com/dsp/global/inmobi-dsp-global/reporting-for-inmobi-dsp-global/cost-api-integration-for-inmobi-dsp
  evidence:
    body: '{"status":"FAILED","code":400,"error":{"code":"client.cred.invalid","message":"The provided credentials are invalid. Please check your clientId & clientSecret and try again."},"message":"Request Processing Failed."}'
    http_status: 400
    method: POST
    note: Live token endpoint. Uses a client-credentials SHAPE (clientId / clientSecret) but is NOT an OAuth 2.0 token endpoint — the response is a custom envelope, not an RFC 6749 token response, and no /.well-known/oauth-authorization-server is served on this host (403).
    probed: '2026-08-12'
    url: https://api.cdr.inmobi.com/api/v3/auth/token
  id: dsp-cost-bearer-token
  in: header
  style: bearer-token
  token_endpoint:
    grant_inputs:
    - clientId
    - clientSecret
    method: POST
    url: https://api.cdr.inmobi.com/api/v3/auth/token
    validity: 8 hours
  type: http
slug: inmobi-authentication
source_filename: inmobi-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: searched\nsource: >-\n  https://support.inmobi.com/monetize/inmobi-apis/reporting-api ,\n  https://support.inmobi.com/monetize/inmobi-apis/ad-management-api/authentication-and-request-protocol ,\n  https://support.inmobi.com/dsp/global/inmobi-dsp-global/reporting-for-inmobi-dsp-global/cost-api-integration-for-inmobi-dsp\nnotes: >-\n  InMobi publishes no OpenAPI, so this profile is read from the provider's own\n  API reference pages and confirmed against live unauthenticated probes of each\n  host. Three distinct authentication schemes are in play across three\n  independently versioned APIs — there is no single InMobi auth model. All\n  schemes are custom header / bearer-token designs; InMobi documents no OAuth 2.0\n  authorization server, no OIDC discovery document, and no scope vocabulary.\nsummary:\n  scheme_count: 3\n  oauth2: false\n  openid_connect: false\n  mutual_tls: false\n  api_key: true\n  bearer_token: true\n  session_token: true\n\
  \  discovery_document: false\n\nschemes:\n- id: publisher-reporting-session\n  api: InMobi Publisher Reporting API 3.0\n  type: apiKey\n  in: header\n  style: two-step-session\n  docs: https://support.inmobi.com/monetize/inmobi-apis/reporting-api\n  credentials:\n  - name: userName\n    location: header\n    description: Account email address registered on the InMobi publisher platform.\n  - name: secretKey\n    location: header\n    description: API key generated from the InMobi publisher dashboard.\n  - name: accountId\n    location: header\n    description: InMobi account identifier.\n  - name: sessionId\n    location: header\n    description: Session token returned by the session-generation call; may exceed 1000 characters.\n  session:\n    endpoint: https://api.inmobi.com/v1.0/generatesession/generate\n    method: POST\n    request_headers:\n    - userName\n    - secretKey\n    validity: 8 hours from issuance\n    max_sessions: 15 per 8-hour window per API key\n  evidence:\n    probed:\
  \ '2026-08-12'\n    url: https://api.inmobi.com/v3.0/reporting/publisher\n    method: POST\n    http_status: 400\n    body: '{\"error\":true,\"errorList\":[{\"code\":1004,\"message\":\"Secret Key is missing\"}]}'\n    note: >-\n      Unauthenticated POST is rejected with the documented error code 1004,\n      confirming the secretKey header is the enforced credential. A POST to the\n      documented session endpoint https://api.inmobi.com/v1.0/generatesession/generate\n      returned HTTP 404 with a JSON error envelope on 2026-08-12 — the host routes\n      the path but the documented generatesession route did not answer, which may\n      mean the documentation is ahead of or behind the deployed route.\n\n- id: ad-management-static-headers\n  api: InMobi Ad Management API\n  type: apiKey\n  in: header\n  style: static-header-triplet\n  docs: https://support.inmobi.com/monetize/inmobi-apis/ad-management-api/authentication-and-request-protocol\n  credentials:\n  - name: x-client-secret\n\
  \    location: header\n    description: API key generated from the InMobi publisher platform (same key issuance flow as the Reporting API).\n  - name: x-account-id\n    location: header\n    description: Account ID, found under Payment Settings on the Finance tab of the InMobi platform.\n  - name: x-client-id\n    location: header\n    description: Email address of the account.\n  transport: https only (stated in the provider docs)\n  evidence:\n    probed: '2026-08-12'\n    url: https://publisher.inmobi.com/rest/api/v2/apps\n    method: GET\n    http_status: 401\n    body: '{\"error\":true,\"errors\":[{\"errorCode\":\"[ERROR_MISSING_HEADERS]\",\"reason\":\"[x-account-id] header is missing\"}]}'\n    note: >-\n      Anonymous GET names the missing header explicitly; supplying placeholder\n      values for all three headers returned 401\n      {\"errorCode\":\"AUTHENTICATION_ERROR\"} — the triplet is enforced server-side.\n\n- id: dsp-cost-bearer-token\n  api: InMobi DSP Cost API\n  type:\
  \ http\n  in: header\n  style: bearer-token\n  docs: https://support.inmobi.com/dsp/global/inmobi-dsp-global/reporting-for-inmobi-dsp-global/cost-api-integration-for-inmobi-dsp\n  credentials:\n  - name: Authorization\n    location: header\n    description: Token issued by the token endpoint; sent as the raw token value per the provider docs.\n  token_endpoint:\n    url: https://api.cdr.inmobi.com/api/v3/auth/token\n    method: POST\n    grant_inputs:\n    - clientId\n    - clientSecret\n    validity: 8 hours\n  evidence:\n    probed: '2026-08-12'\n    url: https://api.cdr.inmobi.com/api/v3/auth/token\n    method: POST\n    http_status: 400\n    body: '{\"status\":\"FAILED\",\"code\":400,\"error\":{\"code\":\"client.cred.invalid\",\"message\":\"The provided credentials are invalid. Please check your clientId & clientSecret and try again.\"},\"message\":\"Request Processing Failed.\"}'\n    note: >-\n      Live token endpoint. Uses a client-credentials SHAPE (clientId /\n      clientSecret)\
  \ but is NOT an OAuth 2.0 token endpoint — the response is a\n      custom envelope, not an RFC 6749 token response, and no\n      /.well-known/oauth-authorization-server is served on this host (403).\n\nunauthenticated_surfaces:\n- api: InMobi Server-to-Server Ad Request API 3.1\n  url: https://api.w.inmobi.com/showad/v3.1\n  note: >-\n    Ad-serving endpoint. No credential header is documented; the caller is\n    identified by an InMobi Property ID carried in the request payload. An\n    anonymous GET and POST both returned HTTP 204 on 2026-08-12 (live host,\n    no ad returned for an empty request).\n\ngaps:\n- no OAuth 2.0 or OpenID Connect authorization server\n- no /.well-known/openid-configuration or /.well-known/oauth-authorization-server on any InMobi host (all 404 or 403 — see well-known/inmobi-well-known.yml)\n- no documented scope or permission vocabulary; access is account-wide per API key\n- no documented key-rotation or key-revocation API\n- three different header conventions\
  \ across three APIs (secretKey vs x-client-secret vs Authorization)\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/inmobi/refs/heads/main/authentication/inmobi-authentication.yml
summary_line: 3 schemes
tags:
- Company
- Enterprise
- Advertising
- AdTech
- Mobile
- Monetization
- Programmatic
- OpenRTB
- SDK
- Consent Management
- DSP
- Reporting
---
