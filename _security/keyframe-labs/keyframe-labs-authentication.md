---
api_key_in: []
api_specs:
- filename: keyframe-labs-sessions-openapi-original.json
  format: json
  label: Keyframe Sessions API
  slug: keyframe-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/keyframe-labs/refs/heads/main/openapi/keyframe-labs-sessions-openapi-original.json
auth_types:
- http
description: 'The Keyframe Sessions API is authenticated with a bearer API key. Create and manage keys in the Keyframe platform dashboard (https://platform.keyframelabs.com/api-keys); a key is shown only once at creation. Pass the key as an HTTP bearer token in the Authorization header (Authorization: Bearer <api_key>) on every request.'
kind: authentication
layout: security
method: searched
name: Keyframe Labs Authentication
name_suffix: Authentication
oauth_flows: []
overview: Keyframe Labs secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Keyframe Labs
provider_slug: keyframe-labs
scheme_count: 1
schemes:
- docs: https://docs.keyframelabs.com/guides/getting-started/get-your-api-key
  format: Bearer <api_key>
  header: Authorization
  in: header
  key_management: https://platform.keyframelabs.com/api-keys
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/keyframe-labs-sessions-openapi-original.json
  type: http
slug: keyframe-labs-authentication
source_filename: keyframe-labs-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: openapi/keyframe-labs-sessions-openapi-original.json\ndocs: https://docs.keyframelabs.com/guides/getting-started/get-your-api-key\nsummary:\n  types:\n  - http\n  http_schemes:\n  - bearer\ndescription: >-\n  The Keyframe Sessions API is authenticated with a bearer API key. Create and\n  manage keys in the Keyframe platform dashboard (https://platform.keyframelabs.com/api-keys);\n  a key is shown only once at creation. Pass the key as an HTTP bearer token in\n  the Authorization header (Authorization: Bearer <api_key>) on every request.\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  in: header\n  header: Authorization\n  format: 'Bearer <api_key>'\n  docs: https://docs.keyframelabs.com/guides/getting-started/get-your-api-key\n  key_management: https://platform.keyframelabs.com/api-keys\n  sources:\n  - openapi/keyframe-labs-sessions-openapi-original.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/keyframe-labs/refs/heads/main/authentication/keyframe-labs-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- AI
- Avatars
- Video
- Conversational AI
- Agents
- Real-Time
- Personas
- Voice
- Y Combinator
---
