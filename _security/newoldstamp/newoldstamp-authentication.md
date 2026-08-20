---
api_key_in: []
auth_types:
- http
description: ''
kind: authentication
layout: security
method: probed
name: Newoldstamp Authentication
name_suffix: Authentication
oauth_flows: []
overview: Newoldstamp secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Newoldstamp
provider_slug: newoldstamp
scheme_count: 1
schemes:
- bearer_format: opaque-access-token
  description: Access token issued by the signIn mutation (email + password, or oauth via OauthInput) as a UserAccessToken, and rotated by the refreshToken mutation. Sent as a bearer credential on GraphQL requests.
  name: bearerAuth
  scheme: bearer
  sources:
  - graphql/newoldstamp.graphql
  type: http
slug: newoldstamp-authentication
source_filename: newoldstamp-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: probed\nsource: https://newoldstamp.com/api/graphql\nnote: >-\n  Newoldstamp has no OpenAPI securitySchemes to derive from; the auth model is\n  read from the live GraphQL schema (signIn / refreshToken mutations returning\n  UserAccessToken) and observed request headers. This is the application\n  backend, not a documented public developer API — there is no published API-key\n  program.\nsummary:\n  types:\n  - http\n  http_scheme: bearer\n  token_issuance: password + OAuth (Google) login via signIn mutation\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearer_format: opaque-access-token\n  description: >-\n    Access token issued by the signIn mutation (email + password, or oauth via\n    OauthInput) as a UserAccessToken, and rotated by the refreshToken mutation.\n    Sent as a bearer credential on GraphQL requests.\n  sources:\n  - graphql/newoldstamp.graphql\noauth_login:\n  provider: google\n  input_type: OauthInput\n\
  \  note: >-\n    Google OAuth is offered as an end-user sign-in method (signIn/signUp accept\n    an oauth: OauthInput), plus a recaptcha token (newGoogleRecaptchaToken). This\n    is consumer login, not a delegated third-party OAuth authorization surface —\n    there are no OAuth scopes and no /.well-known/oauth-authorization-server.\nmutations:\n- signIn(email, password, oauth, newGoogleRecaptchaToken) -> UserAccessToken\n- refreshToken(refreshToken) -> UserAccessToken\n- invitePasswordUpdate(invitationToken, password) -> UserAccessToken\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/newoldstamp/refs/heads/main/authentication/newoldstamp-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Email Signatures
- Email Signature Management
- Email Marketing
- Branding
- Software-as-a-Service
- Productivity
- Website Visitor Identification
- GraphQL
---
