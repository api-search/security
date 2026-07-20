---
api_key_in:
- path
api_specs:
- filename: postman.yaml
  format: yaml
  label: Evolv Participant API
  slug: evolv-participant-api
  spec_type: Postman
  url: https://developers.evolv.ai/
auth_types:
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Evolv Authentication
name_suffix: Authentication
oauth_flows: []
overview: Evolv secures its APIs with apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Evolv
provider_slug: evolv
scheme_count: 2
schemes:
- description: The Participant API is keyed by a public environment id embedded in the request URL path (https://participants.evolv.ai/v1/{environment}/...). The environment id scopes all configuration, allocation, and event-ingestion requests to a specific Evolv project/environment. It is a publishable (client-side) key delivered in the browser or mobile app snippet.
  in: path
  name: environmentId
  sources:
  - evolv-ai/android-sdk EvolvConfig.java (DEFAULT_ENDPOINT https://participants.evolv.ai/v1)
  type: apiKey
- description: A participant/visitor identifier (uid), and optionally a session id (sid), are passed in the request path to fetch that participant's allocations and to attribute ingested events. Identity is managed by the SDK, not an account credential.
  in: path
  name: participantUid
  sources:
  - evolv-ai/javascript-sdk src/index.js
  type: apiKey
slug: evolv-authentication
source_filename: evolv-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: >-\n  Evolv SDK source (evolv-ai/javascript-sdk build-options.js, evolv-ai/android-sdk\n  EvolvConfig.java) + developers.evolv.ai Participant API reference\nsummary:\n  types:\n  - apiKey\n  api_key_in:\n  - path\n  oauth2_flows: []\nschemes:\n- name: environmentId\n  type: apiKey\n  in: path\n  description: >-\n    The Participant API is keyed by a public environment id embedded in the request URL\n    path (https://participants.evolv.ai/v1/{environment}/...). The environment id scopes\n    all configuration, allocation, and event-ingestion requests to a specific Evolv\n    project/environment. It is a publishable (client-side) key delivered in the browser\n    or mobile app snippet.\n  sources:\n  - evolv-ai/android-sdk EvolvConfig.java (DEFAULT_ENDPOINT https://participants.evolv.ai/v1)\n- name: participantUid\n  type: apiKey\n  in: path\n  description: >-\n    A participant/visitor identifier (uid), and optionally a session\
  \ id (sid), are passed\n    in the request path to fetch that participant's allocations and to attribute ingested\n    events. Identity is managed by the SDK, not an account credential.\n  sources:\n  - evolv-ai/javascript-sdk src/index.js\nnotes: >-\n  The runtime Participant API uses no OAuth or bearer token — access is by public\n  environment id plus participant uid over HTTPS. Management/authoring of experiments\n  (via the Evolv app and the experiment-management-cli) is performed against the\n  authenticated Evolv account, separate from this runtime edge API. No OpenAPI is\n  published, so this profile is derived from the official SDK source rather than a spec.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/evolv/refs/heads/main/authentication/evolv-authentication.yml
summary_line: apiKey · 2 schemes
tags:
- Experimentation
- Optimization
- Personalization
- A/B Testing
- Machine Learning
- Conversion Rate Optimization
- Experience Optimization
- Analytics
- Company
---
