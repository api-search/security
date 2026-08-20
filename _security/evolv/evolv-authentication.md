---
api_key_in:
- path
api_specs:
- filename: evolv-participant-api.postman_collection.json
  format: json
  label: Evolv Participant API
  slug: evolv-participant-api
  spec_type: Postman
  url: https://raw.githubusercontent.com/api-evangelist/evolv/refs/heads/main/postman/evolv-participant-api.postman_collection.json
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: searched
name: Evolv Authentication
name_suffix: Authentication
oauth_flows: []
overview: Evolv secures its APIs with apiKey and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Evolv
provider_slug: evolv
scheme_count: 3
schemes:
- description: The Participant API is keyed by a public environment id embedded in the request URL path (https://participants.evolv.ai/v1/{environment_id}/...). The environment id scopes all configuration, allocation, preallocation and event-ingestion requests to a specific Evolv project/environment. It is a publishable (client-side) key delivered in the browser snippet or mobile app SDK config — not a secret.
  in: path
  name: environmentId
  sources:
  - postman/evolv-participant-api.postman_collection.json (every request path is {{root_domain}}/{{participant_api_version}}/{{environment_id}}/...)
  - evolv-ai/android-sdk EvolvConfig.java (DEFAULT_ENDPOINT https://participants.evolv.ai/v1)
  type: apiKey
- description: A participant/visitor identifier (uid), and optionally a session id (sid), identify the subject of the request. They are carried as query parameters on the GET operations and as form fields on the POST/PATCH operations. Both are minted and persisted by the Evolv SDK (format `<random>_<epoch-millis>`), not issued by Evolv as an account credential — they are identity, not authorization.
  in: query
  name: participantUid
  sources:
  - postman/evolv-participant-api.postman_collection.json
  - evolv-ai/javascript-sdk src/index.js
  type: apiKey
- description: Evolv's own published Postman collection declares collection-level auth of `{"type":"bearer","bearer":{"token":"<token>"}}`, so a bearer token is the intended credential for at least some Participant API usage. No published documentation explains how that token is issued, scoped, rotated or revoked, and no individual operation in the collection overrides or annotates it.
  in: header
  name: bearerToken
  observability: The declaration could not be confirmed against the live API anonymously. Unauthenticated calls to the routed endpoints return HTTP 404 `{"msg":"Not found"}` rather than 401 or 403, so the API does not distinguish "unauthenticated" from "unknown environment" on the wire and enforcement cannot be observed without a real environment id. Recorded as declared by the provider, not as verified by probe.
  scheme: bearer
  sources:
  - postman/evolv-participant-api.postman_collection.json (collection `auth` block)
  status: declared-not-observable
  type: http
slug: evolv-authentication
source_filename: evolv-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: >-\n  Evolv-published Postman collection at developers.evolv.ai\n  (postman/evolv-participant-api.postman_collection.json) + Evolv SDK source\n  (evolv-ai/javascript-sdk build-options.js, evolv-ai/android-sdk EvolvConfig.java) +\n  live probes of https://participants.evolv.ai/v1/...\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - path\n  http_schemes:\n  - bearer\n  oauth2_flows: []\nschemes:\n- name: environmentId\n  type: apiKey\n  in: path\n  description: >-\n    The Participant API is keyed by a public environment id embedded in the request URL\n    path (https://participants.evolv.ai/v1/{environment_id}/...). The environment id scopes\n    all configuration, allocation, preallocation and event-ingestion requests to a specific\n    Evolv project/environment. It is a publishable (client-side) key delivered in the\n    browser snippet or mobile app SDK config — not a secret.\n  sources:\n  - postman/evolv-participant-api.postman_collection.json\
  \ (every request path is\n    {{root_domain}}/{{participant_api_version}}/{{environment_id}}/...)\n  - evolv-ai/android-sdk EvolvConfig.java (DEFAULT_ENDPOINT https://participants.evolv.ai/v1)\n- name: participantUid\n  type: apiKey\n  in: query\n  description: >-\n    A participant/visitor identifier (uid), and optionally a session id (sid), identify the\n    subject of the request. They are carried as query parameters on the GET operations and\n    as form fields on the POST/PATCH operations. Both are minted and persisted by the Evolv\n    SDK (format `<random>_<epoch-millis>`), not issued by Evolv as an account credential —\n    they are identity, not authorization.\n  sources:\n  - postman/evolv-participant-api.postman_collection.json\n  - evolv-ai/javascript-sdk src/index.js\n- name: bearerToken\n  type: http\n  scheme: bearer\n  in: header\n  status: declared-not-observable\n  description: >-\n    Evolv's own published Postman collection declares collection-level auth of\n    `{\"\
  type\":\"bearer\",\"bearer\":{\"token\":\"<token>\"}}`, so a bearer token is the intended\n    credential for at least some Participant API usage. No published documentation\n    explains how that token is issued, scoped, rotated or revoked, and no individual\n    operation in the collection overrides or annotates it.\n  observability: >-\n    The declaration could not be confirmed against the live API anonymously. Unauthenticated\n    calls to the routed endpoints return HTTP 404 `{\"msg\":\"Not found\"}` rather than 401 or\n    403, so the API does not distinguish \"unauthenticated\" from \"unknown environment\" on the\n    wire and enforcement cannot be observed without a real environment id. Recorded as\n    declared by the provider, not as verified by probe.\n  sources:\n  - postman/evolv-participant-api.postman_collection.json (collection `auth` block)\nmanagement_api:\n  status: undocumented\n  detail: >-\n    Authoring and management of experiments happens in the Evolv Manager\
  \ console\n    (https://app.evolv.ai, HTTP 200, login required) and via the first-party\n    experiment-management-cli, both against an authenticated Evolv account. Evolv publishes\n    no reference for that management surface, so no scheme for it is recorded here.\ndocs: https://developers.evolv.ai/\nnotes: >-\n  There is no OAuth, no OpenID Connect, no scope model and no mTLS on the Evolv runtime\n  surface; `scopes/` is therefore correctly absent rather than empty. This profile is built\n  from Evolv's published Postman collection and SDK source because Evolv publishes no\n  OpenAPI. The bearer scheme is recorded exactly as strongly as the evidence supports —\n  declared by Evolv, unverifiable anonymously.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/evolv/refs/heads/main/authentication/evolv-authentication.yml
summary_line: apiKey/http · 3 schemes
tags:
- Experimentation
- Optimization
- Personalization
- A/B Testing
- Machine-Learning
- Conversion Rate Optimization
- Experience Optimization
- Analytics
- Company
---
