---
api_key_in:
- header
auth_types:
- http-bearer
- token
description: ''
kind: authentication
layout: security
method: searched
name: Soundtrackyourbrand Authentication
name_suffix: Authentication
oauth_flows: []
overview: Soundtrack Your Brand secures its APIs with http-bearer and token across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Soundtrack Your Brand
provider_slug: soundtrackyourbrand
scheme_count: 1
schemes:
- description: 'API token issued from the Soundtrack account settings (https://app.soundtrack.io/accounts/_/settings/api) or requested via the apiAccessRequest mutation / partner program. Sent as `Authorization: Basic <token>` per the Soundtrack docs; the token scopes access to the account(s) it was issued for.'
  header: Authorization
  in: header
  name: apiToken
  scheme: bearer
  token_management: https://app.soundtrack.io/accounts/_/settings/api
  type: http
slug: soundtrackyourbrand-authentication
source_filename: soundtrackyourbrand-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://api.soundtrackyourbrand.com/v2/docs/the-basics\ndocs: https://api.soundtrackyourbrand.com/v2/docs\nsummary:\n  types: [http-bearer, token]\n  api_key_in: [header]\n  oauth2_flows: []\n  notes: >-\n    Soundtrack API is a GraphQL API authenticated with an API token passed in\n    the HTTP Authorization header. The API is free for paying Soundtrack\n    customers. There is also an in-API login flow (loginUser / loginDevice /\n    generateOTP / loginOTP / refreshLogin mutations) that returns a token for\n    apps acting on behalf of a user or device, as an alternative to a\n    pre-provisioned API token.\nschemes:\n- name: apiToken\n  type: http\n  scheme: bearer\n  in: header\n  header: Authorization\n  description: >-\n    API token issued from the Soundtrack account settings\n    (https://app.soundtrack.io/accounts/_/settings/api) or requested via the\n    apiAccessRequest mutation / partner program. Sent as\n    `Authorization:\
  \ Basic <token>` per the Soundtrack docs; the token scopes\n    access to the account(s) it was issued for.\n  token_management: https://app.soundtrack.io/accounts/_/settings/api\nlogin_flow:\n  description: >-\n    Alternative to a static API token — authenticate a user or device in-band\n    and receive a session token.\n  operations:\n  - loginUser\n  - loginDevice\n  - generateOTP\n  - loginOTP\n  - refreshLogin\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/soundtrackyourbrand/refs/heads/main/authentication/soundtrackyourbrand-authentication.yml
summary_line: http-bearer/token · 1 scheme
tags:
- Company
- Music
- Streaming
- Business Music
- Media
- Entertainment
- GraphQL
- Playback Control
- Retail
---
