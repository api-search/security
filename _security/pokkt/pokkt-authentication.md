---
api_key_in:
- query
- path
auth_types:
- apiKey
- custom-hash-signature
- undocumented-header
description: ''
kind: authentication
layout: security
method: searched
name: Pokkt Authentication
name_suffix: Authentication
oauth_flows: []
overview: Pokkt secures its APIs with apiKey, custom-hash-signature, and undocumented-header across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Pokkt
provider_slug: pokkt
scheme_count: 4
schemes:
- applies_to:
  - ad-server-api
  - vast-video-api
  - mobile-web-video-api
  in: query
  issued_by: POKKT dashboard ("Your unique App ID (available in POKKT dashboard)")
  name: appId
  note: The appId is the caller's whole identity on the ad-serving surface. It is mandatory, it travels in the URL, and there is no accompanying secret, signature or token on the request.
  parameter: appId
  secret: false
  source: https://wiki.pokkt.com/api-guide/interstitial-api.md
  type: apiKey
- applies_to:
  - dsp-openrtb
  endpoint_pattern: https://vdo.pokkt.com/api/rtb/<yourappid>
  in: path
  issued_by: account manager ("Please reach out to your account manager for App ID details")
  name: appId-path-segment
  parameter: <yourappid>
  secret: false
  source: https://wiki.pokkt.com/dsp-integration-guide/pokkt-dsp.md
  type: apiKey
- algorithm: md5
  applies_to:
  - gratification-api
  direction: POKKT -> publisher
  in: query
  name: gratification-callback-token
  note: The only shared secret POKKT documents. It authenticates POKKT's outbound reward callback to the publisher's endpoint, not the publisher's calls to POKKT. MD5 over concatenated fields is not an HMAC; there is no signature header, no key id, no algorithm agility and no documented rotation procedure.
  parameter: token
  secret_location: app settings page in the POKKT console
  signed_input: app_id + unique_id + timestamp + points + app secret key
  source: https://wiki.pokkt.com/api-guide/gratification-api.md
  type: custom-hash-signature
- applies_to:
  - console-graphql
  evidence: An anonymous POST of the introspection query to https://api.pokkt.com/graphql on 2026-08-12 returned {"errors":[{"extensions":{"payload":{"status":401,"message":"Invalid authorization header format"}}}]}. The header is therefore required; its format, issuance and lifetime are not published anywhere.
  in: header
  method: probed
  name: console-authorization-header
  parameter: Authorization
  source: https://api.pokkt.com/graphql
  type: undocumented-header
slug: pokkt-authentication
source_filename: pokkt-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: searched\nsource: >-\n  https://wiki.pokkt.com/api-guide/interstitial-api.md,\n  https://wiki.pokkt.com/api-guide/gratification-api.md,\n  https://wiki.pokkt.com/dsp-integration-guide/pokkt-dsp.md,\n  live probe of https://api.pokkt.com/graphql\ndocs: https://wiki.pokkt.com/api-guide\nnote: >-\n  Derived by hand from POKKT's own documentation and one live unauthenticated probe, because\n  there is no OpenAPI to mine securitySchemes from. POKKT has no OAuth, no OIDC, no scopes and no\n  key-rotation story; identity on the public ad surface is a plain appId in the query string,\n  and the only cryptographic material anywhere is a shared app secret key used to MD5-sign the\n  rewarded-video callback back to the publisher.\n\nsummary:\n  types: [apiKey, custom-hash-signature, undocumented-header]\n  api_key_in: [query, path]\n  oauth2_flows: []\n  openid_connect: false\n  mutual_tls: false\n  bearer_tokens: false\n\nschemes:\n- name: appId\n  type:\
  \ apiKey\n  in: query\n  parameter: appId\n  applies_to: [ad-server-api, vast-video-api, mobile-web-video-api]\n  issued_by: POKKT dashboard (\"Your unique App ID (available in POKKT dashboard)\")\n  secret: false\n  note: >-\n    The appId is the caller's whole identity on the ad-serving surface. It is mandatory, it\n    travels in the URL, and there is no accompanying secret, signature or token on the request.\n  source: https://wiki.pokkt.com/api-guide/interstitial-api.md\n- name: appId-path-segment\n  type: apiKey\n  in: path\n  parameter: '<yourappid>'\n  applies_to: [dsp-openrtb]\n  endpoint_pattern: 'https://vdo.pokkt.com/api/rtb/<yourappid>'\n  issued_by: 'account manager (\"Please reach out to your account manager for App ID details\")'\n  secret: false\n  source: https://wiki.pokkt.com/dsp-integration-guide/pokkt-dsp.md\n- name: gratification-callback-token\n  type: custom-hash-signature\n  in: query\n  parameter: token\n  algorithm: md5\n  signed_input: app_id + unique_id +\
  \ timestamp + points + app secret key\n  secret_location: app settings page in the POKKT console\n  direction: POKKT -> publisher\n  applies_to: [gratification-api]\n  note: >-\n    The only shared secret POKKT documents. It authenticates POKKT's outbound reward callback to\n    the publisher's endpoint, not the publisher's calls to POKKT. MD5 over concatenated fields is\n    not an HMAC; there is no signature header, no key id, no algorithm agility and no documented\n    rotation procedure.\n  source: https://wiki.pokkt.com/api-guide/gratification-api.md\n- name: console-authorization-header\n  type: undocumented-header\n  in: header\n  parameter: Authorization\n  applies_to: [console-graphql]\n  method: probed\n  evidence: >-\n    An anonymous POST of the introspection query to https://api.pokkt.com/graphql on 2026-08-12\n    returned {\"errors\":[{\"extensions\":{\"payload\":{\"status\":401,\"message\":\"Invalid authorization\n    header format\"}}}]}. The header is therefore required;\
  \ its format, issuance and lifetime are\n    not published anywhere.\n  source: https://api.pokkt.com/graphql\n\npublisher_side_credentials:\n  app_secret_key:\n    where: app settings page in the POKKT console\n    used_for: MD5 token on the rewarded-video server-side callback\n    rotation_documented: false\n  callback_url:\n    where: app settings page in the POKKT console\n    note: 'Documentation calls it a \"secure rewarded server-side callback\" but does not require HTTPS in the published request format.'\n\nnot_found:\n- {mechanism: OAuth 2.0, probed: '/.well-known/oauth-authorization-server + /.well-known/oauth-protected-resource on 5 hosts, developer wiki', result: absent}\n- {mechanism: OpenID Connect, probed: /.well-known/openid-configuration on 5 hosts, result: absent}\n- {mechanism: scopes / permissions model, probed: developer wiki, result: absent — scopes/ deliberately not written}\n- {mechanism: mutual TLS, probed: developer wiki, result: absent}\n- {mechanism: key rotation\
  \ or revocation policy, probed: developer wiki, result: absent}\n- {mechanism: public self-service key issuance, probed: pokkt.com, result: 'absent — pokkt.com root is the console login SPA; access is account-manager mediated'}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pokkt/refs/heads/main/authentication/pokkt-authentication.yml
summary_line: apiKey/custom-hash-signature/undocumented-header · 4 schemes
tags:
- Company
- Advertising
- Monetization
- Mobile
- Video Advertising
- AdTech
- Remarketing
- OpenRTB
- Programmatic Advertising
- Rewarded Video
- Mobile SDK
- Ad Serving
- Connected TV
- Supply Side Platform
- Demand-Side Platform
---
