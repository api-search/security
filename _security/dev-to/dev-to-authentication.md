---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: dev-to-webhooks-asyncapi.yml
  format: yaml
  label: Dev.to Webhooks API
  slug: webhooks-api
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/dev-to/refs/heads/main/asyncapi/dev-to-webhooks-asyncapi.yml
- filename: dev-to-webhooks-api-openapi.yml
  format: yaml
  label: dev-to Webhooks API
  slug: dev-to-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dev-to/refs/heads/main/openapi/dev-to-webhooks-api-openapi.yml
- filename: dev-to-display-ads-api-openapi.yml
  format: yaml
  label: DEV Community Display Ads API
  slug: dev-to-display-ads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dev-to/refs/heads/main/openapi/dev-to-display-ads-api-openapi.yml
- filename: devto-agent-sessions-api-openapi.yml
  format: yaml
  label: DEV Community Agent Sessions API
  slug: devto-agent-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dev-to/refs/heads/main/openapi/devto-agent-sessions-api-openapi.yml
- filename: devto-articles-api-openapi.yml
  format: yaml
  label: DEV Community Articles API
  slug: devto-articles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dev-to/refs/heads/main/openapi/devto-articles-api-openapi.yml
- filename: devto-billboards-api-openapi.yml
  format: yaml
  label: DEV Community Billboards API
  slug: devto-billboards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dev-to/refs/heads/main/openapi/devto-billboards-api-openapi.yml
- filename: devto-comments-api-openapi.yml
  format: yaml
  label: DEV Community Comments API
  slug: devto-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dev-to/refs/heads/main/openapi/devto-comments-api-openapi.yml
- filename: devto-followed-tags-api-openapi.yml
  format: yaml
  label: DEV Community Followed Tags API
  slug: devto-followed-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dev-to/refs/heads/main/openapi/devto-followed-tags-api-openapi.yml
- filename: devto-followers-api-openapi.yml
  format: yaml
  label: DEV Community Followers API
  slug: devto-followers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dev-to/refs/heads/main/openapi/devto-followers-api-openapi.yml
- filename: devto-organizations-api-openapi.yml
  format: yaml
  label: DEV Community Organizations API
  slug: devto-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dev-to/refs/heads/main/openapi/devto-organizations-api-openapi.yml
- filename: devto-pages-api-openapi.yml
  format: yaml
  label: DEV Community Pages API
  slug: devto-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dev-to/refs/heads/main/openapi/devto-pages-api-openapi.yml
- filename: devto-podcast-episodes-api-openapi.yml
  format: yaml
  label: DEV Community Podcast Episodes API
  slug: devto-podcast-episodes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dev-to/refs/heads/main/openapi/devto-podcast-episodes-api-openapi.yml
- filename: devto-profile-images-api-openapi.yml
  format: yaml
  label: DEV Community profile images API
  slug: devto-profile-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dev-to/refs/heads/main/openapi/devto-profile-images-api-openapi.yml
- filename: devto-reactions-api-openapi.yml
  format: yaml
  label: DEV Community Reactions API
  slug: devto-reactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dev-to/refs/heads/main/openapi/devto-reactions-api-openapi.yml
- filename: devto-segments-api-openapi.yml
  format: yaml
  label: DEV Community Segments API
  slug: devto-segments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dev-to/refs/heads/main/openapi/devto-segments-api-openapi.yml
- filename: devto-surveys-api-openapi.yml
  format: yaml
  label: DEV Community Surveys API
  slug: devto-surveys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dev-to/refs/heads/main/openapi/devto-surveys-api-openapi.yml
- filename: devto-tags-api-openapi.yml
  format: yaml
  label: DEV Community Tags API
  slug: devto-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dev-to/refs/heads/main/openapi/devto-tags-api-openapi.yml
- filename: devto-trends-api-openapi.yml
  format: yaml
  label: DEV Community Trends API
  slug: devto-trends-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dev-to/refs/heads/main/openapi/devto-trends-api-openapi.yml
