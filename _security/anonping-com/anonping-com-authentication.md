---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Anonping Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: AnonPing declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: AnonPing
provider_slug: anonping-com
scheme_count: 1
schemes:
- authorizationUrl: https://anonping.com/oauth/authorize
  flow: authorization_code
  scopes:
    anonping:match: Allows starting and managing matches
    anonping:read: Read conversation status and messages
    anonping:send: Send messages in a conversation
  tokenUrl: https://anonping.com/oauth/token
  type: oauth2
slug: anonping-com-authentication
source_filename: anonping-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: searched\nsource: https://anonping.com/.well-known/oauth-authorization-server\nschemes:\n  - type: oauth2\n    flow: authorization_code\n    authorizationUrl: https://anonping.com/oauth/authorize\n    tokenUrl: https://anonping.com/oauth/token\n    scopes:\n      anonping:match: \"Allows starting and managing matches\"\n      anonping:read: \"Read conversation status and messages\"\n      anonping:send: \"Send messages in a conversation\"\n"
source_yaml_url: https://artifacts.apis.io/anonping-com/authentication/anonping-com-authentication.yml
summary_line: 1 scheme
tags:
- Chat
- Anonymous
- Social
- Artificial Intelligence
- Privacy
---
