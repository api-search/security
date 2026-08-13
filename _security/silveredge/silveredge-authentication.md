---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Silveredge Authentication
name_suffix: Authentication
oauth_flows: []
overview: Silveredge declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Silveredge
provider_slug: silveredge
scheme_count: 2
schemes:
- description: Publisher id provided by Silverpush. Declared required in the first-party bid-parameter JSON Schema published upstream at prebid-server/static/bidder-params/silverpush.json. It identifies the seller account the bid request is attributed to; it is not a secret and it is not a bearer credential.
  in: body
  issued_by: Silverpush, on approval
  location: imp[].ext.prebid.bidder.silverpush.publisherId
  name: publisherId
  required: true
  spec: json-schema/silveredge-prebid-bidder-params.json
  type: identifier
- description: A fixed routing parameter baked into the endpoint URL registered in prebid-server/static/bidder-info/silverpush.yaml (https://prebid.chocolateplatform.co/bidder/?identifier=prebidchoc). It selects the integration path, not the caller — it is identical for every Prebid caller and carries no per-tenant secret.
  in: query
  location: ?identifier=prebidchoc
  name: identifier
  required: true
  type: query-parameter
slug: silveredge-authentication
source_filename: silveredge-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: searched\nsource: >-\n  https://docs.prebid.org/dev-docs/bidders/silverpush.html and\n  https://github.com/prebid/prebid-server/blob/master/static/bidder-info/silverpush.yaml\ndocs: https://docs.prebid.org/dev-docs/bidders/silverpush.html\napi: Silverpush Prebid Bidder (Chocolate Ad Exchange)\nsummary: >-\n  Silverpush publishes no REST API, no OAuth surface and no API-key programme.\n  The only publicly documented way to authenticate against a Silverpush endpoint\n  is the programmatic one: a publisher is onboarded manually by Silverpush, is\n  issued a publisherId, and that identifier is carried inside every OpenRTB bid\n  request the Prebid client or Prebid Server sends to the Chocolate bid endpoint.\n  There is no self-service credential issuance, no token endpoint, no key\n  rotation policy and no scope model published anywhere.\nmodel: partner-identifier\nself_service: false\nschemes:\n- name: publisherId\n  type: identifier\n  in: body\n\
  \  location: imp[].ext.prebid.bidder.silverpush.publisherId\n  required: true\n  issued_by: Silverpush, on approval\n  description: >-\n    Publisher id provided by Silverpush. Declared required in the first-party\n    bid-parameter JSON Schema published upstream at\n    prebid-server/static/bidder-params/silverpush.json. It identifies the seller\n    account the bid request is attributed to; it is not a secret and it is not\n    a bearer credential.\n  spec: json-schema/silveredge-prebid-bidder-params.json\n- name: identifier\n  type: query-parameter\n  in: query\n  location: \"?identifier=prebidchoc\"\n  required: true\n  description: >-\n    A fixed routing parameter baked into the endpoint URL registered in\n    prebid-server/static/bidder-info/silverpush.yaml\n    (https://prebid.chocolateplatform.co/bidder/?identifier=prebidchoc). It\n    selects the integration path, not the caller — it is identical for every\n    Prebid caller and carries no per-tenant secret.\nonboarding:\n  self_service:\
  \ false\n  gate: manual approval\n  contact: prebid@silverpush.co\n  quote: >-\n    \"The Silverpush Bidder Adapter requires setup and approval before use.\n    Please reach out to prebid@silverpush.co representative for more details.\"\n    — github.com/prebid/Prebid.js/blob/master/modules/silverpushBidAdapter.md\ngaps:\n- No OAuth 2.0, OIDC, mTLS or API-key scheme is documented on any host.\n- No /.well-known/oauth-authorization-server or /.well-known/openid-configuration is served.\n- No credential rotation, expiry or revocation policy is published.\n- The publisherId is an account identifier, not an authenticated credential; transport-level trust is whatever the OpenRTB HTTPS connection provides.\nx-evidence:\n  fetched: '2026-08-12'\n  probes:\n  - url: https://docs.prebid.org/dev-docs/bidders/silverpush.html\n    status: 200\n  - url: https://raw.githubusercontent.com/prebid/prebid-server/master/static/bidder-info/silverpush.yaml\n    status: 200\n  - url: https://raw.githubusercontent.com/prebid/prebid-server/master/static/bidder-params/silverpush.json\n\
  \    status: 200\n  - url: https://silverpush.co/.well-known/oauth-authorization-server\n    status: 404\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/silveredge/refs/heads/main/authentication/silveredge-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Advertising
- AdTech
- Contextual Intelligence
- Artificial Intelligence
- Video Advertising
- Marketing
- Programmatic Advertising
- OpenRTB
- Prebid
- Supply Side Platform
- CTV
- Mobile Advertising
- Brand Safety
---