- filename: devto-users-api-openapi.yml
  format: yaml
  label: DEV Community Users API
  slug: devto-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dev-to/refs/heads/main/openapi/devto-users-api-openapi.yml
- filename: devto-videos-api-openapi.yml
  format: yaml
  label: DEV Community Videos API
  slug: devto-videos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dev-to/refs/heads/main/openapi/devto-videos-api-openapi.yml
- filename: devto-reading-list-api-openapi.yml
  format: yaml
  label: DEV Community Reading List API
  slug: devto-reading-list-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dev-to/refs/heads/main/openapi/devto-reading-list-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Dev To Authentication
name_suffix: Authentication
oauth_flows: []
overview: DEV Community secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: DEV Community
provider_slug: dev-to
scheme_count: 2
schemes:
- description: Per-user API key. Authentication for write operations (Articles, Reactions, Follows, Webhooks) requires a DEV API key; many read endpoints are accessible publicly without one. All authenticated endpoints are CORS-disabled — the key is intended for non-browser scripts.
  in: header
  name: api-key
  obtain: https://dev.to/settings/extensions
  parameter: api-key
  sources:
  - https://dev.to/openapi.json
  type: apiKey
- bearer_format: JWT
  description: Short-lived RS256 RFC 9068 access token issued by the configured delegation service and verified against its configured JWKS. The issuer authorizes the client and requested operation before minting the token; Forem validates it and resolves its subject and owner to a local user. An invalid token returns 401; an unavailable trust dependency with no usable cached key returns 503. Available only on instances that enable delegated access.
  name: bearer_auth
  scheme: bearer
  sources:
  - https://dev.to/openapi.json
  type: http
slug: dev-to-authentication
source_filename: dev-to-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-17'\nmethod: searched\nsource: https://dev.to/openapi.json (components.securitySchemes) + https://developers.forem.com/api\ndocs: https://developers.forem.com/api\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\n  notes: >-\n    Forem API V1 accepts two credentials. The universal one is the per-user `api-key` header,\n    generated by the account holder at https://dev.to/settings/extensions. Instances that enable\n    delegated access additionally accept an RFC 9068 `Authorization: Bearer` JWT minted by the\n    instance's configured delegation service and verified against its JWKS. Every V1 request must\n    also carry `Accept: application/vnd.forem.api-v1+json` — the Accept header is the version\n    selector, not a path segment, and omitting it silently routes the call to the deprecated V0 API.\nschemes:\n- name: api-key\n  type: apiKey\n  in: header\n  parameter: api-key\n  description: >-\n    Per-user API key. Authentication for\
  \ write operations (Articles, Reactions, Follows, Webhooks)\n    requires a DEV API key; many read endpoints are accessible publicly without one. All\n    authenticated endpoints are CORS-disabled — the key is intended for non-browser scripts.\n  obtain: https://dev.to/settings/extensions\n  sources:\n  - https://dev.to/openapi.json\n- name: bearer_auth\n  type: http\n  scheme: bearer\n  bearer_format: JWT\n  description: >-\n    Short-lived RS256 RFC 9068 access token issued by the configured delegation service and verified\n    against its configured JWKS. The issuer authorizes the client and requested operation before\n    minting the token; Forem validates it and resolves its subject and owner to a local user. An\n    invalid token returns 401; an unavailable trust dependency with no usable cached key returns 503.\n    Available only on instances that enable delegated access.\n  sources:\n  - https://dev.to/openapi.json\nrequired_headers:\n- name: Accept\n  value: application/vnd.forem.api-v1+json\n\
  \  reason: >-\n    Selects API version 1. Omitting it routes to the deprecated V0 API (the server replies with a\n    299 Warning header pointing at the V1 Accept header).\noauth2: false\nscopes_published: false\nnotes: >-\n  No OAuth 2.0 authorization-code flow is published for the API surface, so no scopes/ artifact is\n  emitted. Social sign-in (GitHub, Twitter) exists for the web application only, not for API clients.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dev-to/refs/heads/main/authentication/dev-to-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Developer Community
- Content
- Publishing
- Social
- Blogging
- Open Source
- Articles
- Webhook
---
