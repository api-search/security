---
api_key_in:
- header
auth_types:
- apiKey
- http
description: 'Arena''s Platform API and SDKs authenticate over an Authorization header using one of two credential types: a site API Key, or a JSON Web Token (JWT). JWT is also the mechanism for Single Sign-On (SSO) so a host site can pass an already authenticated end user into Live Chat and Live Blog. There is no OpenAPI document published for Arena, so this profile is captured from the developer docs rather than derived from a spec.'
kind: authentication
layout: security
method: searched
name: Arena Authentication
name_suffix: Authentication
oauth_flows: []
overview: Arena secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Arena
provider_slug: arena
scheme_count: 2
schemes:
- description: Site API key sent in the Authorization header. The site slug and keys are obtained from the Arena Dashboard (dashboard.arena.im) or the Platform API.
  header: Authorization
  in: header
  name: apiKey
  sources:
  - https://developers.arena.im/
  type: apiKey
- bearerFormat: JWT
  description: JSON Web Token sent in the Authorization header. Also used to implement Single Sign-On (SSO) for Live Chat and Live Blog, passing a host site's authenticated user identity into Arena.
  name: jwt
  scheme: bearer
  sources:
  - https://help.arena.im/en/articles/5211494-documentation-for-developers
  type: http
slug: arena-authentication
source_filename: arena-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: searched\nsource: https://developers.arena.im/ + https://help.arena.im/en/articles/5211494-documentation-for-developers\ndocs: https://developers.arena.im/\ndescription: >-\n  Arena's Platform API and SDKs authenticate over an Authorization header using\n  one of two credential types: a site API Key, or a JSON Web Token (JWT). JWT is\n  also the mechanism for Single Sign-On (SSO) so a host site can pass an already\n  authenticated end user into Live Chat and Live Blog. There is no OpenAPI\n  document published for Arena, so this profile is captured from the developer\n  docs rather than derived from a spec.\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n  - name: apiKey\n    type: apiKey\n    in: header\n    header: Authorization\n    description: >-\n      Site API key sent in the Authorization header. The site slug and keys are\n      obtained from the Arena Dashboard (dashboard.arena.im) or the Platform API.\n\
  \    sources:\n    - https://developers.arena.im/\n  - name: jwt\n    type: http\n    scheme: bearer\n    bearerFormat: JWT\n    description: >-\n      JSON Web Token sent in the Authorization header. Also used to implement\n      Single Sign-On (SSO) for Live Chat and Live Blog, passing a host site's\n      authenticated user identity into Arena.\n    sources:\n    - https://help.arena.im/en/articles/5211494-documentation-for-developers\nsso:\n  supported: true\n  mechanism: JWT\n  applies_to:\n  - Live Chat\n  - Live Blog\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/arena/refs/heads/main/authentication/arena-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- Developer Tools
- Audience Engagement
- Live Chat
- Live Blog
- Comments
- Community
- Real-Time
- Moderation
- Media
---
