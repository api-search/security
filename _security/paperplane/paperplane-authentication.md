---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: Paperplane Authentication
name_suffix: Authentication
oauth_flows: []
overview: Paperplane declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Paperplane
provider_slug: paperplane
scheme_count: 1
schemes:
- claims:
  - sub
  - iss
  - aud
  - exp
  - iat
  - name
  - given_name
  - family_name
  - preferred_username
  - picture
  - email
  - email_verified
  - org_id
  endpoints:
    authorization: https://clerk.paperplane.ai/oauth/authorize
    introspection: https://clerk.paperplane.ai/oauth/token_info
    jwks: https://clerk.paperplane.ai/.well-known/jwks.json
    revocation: https://clerk.paperplane.ai/oauth/token/revoke
    token: https://clerk.paperplane.ai/oauth/token
    userinfo: https://clerk.paperplane.ai/oauth/userinfo
  flows:
  - authorization_code
  - refresh_token
  id: paperplane-clerk-oidc
  id_token_signing_alg:
  - RS256
  issuer: https://clerk.paperplane.ai
  logout:
    backchannel_supported: false
    frontchannel_supported: false
  name: Clerk-hosted OpenID Connect
  oauth_metadata_url: https://clerk.paperplane.ai/.well-known/oauth-authorization-server
  openid_connect_url: https://clerk.paperplane.ai/.well-known/openid-configuration
  pkce:
    code_challenge_methods:
    - S256
    required: unknown
  response_modes:
  - form_post
  - query
  response_types:
  - code
  scopes_ref: scopes/paperplane-scopes.yml
  subject_types:
  - public
  token_endpoint_auth_methods:
  - client_secret_basic
  - client_secret_post
  - none
  type: openIdConnect
slug: paperplane-authentication
source_filename: paperplane-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: https://clerk.paperplane.ai/.well-known/openid-configuration\nscope_note: >-\n  Paperplane publishes no public developer API and no OpenAPI, so there is no\n  spec securitySchemes block to derive from. This profile is read verbatim from\n  the live OIDC discovery document and the RFC 8414 OAuth 2.0 Authorization\n  Server Metadata document served at clerk.paperplane.ai — Paperplane's own\n  Clerk-hosted identity instance (issuer https://clerk.paperplane.ai, instance\n  ins_2eXpXIGIP45PViegvGGdEfVfHcf, CNAME frontend-api.clerk.services). This\n  documents how identities authenticate to the Paperplane application, NOT how\n  a third-party developer would authenticate against a public Paperplane API,\n  because no such API is published. Note also that the application this\n  identity server fronts is currently offline (app.paperplane.ai returns\n  Vercel 402 DEPLOYMENT_DISABLED) — see lifecycle/paperplane-lifecycle.yml.\nschemes:\n\
  - id: paperplane-clerk-oidc\n  type: openIdConnect\n  name: Clerk-hosted OpenID Connect\n  issuer: https://clerk.paperplane.ai\n  openid_connect_url: https://clerk.paperplane.ai/.well-known/openid-configuration\n  oauth_metadata_url: https://clerk.paperplane.ai/.well-known/oauth-authorization-server\n  endpoints:\n    authorization: https://clerk.paperplane.ai/oauth/authorize\n    token: https://clerk.paperplane.ai/oauth/token\n    revocation: https://clerk.paperplane.ai/oauth/token/revoke\n    introspection: https://clerk.paperplane.ai/oauth/token_info\n    userinfo: https://clerk.paperplane.ai/oauth/userinfo\n    jwks: https://clerk.paperplane.ai/.well-known/jwks.json\n  flows:\n  - authorization_code\n  - refresh_token\n  pkce:\n    required: unknown\n    code_challenge_methods:\n    - S256\n  response_types:\n  - code\n  response_modes:\n  - form_post\n  - query\n  token_endpoint_auth_methods:\n  - client_secret_basic\n  - client_secret_post\n  - none\n  id_token_signing_alg:\n  -\
  \ RS256\n  subject_types:\n  - public\n  claims:\n  - sub\n  - iss\n  - aud\n  - exp\n  - iat\n  - name\n  - given_name\n  - family_name\n  - preferred_username\n  - picture\n  - email\n  - email_verified\n  - org_id\n  scopes_ref: scopes/paperplane-scopes.yml\n  logout:\n    backchannel_supported: false\n    frontchannel_supported: false\napi_key_auth: none-published\nmutual_tls: none-published\ndocs: null\ndocs_note: >-\n  Paperplane publishes no authentication documentation of its own. The GitBook\n  documentation site at docs.paperplane.ai is an unfilled GitBook starter\n  template (lorem ipsum bodies, \"Awesome Feature One\", last updated three years\n  ago) and contains no auth page. The only prose reference the discovery\n  document itself carries is Clerk's generic\n  https://clerk.com/docs/oauth/scoped-access, which is the vendor's\n  documentation, not Paperplane's.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/paperplane/refs/heads/main/authentication/paperplane-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Sales
- CRM
- Salesforce
- Sales Automation
- Conversation Intelligence
- Note Taking
- Artificial Intelligence
- Productivity
---
