---
api_key_in:
- header
auth_types:
- http-bearer
- jwt-sso
description: ''
kind: authentication
layout: security
method: searched
name: Vox Media Authentication
name_suffix: Authentication
oauth_flows: []
overview: Vox Media secures its APIs with http-bearer and jwt-sso across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Vox Media
provider_slug: vox-media
scheme_count: 2
schemes:
- description: 'Direct API integration with the Coral GraphQL API (/api/graphql) is limited to administrative users. Access tokens are created with coral-cli (coral-cli token:create --domain <domain> --name <name> --json) and passed as Authorization: Bearer <signedToken>. Tokens are listed and revoked via coral-cli token:list / token:revoke. Only admin users can make arbitrary queries; other callers get RAW_QUERY_NOT_AUTHORIZED (persisted queries only).'
  docs: https://docs.coralproject.net/api/schema
  name: AdminAccessToken
  scheme: bearer
  type: http
- bearerFormat: JWT
  description: 'End-user (commenter) authentication integrates a publisher''s own identity system via SSO JWTs signed with HS256 using the signing secret from the Coral admin panel. Required claims: user.id, user.email, user.username. Optional claims: jti, exp, iat, user.badges, user.role (COMMENTER, STAFF, MODERATOR, ADMIN), user.url. Tokens are passed to the embed via createStreamEmbed(), embed.login(), and cleared with embed.logout(). Authentication strategies cannot be shared per user (SSO vs email login are exclusive).'
  docs: https://docs.coralproject.net/sso
  name: SSOUserToken
  scheme: bearer
  type: http
slug: vox-media-authentication
source_filename: vox-media-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: searched\nsource: https://docs.coralproject.net/api/schema\ndocs: https://docs.coralproject.net/sso\nsummary:\n  types: [http-bearer, jwt-sso]\n  api_key_in: [header]\n  oauth2_flows: []\nschemes:\n- name: AdminAccessToken\n  type: http\n  scheme: bearer\n  description: >-\n    Direct API integration with the Coral GraphQL API (/api/graphql) is\n    limited to administrative users. Access tokens are created with coral-cli\n    (coral-cli token:create --domain <domain> --name <name> --json) and passed\n    as Authorization: Bearer <signedToken>. Tokens are listed and revoked via\n    coral-cli token:list / token:revoke. Only admin users can make arbitrary\n    queries; other callers get RAW_QUERY_NOT_AUTHORIZED (persisted queries\n    only).\n  docs: https://docs.coralproject.net/api/schema\n- name: SSOUserToken\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: >-\n    End-user (commenter) authentication integrates a publisher's\
  \ own identity\n    system via SSO JWTs signed with HS256 using the signing secret from the\n    Coral admin panel. Required claims: user.id, user.email, user.username.\n    Optional claims: jti, exp, iat, user.badges, user.role (COMMENTER, STAFF,\n    MODERATOR, ADMIN), user.url. Tokens are passed to the embed via\n    createStreamEmbed(), embed.login(), and cleared with embed.logout().\n    Authentication strategies cannot be shared per user (SSO vs email login\n    are exclusive).\n  docs: https://docs.coralproject.net/sso\nnotes: >-\n  No OAuth 2.0 or OpenID Connect surface is published. The GraphQL schema also\n  carries an @auth(roles:[...]) directive gating fields by role (ADMIN,\n  MODERATOR, etc.).\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vox-media/refs/heads/main/authentication/vox-media-authentication.yml
summary_line: http-bearer/jwt-sso · 2 schemes
tags:
- Company
- Consumer
- Media
- Publishing
- News
- Comments
- Community
- Moderation
- GraphQL
---
