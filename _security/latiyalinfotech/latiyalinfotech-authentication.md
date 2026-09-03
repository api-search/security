---
api_key_in: []
api_specs:
- filename: 2sAY52cKG2
  format: yaml
  label: Cricket Live Line API
  slug: cricket-live-line-api
  spec_type: Postman
  url: https://documenter.getpostman.com/view/27917034/2sAY52cKG2
auth_types: []
description: ''
kind: authentication
layout: security
method: derived
name: Latiyalinfotech Authentication
name_suffix: Authentication
oauth_flows: []
overview: Latiyal Infotech declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Latiyal Infotech
provider_slug: latiyalinfotech
scheme_count: 2
schemes:
- applies_to: https://apicricketchampion.in/apiv{3,4,5}/{operation}/{api_token}
  distribution: direct contract; token issued by the provider after purchase (WhatsApp / sales)
  evidence: Every request in both published Postman collections is {{api_url}}{{api_plan}}/<operation>/{{api_token}} -- 51 of 51 in the v4/v5 collection and 30 of 30 in the v3 collection.
  in: path
  name: api_token_in_path
  note: 'A credential in the URL path is a real security finding, not a style choice: it lands in proxy logs, browser history, Referer headers and CDN access logs, and it cannot be rotated per-request or scoped. A header or Authorization scheme would cost the provider nothing and is the single highest-value auth change available to them.'
  parameter: api_token
  position: final path segment
  rotation_documented: false
  scopes: none
  type: apiKey
- additional_headers:
  - X-RapidAPI-Host: cricket-live-line4.p.rapidapi.com
  applies_to: https://cricket-live-line4.p.rapidapi.com
  distribution: self-serve; issued by RapidAPI on subscription to a plan
  evidence: The RapidAPI listing publishes cricket-live-line4.p.rapidapi.com as the public DNS for the API; RapidAPI's gateway enforces its standard X-RapidAPI-Key / X-RapidAPI-Host pair.
  in: header
  name: rapidapi_headers
  parameter: X-RapidAPI-Key
  rotation_documented: false
  scopes: none
  type: apiKey
slug: latiyalinfotech-authentication
source_filename: latiyalinfotech-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-01'\nmethod: derived\nsource: >-\n  postman/latiyalinfotech-cricket-live-line-v4-v5.postman_collection.json,\n  postman/latiyalinfotech-cricket-live-line-v3.postman_collection.json,\n  https://rapidapi.com/latiyalinfotechprivatelimited/api/cricket-live-line4,\n  live probe of https://apicricketchampion.in/apiv5/homeList/{api_token} (2026-09-01)\napi: Cricket Live Line API\nsummary: >-\n  Two distribution paths, two different credential models. Direct customers call\n  apicricketchampion.in with an opaque API token embedded as the LAST PATH SEGMENT of every\n  request; RapidAPI subscribers call the same API through cricket-live-line4.p.rapidapi.com\n  with the standard RapidAPI header pair. There is no OAuth, no OIDC, no mTLS, and no scope\n  system on either path. The provider publishes no dedicated authentication page -- the model\n  is only visible in the Postman collections and the RapidAPI listing.\nschemes:\n- name: api_token_in_path\n  type: apiKey\n\
  \  in: path\n  parameter: api_token\n  position: final path segment\n  applies_to: https://apicricketchampion.in/apiv{3,4,5}/{operation}/{api_token}\n  distribution: direct contract; token issued by the provider after purchase (WhatsApp / sales)\n  rotation_documented: false\n  scopes: none\n  evidence: >-\n    Every request in both published Postman collections is\n    {{api_url}}{{api_plan}}/<operation>/{{api_token}} -- 51 of 51 in the v4/v5 collection and\n    30 of 30 in the v3 collection.\n  note: >-\n    A credential in the URL path is a real security finding, not a style choice: it lands in\n    proxy logs, browser history, Referer headers and CDN access logs, and it cannot be rotated\n    per-request or scoped. A header or Authorization scheme would cost the provider nothing and\n    is the single highest-value auth change available to them.\n- name: rapidapi_headers\n  type: apiKey\n  in: header\n  parameter: X-RapidAPI-Key\n  additional_headers:\n  - X-RapidAPI-Host: cricket-live-line4.p.rapidapi.com\n\
  \  applies_to: https://cricket-live-line4.p.rapidapi.com\n  distribution: self-serve; issued by RapidAPI on subscription to a plan\n  rotation_documented: false\n  scopes: none\n  evidence: >-\n    The RapidAPI listing publishes cricket-live-line4.p.rapidapi.com as the public DNS for the\n    API; RapidAPI's gateway enforces its standard X-RapidAPI-Key / X-RapidAPI-Host pair.\nplan_selection:\n  mechanism: path segment\n  detail: >-\n    The plan tier is also carried in the path, not in the credential: {{api_plan}} resolves to\n    apiv3, apiv4 or apiv5 depending on the plan purchased. The provider states it plainly in the\n    v4/v5 collection description -- 'In Environments, the value of \"api_plan\" for v5 plan is\n    \"v5\" and for v4 plan is \"v4\"'.\nfailure_behavior:\n  http_status_on_invalid_credential: 200\n  body: '{\"status\": false, \"msg\": \"Invalid api key. ...\", \"data\": []}'\n  observed: '2026-09-01 against https://apicricketchampion.in/apiv5/homeList/{api_token}'\n\
  \  note: >-\n    Authentication failure is returned as HTTP 200 with status:false in the envelope. An agent\n    or client that branches on the HTTP status code will treat a rejected credential as success.\ngaps:\n- No published authentication reference page on latiyalinfotech.com.\n- No documented key rotation, revocation or expiry policy.\n- No 401/403 status codes; auth failures are 200 with an in-body flag.\n- No scopes, no least-privilege model, no per-key restriction documented.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/latiyalinfotech/refs/heads/main/authentication/latiyalinfotech-authentication.yml
summary_line: 2 schemes
tags:
- Cricket
- Sports
- Live Scores
- Sports Data
- Odds
- Fantasy Sports
- Real-Time Data
- Cricket API
- India
- Postman
---
