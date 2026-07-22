---
api_key_in:
- header
- query
api_specs:
- filename: vanilla-api-openapi-original.json
  format: json
  label: Vanilla API v2
  slug: vanilla-api-v2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vanilla-forums/refs/heads/main/openapi/vanilla-api-openapi-original.json
auth_types:
- http bearer (personal access token)
- http bearer (JWT)
- apiKey in query (access_token)
- apiKey in query (role-token)
description: Authentication profile for the Vanilla (Higher Logic Vanilla) API v2. The platform-generated OpenAPI declares no securitySchemes, so this profile is documented from the provider's own authentication articles. All tokens carry the permissions of the user they represent (Vanilla roles and permissions).
kind: authentication
layout: security
method: searched
name: Vanilla Forums Authentication
name_suffix: Authentication
oauth_flows: []
overview: Vanilla Forums secures its APIs with http bearer (personal access token), http bearer (JWT), apiKey in query (access_token), and apiKey in query (role-token) across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Vanilla Forums
provider_slug: vanilla-forums
scheme_count: 3
schemes:
- description: 'Personal access tokens are generated from the user profile (Edit Profile > Access Tokens > Generate New Token; requires the Garden > Tokens > Add permission). Intended for server-to-server integrations. Preferred usage is the Authorization header with the bearer scheme ("Authorization: Bearer <token>"); the token may instead be passed as the access_token query-string parameter when custom headers are not possible, at the cost of appearing in server logs. API calls reflect the permissions of the user who generated the token.'
  docs: https://success.vanillaforums.com/kb/articles/41-authenticating-apiv2-calls-with-personal-access-tokens
  name: personalAccessToken
  scheme: bearer
  type: http
- bearerFormat: JWT
  description: 'The JWT addon authenticates API v2 calls with an RFC 7519 JSON Web Token passed as an RFC 6750 bearer token. Supported algorithm HS256; required claims: iss, sub (the SSO UniqueID), aud, email, displayname, exp, and iat or nbf; optional picture. The JWT is signed with the shared secret configured in the JWT addon settings.'
  docs: https://success.vanillaforums.com/kb/articles/122-authenticating-api-v2-calls-with-jwt
  name: jwtBearer
  scheme: bearer
  type: http
- description: Role tokens are short-lived signed JWTs (valid 1-3 minutes on a two-minute expiry window with one-minute rollover) carrying claims about Roles only - no user identity - so responses can be HTTP-cached and shared across users with identical permissions. Issued to an already-authorized user via POST /api/v2/tokens/roles and passed as the role-token query parameter. Valid only on GET /api/v2/users/:userID, GET /api/v2/subcommunities, and GET /api/v2/products.
  docs: https://success.vanillaforums.com/kb/articles/436-authenticating-api-v2-calls-with-role-tokens
  in: query
  name: roleToken
  parameter: role-token
  type: apiKey
slug: vanilla-forums-authentication
source_filename: vanilla-forums-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: >-\n  https://success.vanillaforums.com/kb/articles/41-authenticating-apiv2-calls-with-personal-access-tokens\n  + https://success.vanillaforums.com/kb/articles/122-authenticating-api-v2-calls-with-jwt\n  + https://success.vanillaforums.com/kb/articles/436-authenticating-api-v2-calls-with-role-tokens\n  + https://success.vanillaforums.com/kb/articles/326-authenticate-api-v2-calls-as-another-user-spoofing\ndocs: https://success.vanillaforums.com/kb/categories/97-api-and-webhooks\ndescription: >-\n  Authentication profile for the Vanilla (Higher Logic Vanilla) API v2. The\n  platform-generated OpenAPI declares no securitySchemes, so this profile is\n  documented from the provider's own authentication articles. All tokens carry\n  the permissions of the user they represent (Vanilla roles and permissions).\nsummary:\n  types: [http bearer (personal access token), http bearer (JWT), apiKey in query (access_token), apiKey in query\
  \ (role-token)]\n  api_key_in: [header, query]\n  oauth2_flows: []\nschemes:\n  - name: personalAccessToken\n    type: http\n    scheme: bearer\n    description: >-\n      Personal access tokens are generated from the user profile (Edit Profile\n      > Access Tokens > Generate New Token; requires the Garden > Tokens > Add\n      permission). Intended for server-to-server integrations. Preferred usage\n      is the Authorization header with the bearer scheme\n      (\"Authorization: Bearer <token>\"); the token may instead be passed as the\n      access_token query-string parameter when custom headers are not possible,\n      at the cost of appearing in server logs. API calls reflect the\n      permissions of the user who generated the token.\n    docs: https://success.vanillaforums.com/kb/articles/41-authenticating-apiv2-calls-with-personal-access-tokens\n  - name: jwtBearer\n    type: http\n    scheme: bearer\n    bearerFormat: JWT\n    description: >-\n      The JWT addon authenticates\
  \ API v2 calls with an RFC 7519 JSON Web Token\n      passed as an RFC 6750 bearer token. Supported algorithm HS256; required\n      claims: iss, sub (the SSO UniqueID), aud, email, displayname, exp, and\n      iat or nbf; optional picture. The JWT is signed with the shared secret\n      configured in the JWT addon settings.\n    docs: https://success.vanillaforums.com/kb/articles/122-authenticating-api-v2-calls-with-jwt\n  - name: roleToken\n    type: apiKey\n    in: query\n    parameter: role-token\n    description: >-\n      Role tokens are short-lived signed JWTs (valid 1-3 minutes on a\n      two-minute expiry window with one-minute rollover) carrying claims about\n      Roles only - no user identity - so responses can be HTTP-cached and\n      shared across users with identical permissions. Issued to an\n      already-authorized user via POST /api/v2/tokens/roles and passed as the\n      role-token query parameter. Valid only on GET /api/v2/users/:userID,\n      GET /api/v2/subcommunities,\
  \ and GET /api/v2/products.\n    docs: https://success.vanillaforums.com/kb/articles/436-authenticating-api-v2-calls-with-role-tokens\nnotes:\n  - Guest (unauthenticated) requests are served with edge HTTP caching (2-minute TTL) and see only what guests can see.\n  - >-\n    Spoofing: an access token with admin access (Garden > Settings > Manage)\n    can make any API v2 call as another user by passing the X-Vanilla-Spoof\n    header with the target userID (or a smart ID such as $name:frank or\n    $saml:<ssoid>); the call is limited to the spoofed user's permissions.\n    Server-side only - never pass spoof headers from clients.\n  - No OAuth 2.0 authorization-server flow is published for the API; SSO products (jsConnect, SAML, OAuth SSO addons) govern web sign-in rather than API token issuance.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vanilla-forums/refs/heads/main/authentication/vanilla-forums-authentication.yml
summary_line: http bearer (personal access token)/http bearer (JWT)/apiKey in query (access_token)/apiKey in query (role-token) · 3 schemes
tags:
- Community
- Forums
- Community Management
- Webhooks
- Customer Experience
- Knowledge Base
- SaaS
---
