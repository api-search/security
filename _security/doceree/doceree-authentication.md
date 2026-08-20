---
api_key_in:
- query
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Doceree Authentication
name_suffix: Authentication
oauth_flows: []
overview: Doceree secures its APIs with apiKey across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Doceree
provider_slug: doceree
scheme_count: 3
schemes:
- description: 'The Doceree placement identifier that identifies the publisher ad slot making the request. Example form published in the Prebid.js bidder docs: DOC_7jm9j5eqkl0xvc5w. Required on GET /v1/adrequest; the Prebid.js adapter rejects a bid request without it (isBidRequestValid).'
  in: query
  name: placementId
  parameter: id
  required: true
  sources:
  - https://docs.prebid.org/dev-docs/bidders/doceree.html
  - https://github.com/prebid/Prebid.js/blob/master/modules/docereeBidAdapter.js
  type: apiKey
- description: Publisher token read from the Prebid.js `doceree.context` config (config.getConfig('doceree.context').token) and appended to the ad request. Identifies the publisher context alongside publisherDomain.
  in: query
  name: publisherToken
  parameter: token
  required: false
  sources:
  - https://github.com/prebid/Prebid.js/blob/master/modules/docereeBidAdapter.js
  type: apiKey
- description: Mobile application key sent by the Doceree iOS/Android ad SDKs on GET /v1/adrequest, alongside id, size and platformType. Issued when a publisher creates a Doceree account.
  in: query
  name: appKey
  parameter: appKey
  required: true
  sources:
  - https://github.com/doceree/ios-sdk/blob/master/DocereeAdsSdk/Repo/AdWebRepo.swift
  type: apiKey
slug: doceree-authentication
source_filename: doceree-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: searched\nsource: >-\n  https://servedbydoceree.doceree.com/script/render-header.js,\n  https://github.com/prebid/Prebid.js/blob/master/modules/docereeBidAdapter.js,\n  https://github.com/doceree/ios-sdk (DocereeAdsSdk/Repo/AdWebRepo.swift),\n  https://docs.prebid.org/dev-docs/bidders/doceree.html\ndocs: https://docs.prebid.org/dev-docs/bidders/doceree.html\nnote: >-\n  Doceree publishes no OpenAPI, so there are no machine-readable\n  securitySchemes to derive from. This profile is read from Doceree's own\n  public client code (the hosted publisher tag, the first-party Prebid.js\n  adapter, and the open-source iOS SDK). Authentication is publisher-identity\n  based and travels in the query string; there is no OAuth 2.0, OpenID Connect,\n  HTTP Basic/Bearer or mTLS surface on the public ad-serving endpoints.\nsummary:\n  types: [apiKey]\n  api_key_in: [query]\n  oauth2_flows: []\n  bearer: false\n  mtls: false\nschemes:\n- name: placementId\n\
  \  type: apiKey\n  in: query\n  parameter: id\n  required: true\n  description: >-\n    The Doceree placement identifier that identifies the publisher ad slot\n    making the request. Example form published in the Prebid.js bidder docs:\n    DOC_7jm9j5eqkl0xvc5w. Required on GET /v1/adrequest; the Prebid.js adapter\n    rejects a bid request without it (isBidRequestValid).\n  sources:\n  - https://docs.prebid.org/dev-docs/bidders/doceree.html\n  - https://github.com/prebid/Prebid.js/blob/master/modules/docereeBidAdapter.js\n- name: publisherToken\n  type: apiKey\n  in: query\n  parameter: token\n  required: false\n  description: >-\n    Publisher token read from the Prebid.js `doceree.context` config\n    (config.getConfig('doceree.context').token) and appended to the ad request.\n    Identifies the publisher context alongside publisherDomain.\n  sources:\n  - https://github.com/prebid/Prebid.js/blob/master/modules/docereeBidAdapter.js\n- name: appKey\n  type: apiKey\n  in: query\n  parameter:\
  \ appKey\n  required: true\n  description: >-\n    Mobile application key sent by the Doceree iOS/Android ad SDKs on\n    GET /v1/adrequest, alongside id, size and platformType. Issued when a\n    publisher creates a Doceree account.\n  sources:\n  - https://github.com/doceree/ios-sdk/blob/master/DocereeAdsSdk/Repo/AdWebRepo.swift\nidentity_context:\n  description: >-\n    Beyond credentialing, Doceree's ad request carries an HCP identity payload.\n    The Prebid.js adapter base64-encodes a URI-encoded JSON object from\n    config.getConfig('doceree.user').data onto the `loggedInUser` query\n    parameter; the hosted publisher tag builds the same value from a\n    site-provided `hcpContext` object and a first-party Doceree cookie. This is\n    the input to Doceree's HCP identity-resolution layer, not an auth\n    credential.\n  parameters: [loggedInUser, publisherDomain, currentUrl, pubRequestedURL]\nconsent:\n  framework: IAB Europe Transparency & Consent Framework (TCF)\n  gvl_id: 1063\n\
  \  parameters:\n    gdpr: Flag indicating whether GDPR applies (string, e.g. \"1\")\n    gdpr_consent: URL-safe base64-encoded TCF consent string\n  note: >-\n    The Prebid.js adapter enforces that a consent string is present when\n    gdpr == 1 (isGdprConsentPresent). USP/CCPA and COPPA support are listed as\n    \"check with bidder\" in the Prebid bidder documentation.\ngaps:\n- No published authentication reference page on a Doceree-owned host; the\n  authoritative public reference is the Prebid bidder documentation.\n- Credentials travel as query parameters rather than headers, so they appear in\n  intermediary logs and referrer chains.\n- No documented key rotation, expiry, or scope model.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/doceree/refs/heads/main/authentication/doceree-authentication.yml
summary_line: apiKey · 3 schemes
tags:
- Advertising
- Healthcare
- Marketing
- AdTech
- Programmatic
- Header Bidding
- Life Sciences
- Pharmaceuticals
- Point of Care
- Identity Resolution
- Electronic Health Records
- Company
---
