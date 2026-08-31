---
api_key_in: []
api_specs:
- filename: instagram-comments-api-openapi.yml
  format: yaml
  label: Instagram Comments API
  slug: instagram-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/instagram/refs/heads/main/openapi/instagram-comments-api-openapi.yml
- filename: instagram-hashtags-api-openapi.yml
  format: yaml
  label: Instagram Hashtags API
  slug: instagram-hashtags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/instagram/refs/heads/main/openapi/instagram-hashtags-api-openapi.yml
- filename: instagram-insights-api-openapi.yml
  format: yaml
  label: Instagram Insights API
  slug: instagram-insights-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/instagram/refs/heads/main/openapi/instagram-insights-api-openapi.yml
- filename: instagram-media-api-openapi.yml
  format: yaml
  label: Instagram Media API
  slug: instagram-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/instagram/refs/heads/main/openapi/instagram-media-api-openapi.yml
- filename: instagram-mentions-api-openapi.yml
  format: yaml
  label: Instagram Mentions API
  slug: instagram-mentions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/instagram/refs/heads/main/openapi/instagram-mentions-api-openapi.yml
- filename: instagram-publishing-api-openapi.yml
  format: yaml
  label: Instagram Publishing API
  slug: instagram-publishing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/instagram/refs/heads/main/openapi/instagram-publishing-api-openapi.yml
- filename: instagram-users-api-openapi.yml
  format: yaml
  label: Instagram Users API
  slug: instagram-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/instagram/refs/heads/main/openapi/instagram-users-api-openapi.yml
auth_types:
- oauth2
description: The Instagram Platform is OAuth 2.0 authorization code only. There is no API key, no basic auth, no mTLS and no service account. Which of the two login models you pick determines the host, the permission family, the token endpoints and which capabilities you can reach - they are not interchangeable. Upgraded 2026-08-29 from a derivation off the OpenAPI securitySchemes to the published Business Login reference, which supplied the Instagram Login endpoints and the token lifetimes the specs do not carry.
kind: authentication
layout: security
method: searched
name: Instagram Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Instagram secures its APIs with oauth2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Instagram
provider_slug: instagram
scheme_count: 2
schemes:
- base: https://graph.instagram.com
  deprecated_scope_values:
    deprecated_on: '2025-01-27'
    replaced:
    - business_basic
    - business_content_publish
    - business_manage_comments
    - business_manage_messages
  description: Native Instagram authentication. The professional account authorizes directly; no Facebook Page is involved. Cannot reach hashtag search or business discovery.
  flows:
  - authorizationUrl: https://www.instagram.com/oauth/authorize
    flow: authorizationCode
    longLivedTokenUrl: https://graph.instagram.com/access_token
    refreshUrl: https://graph.instagram.com/refresh_access_token
    scopes: 4
    tokenUrl: https://api.instagram.com/oauth/access_token
  login_model: Instagram API with Instagram Login
  name: oauth2-instagram-login
  scope_family: instagram_business_*
  scopes:
  - instagram_business_basic
  - instagram_business_content_publish
  - instagram_business_manage_comments
  - instagram_business_manage_messages
  type: oauth2
- base: https://graph.facebook.com
  description: Facebook Page-linked authentication. The Instagram professional account must be connected to a Facebook Page and the user must hold a task role on that Page. Required for IG Hashtag Search and Business Discovery.
  flows:
  - authorizationUrl: https://www.facebook.com/dialog/oauth
    flow: authorizationCode
    scopes: 15
    tokenUrl: https://graph.facebook.com/oauth/access_token
  login_model: Instagram API with Facebook Login
  name: oauth2-facebook-login
  openid_connect:
    caveat: The document omits token_endpoint and userinfo_endpoint, so it is not a complete OIDC discovery document. Instagram Login publishes no discovery document at all and issues no id_token.
    discovery_document: https://www.facebook.com/.well-known/openid-configuration
    id_token_signing_alg: RS256
    issuer: https://www.facebook.com
    jwks_uri: https://www.facebook.com/.well-known/oauth/openid/jwks/
    response_types:
    - id_token
    - token id_token
    saved: well-known/instagram-facebook-openid-configuration.json
    status: 200
    subject_types: pairwise
  scope_family: instagram_*
  type: oauth2
