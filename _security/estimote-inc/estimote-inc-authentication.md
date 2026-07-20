---
api_key_in:
- header
auth_types:
- oauth2
- http
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Estimote Inc Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Estimote Inc secures its APIs with oauth2, http, and apiKey across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Estimote Inc
provider_slug: estimote-inc
scheme_count: 2
schemes:
- authorizationUrl: https://cloud.estimote.com/v1/oauth2/authorize
  flow: authorizationCode
  name: OAuth2
  note: Authorization Code grant only, intended for server-side applications where the client secret can be protected. Not suitable for mobile or JavaScript apps. Credentials issued on request during private beta.
  sources:
  - https://developer.estimote.com/cloud/oauth/
  status: private-beta
  tokenUrl: https://cloud.estimote.com/v1/oauth2/access_token
  token_usage: 'Authorization: Bearer <token>'
  type: oauth2
- description: App ID and App Token credential pair (created in Estimote Cloud) passed via HTTP Basic Authorization header to authenticate REST API requests.
  name: AppToken
  scheme: basic
  sources:
  - https://cloud.estimote.com/docs/
  type: http
slug: estimote-inc-authentication
source_filename: estimote-inc-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://developer.estimote.com/cloud/oauth/ and https://cloud.estimote.com/docs/\ndocs: https://developer.estimote.com/cloud/oauth/\nsummary:\n  types: [oauth2, http, apiKey]\n  api_key_in: [header]\n  oauth2_flows: [authorizationCode]\n  notes: >-\n    Estimote Cloud REST API accepts OAuth 2.0 (authorization code grant, server-side apps)\n    with a Bearer access token, or an App ID + App Token credential pair passed as an HTTP\n    Basic Authorization header for direct API access.\nschemes:\n- name: OAuth2\n  type: oauth2\n  flow: authorizationCode\n  authorizationUrl: https://cloud.estimote.com/v1/oauth2/authorize\n  tokenUrl: https://cloud.estimote.com/v1/oauth2/access_token\n  token_usage: \"Authorization: Bearer <token>\"\n  status: private-beta\n  note: >-\n    Authorization Code grant only, intended for server-side applications where the client\n    secret can be protected. Not suitable for mobile or JavaScript apps.\
  \ Credentials issued\n    on request during private beta.\n  sources: [https://developer.estimote.com/cloud/oauth/]\n- name: AppToken\n  type: http\n  scheme: basic\n  description: >-\n    App ID and App Token credential pair (created in Estimote Cloud) passed via HTTP Basic\n    Authorization header to authenticate REST API requests.\n  sources: [https://cloud.estimote.com/docs/]\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/estimote-inc/refs/heads/main/authentication/estimote-inc-authentication.yml
summary_line: oauth2/http/apiKey · 2 schemes
tags:
- Company
- Proximity
- Beacons
- Bluetooth
- BLE
- UWB
- Ultra Wideband
- LTE
- IoT
- Indoor Location
- Asset Tracking
- RTLS
- Sensors
- Hardware
---
