---
anonymous_access: false
api_key_in: []
api_specs:
- filename: hot-mic-presence-api-openapi.yml
  format: yaml
  label: Hot Mic Presence API
  slug: hot-mic-presence-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hot-mic/refs/heads/main/openapi/hot-mic-presence-api-openapi.yml
- filename: hot-mic-streams-api-openapi.yml
  format: yaml
  label: Hot Mic Streams API
  slug: hot-mic-streams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hot-mic/refs/heads/main/openapi/hot-mic-streams-api-openapi.yml
- filename: hot-mic-studio-api-openapi.yml
  format: yaml
  label: Hot Mic Studio API
  slug: hot-mic-studio-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hot-mic/refs/heads/main/openapi/hot-mic-studio-api-openapi.yml
- filename: hot-mic-users-api-openapi.yml
  format: yaml
  label: Hot Mic Users API
  slug: hot-mic-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/hot-mic/refs/heads/main/openapi/hot-mic-users-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Hot Mic Authentication
name_suffix: Authentication
oauth_flows: []
overview: Hot Mic declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Hot Mic
provider_slug: hot-mic
scheme_count: 1
schemes:
- evidence: All requests are authenticated with an API key issued by HotMic.
  header: x-api-key
  how_to_obtain: API key issued by HotMic
  location: header
  name: x-api-key
  type: apiKey
slug: hot-mic-authentication
source_filename: hot-mic-authentication.yml
source_heading: Authentication Profile
source_url: https://hotmic.io/docs/api
source_yaml: "generated: '2026-10-12'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://hotmic.io/docs/api\nsources:\n- https://hotmic.io/docs/api\n- https://hotmic.io/docs/platform/orgs\n- https://hotmic.io/docs/platform/onboarding\nschemes:\n- type: apiKey\n  name: x-api-key\n  evidence: All requests are authenticated with an API key issued by HotMic.\n  location: header\n  header: x-api-key\n  how_to_obtain: API key issued by HotMic\ndocs: https://hotmic.io/docs/api\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hot-mic/refs/heads/main/authentication/hot-mic-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Video
- LiveStreaming
- CreatorContent
- SDK
---
