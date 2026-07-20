---
api_key_in:
- request-body
auth_types:
- custom-hmac-signature
description: ''
kind: authentication
layout: security
method: searched
name: Learnosity Authentication
name_suffix: Authentication
oauth_flows: []
overview: Learnosity secures its APIs with custom-hmac-signature across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Learnosity
provider_slug: learnosity
scheme_count: 1
schemes:
- algorithm: HMAC-SHA256
  credentials:
  - description: Public account identifier supplied by Learnosity, sent in the security object.
    name: consumer_key
    secret: false
  - description: Private key supplied by Learnosity, used only as the HMAC key. Must never be sent to the browser or across the network, and is never part of the pre-hash string.
    name: consumer_secret
    secret: true
  domain_binding: The `domain` value must match the domain actually serving the page/app; Learnosity checks the request originates from one of the consumer's authorized domains.
  location: request body (`security` object)
  name: LearnositySignedRequest
  pre_hash_rule: Concatenate the signature components in order, underscore-separated, with the JSON representation of the request object appended last; HMAC-SHA256 that string using consumer_secret as the key, then prepend `$02$` to the hex digest.
  replay_protection: timestamp in the security object (gmdate('Ymd-Hi') format)
  signature_components:
  - consumer_key
  - domain
  - timestamp
  - user_id
  - JSON-encoded request object
  signature_length: 68
  signature_version_prefix: $02$
  type: signature
slug: learnosity-authentication
source_filename: learnosity-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://help.learnosity.com/hc/en-us/articles/360000754738-Security-and-Authentication\ndocs: https://help.learnosity.com/hc/en-us/articles/360000754738-Security-and-Authentication\nsummary:\n  types:\n  - custom-hmac-signature\n  api_key_in:\n  - request-body\n  oauth2_flows: []\n  notes: >-\n    Learnosity does not use OAuth 2.0, OpenID Connect, bearer tokens, or HTTP\n    header API keys. Every request to every Learnosity API (client-side JS APIs\n    and the server-side Data API alike) carries a `security` object inside the\n    request body, signed server-side with HMAC-SHA256.\nschemes:\n- name: LearnositySignedRequest\n  type: signature\n  algorithm: HMAC-SHA256\n  location: request body (`security` object)\n  signature_version_prefix: $02$\n  signature_length: 68\n  credentials:\n  - name: consumer_key\n    description: Public account identifier supplied by Learnosity, sent in the security object.\n    secret: false\n\
  \  - name: consumer_secret\n    description: >-\n      Private key supplied by Learnosity, used only as the HMAC key. Must never be\n      sent to the browser or across the network, and is never part of the pre-hash string.\n    secret: true\n  signature_components:\n  - consumer_key\n  - domain\n  - timestamp\n  - user_id\n  - JSON-encoded request object\n  pre_hash_rule: >-\n    Concatenate the signature components in order, underscore-separated, with the\n    JSON representation of the request object appended last; HMAC-SHA256 that string\n    using consumer_secret as the key, then prepend `$02$` to the hex digest.\n  domain_binding: >-\n    The `domain` value must match the domain actually serving the page/app; Learnosity\n    checks the request originates from one of the consumer's authorized domains.\n  replay_protection: timestamp in the security object (gmdate('Ymd-Hi') format)\npii_constraints:\n  user_id:\n    must_not_contain_pii: true\n    recommended_format: UUID\n    max_length:\
  \ 50\n    docs: https://help.learnosity.com/hc/en-us/articles/360002309578-Student-Privacy-and-Personally-Identifiable-Information-PII-\ntransport:\n  https_required: true\n  note: >-\n    Requesting Data API endpoints over HTTP instead of HTTPS returns 403 Forbidden.\nimplementation_guidance: >-\n  Learnosity strongly recommends using one of the six official SDKs\n  (Node.js, PHP, Python, ASP.NET, Java, Ruby) rather than hand-rolling the signature;\n  see packages/learnosity-packages.yml. Writing your own signing code is supported\n  only after contacting Learnosity Support.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/learnosity/refs/heads/main/authentication/learnosity-authentication.yml
summary_line: custom-hmac-signature · 1 scheme
tags:
- Education
- Assessment
- EdTech
- Learning
- Analytics
- Content Authoring
- Artificial Intelligence
- Accessibility
- Company
---
