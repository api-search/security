---
api_key_in: []
auth_types:
- none
- contract-gated
- session-login
description: ''
kind: authentication
layout: security
method: probed
name: Nsw Land Registry Authentication
name_suffix: Authentication
oauth_flows: []
overview: NSW Land Registry Services secures its APIs with none, contract-gated, and session-login across 6 declared security schemes, as derived from its OpenAPI definitions.
provider_name: NSW Land Registry Services
provider_slug: nsw-land-registry
scheme_count: 6
schemes:
- documented: true
  evidence: GET /api/v2/status.json, /api/v2/summary.json, /api/v2/components.json, /api/v2/incidents.json and /api/v2/scheduled-maintenances.json all returned HTTP 200 with Content-Type application/json and no credential of any kind on 2026-07-26. The published API reference at https://status.nswlrs.com.au/api documents the endpoints with plain curl examples and describes no authentication step.
  host: https://status.nswlrs.com.au/api/v2
  name: none
  surface: NSW LRS status page API
  type: none
- documented: false
  evidence: The Cantaloupe endpoint root, an info.json and a /full/200,/0/default.jpg derivative all returned HTTP 200 anonymously on 2026-07-26. No key issuance, no token, no rate-limit header.
  host: https://api.lrsnative.com.au/hlrv/iiif/2
  name: none
  surface: HLRV IIIF Image API
  type: none
- documented: false
  enforced: false
  evidence: The HLRV single-page application configures its ReactiveSearch client with an x-portal-token header, but POST /hlrv/documents/_msearch returned HTTP 200 with hits.total 7160622 on 2026-07-26 with no header supplied. The header exists in the client, is not enforced at the edge, and is not documented anywhere by NSW LRS.
  host: https://api.lrsnative.com.au/hlrv/documents
  in: header
  name: x-portal-token
  parameter_name: x-portal-token
  surface: HLRV document search proxy
  type: apiKey
- documented: false
  evidence: 'Every path probed on api.nswlrs.com.au returned HTTP 403 {"message":"Forbidden"} with x-amzn-errortype ForbiddenException from AWS API Gateway, including /, /v1, /health, /docs, /openapi.json and /.well-known/openid-configuration. The status page publishes an "API Service" component under the Information Broker Services group, confirming a production API exists for licensed brokers. Access is granted by an official licence agreement: "Only an information broker we''ve authorised can access our records."'
  host: https://api.nswlrs.com.au
  name: broker-licence
  surface: NSW LRS broker API estate (api.nswlrs.com.au)
  type: contract
- documented: true
  evidence: Writes to the Torrens Title Register are lodged through an Electronic Lodgment Network Operator (PEXA or Sympli) under the Electronic Conveyancing National Law; subscribers are registered under the NSW Participation Rules and examined under NSW LRS's delegated section 33 ECNL compliance authority. No direct machine credential is issued by NSW LRS.
  name: elno-subscriber
  surface: Lodgment and dealing writes
  type: contract
- documented: true
  evidence: connect.nswlrs.com.au is a login-gated OutSystems application for lodging parties; online.nswlrs.com.au is an IBM WebSphere Portal offering web-form searches. Both are human-interactive sessions with no published programmatic authentication.
  host: https://connect.nswlrs.com.au
  name: portal-login
  surface: NSW LRS Connect / NSW LRS Online Portal
  type: session
