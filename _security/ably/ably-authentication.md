---
api_key_in: []
api_specs:
- filename: ably-apps-api-openapi.yml
  format: yaml
  label: Ably apps API
  slug: ably-apps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ably/refs/heads/main/openapi/ably-apps-api-openapi.yml
- filename: ably-authentication-api-openapi.yml
  format: yaml
  label: Ably Authentication API
  slug: ably-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ably/refs/heads/main/openapi/ably-authentication-api-openapi.yml
- filename: ably-history-api-openapi.yml
  format: yaml
  label: Ably History API
  slug: ably-history-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ably/refs/heads/main/openapi/ably-history-api-openapi.yml
- filename: ably-keys-api-openapi.yml
  format: yaml
  label: Ably keys API
  slug: ably-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ably/refs/heads/main/openapi/ably-keys-api-openapi.yml
- filename: ably-namespaces-api-openapi.yml
  format: yaml
  label: Ably namespaces API
  slug: ably-namespaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ably/refs/heads/main/openapi/ably-namespaces-api-openapi.yml
- filename: ably-publishing-api-openapi.yml
  format: yaml
  label: Ably Publishing API
  slug: ably-publishing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ably/refs/heads/main/openapi/ably-publishing-api-openapi.yml
- filename: ably-push-api-openapi.yml
  format: yaml
  label: Ably Push API
  slug: ably-push-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ably/refs/heads/main/openapi/ably-push-api-openapi.yml
- filename: ably-queues-api-openapi.yml
  format: yaml
  label: Ably queues API
  slug: ably-queues-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ably/refs/heads/main/openapi/ably-queues-api-openapi.yml
- filename: ably-rules-api-openapi.yml
  format: yaml
  label: Ably rules API
  slug: ably-rules-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ably/refs/heads/main/openapi/ably-rules-api-openapi.yml
- filename: ably-stats-api-openapi.yml
  format: yaml
  label: Ably Stats API
  slug: ably-stats-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ably/refs/heads/main/openapi/ably-stats-api-openapi.yml
- filename: ably-status-api-openapi.yml
  format: yaml
  label: Ably Status API
  slug: ably-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ably/refs/heads/main/openapi/ably-status-api-openapi.yml
- filename: ably-tokens-api-openapi.yml
  format: yaml
  label: Ably tokens API
  slug: ably-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ably/refs/heads/main/openapi/ably-tokens-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Ably Authentication
name_suffix: Authentication
oauth_flows: []
overview: Ably secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Ably
provider_slug: ably
scheme_count: 2
schemes:
- description: Control API uses bearer authentication. You need to generate an access token for use with this API. More details can be found in the <a href="https://ably.com/docs/account/control-api/#authentication">Ably docs</a>.
  name: bearer_auth
  scheme: bearer
  sources:
  - openapi/ably-control-api-openapi.yml
  - openapi/ably-platform-api-openapi.yml
  type: http
- description: Basic Authentication using an [API key](https://www.ably.io/documentation/core-features/authentication#basic-authentication).
  name: basicAuth
  scheme: basic
  sources:
  - openapi/ably-platform-api-openapi.yml
  type: http
slug: ably-authentication
source_filename: ably-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/ably-control-api-openapi.yml, openapi/ably-platform-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearer_auth\n  type: http\n  scheme: bearer\n  description: Control API uses bearer authentication. You need to generate an access token\n    for use with this API. More details can be found in the <a href=\"https://ably.com/docs/account/control-api/#authentication\">Ably\n    docs</a>.\n  sources:\n  - openapi/ably-control-api-openapi.yml\n  - openapi/ably-platform-api-openapi.yml\n- name: basicAuth\n  type: http\n  scheme: basic\n  description: Basic Authentication using an [API key](https://www.ably.io/documentation/core-features/authentication#basic-authentication).\n  sources:\n  - openapi/ably-platform-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ably/refs/heads/main/authentication/ably-authentication.yml
summary_line: http · 2 schemes
tags:
- Real-Time
- WebSockets
- Pub/Sub
- Messaging
- Streaming
- Push Notifications
- Chat
- LiveSync
---
