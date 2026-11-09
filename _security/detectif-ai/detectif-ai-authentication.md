---
anonymous_access: false
api_key_in: []
api_specs:
- filename: detectif-ai-api-openapi.json
  format: json
  label: DetectifAI Developer API API
  slug: detectifai-developer-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/detectif-ai/openapi/_original/detectif-ai-api-openapi.json
auth_types: []
description: Detectif.ai uses API keys that are sent as bearer tokens in the Authorization header. For Noesis WebSocket connections a stream token can be passed in the URL query string.
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Detectif Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Detectif.ai declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Detectif.ai
provider_slug: detectif-ai
scheme_count: 2
schemes:
- evidence: 'Every request needs an API key, sent as a bearer token in the `Authorization` header:'
  header: Authorization
  how_to_obtain: Create keys under **API keys** in the dashboard; a key is shown once when you create it.
  location: header
  name: API key
  type: http-bearer
- evidence: 'Some clients cannot set headers on a WebSocket: Twilio `<Stream>`, a browser, or a telephony provider where you only enter a URL. For these, your server creates a stream token for each call and the client passes it instead of the key:'
  how_to_obtain: Create a stream token by POSTing to `/v1/detect/stream-tokens` with an API key in the Authorization header.
  location: query
  name: Stream token
  type: other
slug: detectif-ai-authentication
source_filename: detectif-ai-authentication.yml
source_heading: Authentication Profile
source_url: https://platform.detectif.ai/docs/authentication.md
source_yaml: "generated: '2026-11-05'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://platform.detectif.ai/docs/authentication.md\nsources:\n- https://platform.detectif.ai/docs/authentication.md\n- https://platform.detectif.ai/docs/noesis/authentication.md\n- https://platform.detectif.ai/docs/authentication\n- https://platform.detectif.ai/docs/noesis/authentication\ndescription: Detectif.ai uses API keys that are sent as bearer tokens in the Authorization header. For Noesis WebSocket connections a stream token\n  can be passed in the URL query string.\nschemes:\n- type: http-bearer\n  name: API key\n  evidence: 'Every request needs an API key, sent as a bearer token in the `Authorization` header:'\n  location: header\n  header: Authorization\n  how_to_obtain: Create keys under **API keys** in the dashboard; a key is shown once when you create it.\n- type: other\n  name: Stream token\n  evidence: 'Some clients cannot set headers on a WebSocket: Twilio `<Stream>`,\
  \ a browser, or a telephony provider where you only enter a URL.\n    For these, your server creates a stream token for each call and the client passes it instead of the key:'\n  location: query\n  how_to_obtain: Create a stream token by POSTing to `/v1/detect/stream-tokens` with an API key in the Authorization header.\nnote: No OAuth2 flows are documented for Detectif.ai.\ndocs: https://platform.detectif.ai/docs/authentication.md\n"
source_yaml_url: https://artifacts.apis.io/detectif-ai/authentication/detectif-ai-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Artificial Intelligence
- Voice
- Deepfake
- Security
- Audio
---