slug: nsw-land-registry-authentication
source_filename: nsw-land-registry-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-26'\nmethod: probed\nsource: >-\n  live anonymous probes of every reachable NSW LRS host plus the published access statements at\n  nswlrs.com.au; no OpenAPI securitySchemes exist to derive from\ndocs: https://nswlrs.com.au/services/record-searches/how-to-find-an-information-broker\nsummary:\n  types:\n  - none\n  - contract-gated\n  - session-login\n  api_key_in: []\n  oauth2_flows: []\n  note: >-\n    NSW Land Registry Services publishes no authentication documentation, issues no API keys and\n    operates no OAuth or OpenID Connect surface that can be reached anonymously. Authentication in\n    this estate is either absent (the two undocumented public read surfaces and the status page\n    API) or replaced entirely by a commercial licence: register access is authorised by a broker\n    licence agreement or by ELNO subscriber registration, not by a credential a developer can\n    obtain online.\nschemes:\n- name: none\n  type: none\n  surface: NSW LRS\
  \ status page API\n  host: https://status.nswlrs.com.au/api/v2\n  documented: true\n  evidence: >-\n    GET /api/v2/status.json, /api/v2/summary.json, /api/v2/components.json,\n    /api/v2/incidents.json and /api/v2/scheduled-maintenances.json all returned HTTP 200 with\n    Content-Type application/json and no credential of any kind on 2026-07-26. The published API\n    reference at https://status.nswlrs.com.au/api documents the endpoints with plain curl examples\n    and describes no authentication step.\n- name: none\n  type: none\n  surface: HLRV IIIF Image API\n  host: https://api.lrsnative.com.au/hlrv/iiif/2\n  documented: false\n  evidence: >-\n    The Cantaloupe endpoint root, an info.json and a /full/200,/0/default.jpg derivative all\n    returned HTTP 200 anonymously on 2026-07-26. No key issuance, no token, no rate-limit header.\n- name: x-portal-token\n  type: apiKey\n  in: header\n  parameter_name: x-portal-token\n  surface: HLRV document search proxy\n  host: https://api.lrsnative.com.au/hlrv/documents\n\
  \  documented: false\n  enforced: false\n  evidence: >-\n    The HLRV single-page application configures its ReactiveSearch client with an x-portal-token\n    header, but POST /hlrv/documents/_msearch returned HTTP 200 with hits.total 7160622 on\n    2026-07-26 with no header supplied. The header exists in the client, is not enforced at the\n    edge, and is not documented anywhere by NSW LRS.\n- name: broker-licence\n  type: contract\n  surface: NSW LRS broker API estate (api.nswlrs.com.au)\n  host: https://api.nswlrs.com.au\n  documented: false\n  evidence: >-\n    Every path probed on api.nswlrs.com.au returned HTTP 403 {\"message\":\"Forbidden\"} with\n    x-amzn-errortype ForbiddenException from AWS API Gateway, including /, /v1, /health, /docs,\n    /openapi.json and /.well-known/openid-configuration. The status page publishes an \"API Service\"\n    component under the Information Broker Services group, confirming a production API exists for\n    licensed brokers. Access is granted\
  \ by an official licence agreement: \"Only an information\n    broker we've authorised can access our records.\"\n- name: elno-subscriber\n  type: contract\n  surface: Lodgment and dealing writes\n  documented: true\n  evidence: >-\n    Writes to the Torrens Title Register are lodged through an Electronic Lodgment Network Operator\n    (PEXA or Sympli) under the Electronic Conveyancing National Law; subscribers are registered\n    under the NSW Participation Rules and examined under NSW LRS's delegated section 33 ECNL\n    compliance authority. No direct machine credential is issued by NSW LRS.\n- name: portal-login\n  type: session\n  surface: NSW LRS Connect / NSW LRS Online Portal\n  host: https://connect.nswlrs.com.au\n  documented: true\n  evidence: >-\n    connect.nswlrs.com.au is a login-gated OutSystems application for lodging parties;\n    online.nswlrs.com.au is an IBM WebSphere Portal offering web-form searches. Both are\n    human-interactive sessions with no published programmatic\
  \ authentication.\ngaps:\n- No API key issuance, no OAuth 2.0, no OpenID Connect and no mutual TLS is published anywhere.\n- No /.well-known/openid-configuration or /.well-known/oauth-authorization-server exists on any host.\n- 'The only credential that reaches register data is commercial: a broker licence or ELNO subscription.'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nsw-land-registry/refs/heads/main/authentication/nsw-land-registry-authentication.yml
summary_line: none/contract-gated/session-login · 6 schemes
tags:
- Real-Estate
- Australia
- Land Registry
- Title
- Conveyancing
- Property Records
- Torrens Title
- eConveyancing
- Government
- Geospatial
- PropTech
---