slug: instagram-authentication
source_filename: instagram-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-29'\nmethod: searched\nsource:\n- https://developers.facebook.com/docs/instagram-platform/instagram-api-with-instagram-login/business-login\n- https://developers.facebook.com/docs/permissions\n- https://www.facebook.com/.well-known/openid-configuration\n- openapi/\ndocs: https://developers.facebook.com/docs/instagram-platform/instagram-api-with-instagram-login/business-login\ndescription: >-\n  The Instagram Platform is OAuth 2.0 authorization code only. There is no API key, no basic auth,\n  no mTLS and no service account. Which of the two login models you pick determines the host, the\n  permission family, the token endpoints and which capabilities you can reach - they are not\n  interchangeable. Upgraded 2026-08-29 from a derivation off the OpenAPI securitySchemes to the\n  published Business Login reference, which supplied the Instagram Login endpoints and the token\n  lifetimes the specs do not carry.\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n\
  \  - authorizationCode\n  api_key: false\n  basic_auth: false\n  mutual_tls: false\n  openid_connect: partial\nschemes:\n- name: oauth2-instagram-login\n  type: oauth2\n  login_model: Instagram API with Instagram Login\n  base: https://graph.instagram.com\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://www.instagram.com/oauth/authorize\n    tokenUrl: https://api.instagram.com/oauth/access_token\n    longLivedTokenUrl: https://graph.instagram.com/access_token\n    refreshUrl: https://graph.instagram.com/refresh_access_token\n    scopes: 4\n  scope_family: instagram_business_*\n  scopes:\n  - instagram_business_basic\n  - instagram_business_content_publish\n  - instagram_business_manage_comments\n  - instagram_business_manage_messages\n  deprecated_scope_values:\n    deprecated_on: '2025-01-27'\n    replaced:\n    - business_basic\n    - business_content_publish\n    - business_manage_comments\n    - business_manage_messages\n  description: >-\n    Native Instagram\
  \ authentication. The professional account authorizes directly; no Facebook Page\n    is involved. Cannot reach hashtag search or business discovery.\n- name: oauth2-facebook-login\n  type: oauth2\n  login_model: Instagram API with Facebook Login\n  base: https://graph.facebook.com\n  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://www.facebook.com/dialog/oauth\n    tokenUrl: https://graph.facebook.com/oauth/access_token\n    scopes: 15\n  scope_family: instagram_*\n  description: >-\n    Facebook Page-linked authentication. The Instagram professional account must be connected to a\n    Facebook Page and the user must hold a task role on that Page. Required for IG Hashtag Search\n    and Business Discovery.\n  openid_connect:\n    discovery_document: https://www.facebook.com/.well-known/openid-configuration\n    status: 200\n    saved: well-known/instagram-facebook-openid-configuration.json\n    issuer: https://www.facebook.com\n    jwks_uri: https://www.facebook.com/.well-known/oauth/openid/jwks/\n\
  \    id_token_signing_alg: RS256\n    subject_types: pairwise\n    response_types: [id_token, 'token id_token']\n    caveat: >-\n      The document omits token_endpoint and userinfo_endpoint, so it is not a complete OIDC\n      discovery document. Instagram Login publishes no discovery document at all and issues no\n      id_token.\ntokens:\n  authorization_code:\n    lifetime: 1 hour\n    single_use: true\n  short_lived_access_token:\n    lifetime: 1 hour\n    note: Exchange for a long-lived token immediately on receipt.\n  long_lived_access_token:\n    lifetime: 60 days\n    refreshable: true\n    refresh_endpoint: https://graph.instagram.com/refresh_access_token\n    note: >-\n      Refresh extends by another 60 days when conditions are met. An integration that goes quiet for\n      60 days loses the token permanently and has to re-authorize the user - the single most common\n      cause of a silently dead Instagram integration.\n  transport:\n  - preferred: 'Authorization: Bearer {access-token}'\n\
  \  - accepted: '?access_token={access-token}'\n  transport_note: >-\n    Meta accepts the token as a query parameter. That form leaks the credential into access logs,\n    proxy logs and Referer headers - use the header.\n  revocation:\n    user_initiated: >-\n      A user can remove the app from Instagram Settings > Apps and Websites, which invalidates the\n      token immediately (surfaced as error 190 subcode 458).\n    password_change: A credential change invalidates the token (error 190 subcode 460).\nauthorization_model:\n  gate: App Review plus Business Verification, not payment\n  standard_access: permissions usable only against users holding a role on the app\n  advanced_access: permissions usable against any user, after per-permission App Review\n  detail: scopes/instagram-scopes.yml\nerrors:\n  190: Access token expired, revoked or otherwise invalid. Read error_subcode for the cause.\n  102: Login status or access token has expired or been revoked.\n  10: Permission not granted\
  \ or removed.\n  200-299: Permission family errors.\n  detail: errors/instagram-problem-types.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/instagram/refs/heads/main/authentication/instagram-authentication.yml
summary_line: oauth2 · 2 schemes
tags:
- Instagram
- Meta
- Photos
- Social-Media
- Videos
- Content Publishing
---
