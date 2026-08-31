---
api_key_in: []
api_specs:
- filename: yoast-pages-api-openapi.yml
  format: yaml
  label: Yoast Pages API
  slug: yoast-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yoast/refs/heads/main/openapi/yoast-pages-api-openapi.yml
- filename: yoast-posts-api-openapi.yml
  format: yaml
  label: Yoast Posts API
  slug: yoast-posts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yoast/refs/heads/main/openapi/yoast-posts-api-openapi.yml
- filename: yoast-seo-head-api-openapi.yml
  format: yaml
  label: Yoast SEO Head API
  slug: yoast-seo-head-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yoast/refs/heads/main/openapi/yoast-seo-head-api-openapi.yml
- filename: yoast-abilities-api-openapi.yml
  format: yaml
  label: Yoast SEO Abilities API
  slug: yoast-abilities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yoast/refs/heads/main/openapi/yoast-abilities-api-openapi.yml
- filename: yoast-provisioning-account-api-openapi.yml
  format: yaml
  label: Yoast Provisioning Account API
  slug: yoast-provisioning-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yoast/refs/heads/main/openapi/yoast-provisioning-account-api-openapi.yml
- filename: yoast-provisioning-downloads-api-openapi.yml
  format: yaml
  label: Yoast Provisioning Downloads API
  slug: yoast-provisioning-downloads-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yoast/refs/heads/main/openapi/yoast-provisioning-downloads-api-openapi.yml
- filename: yoast-provisioning-users-api-openapi.yml
  format: yaml
  label: Yoast Provisioning Users API
  slug: yoast-provisioning-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yoast/refs/heads/main/openapi/yoast-provisioning-users-api-openapi.yml
- filename: yoast-schema-aggregator-api-openapi.yml
  format: yaml
  label: Yoast Schema Aggregator API
  slug: yoast-schema-aggregator-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yoast/refs/heads/main/openapi/yoast-schema-aggregator-api-openapi.yml
- filename: yoast-subscription-provisioning-api-openapi.yml
  format: yaml
  label: Yoast Subscription Provisioning API
  slug: yoast-subscription-provisioning-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yoast/refs/heads/main/openapi/yoast-subscription-provisioning-api-openapi.yml
auth_types:
- http
- openIdConnect
- none
description: ''
kind: authentication
layout: security
method: searched
name: Yoast Authentication
name_suffix: Authentication
oauth_flows: []
overview: Yoast secures its APIs with http, openIdConnect, and none across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Yoast
provider_slug: yoast
scheme_count: 3
schemes:
- api: MyYoast Provisioning API
  description: HTTP Basic authentication with provisioner credentials issued by Yoast to approved provisioning partners. The password can be rotated with POST /api/provisioning/account/regenerate-token, which immediately invalidates the previous password.
  name: basic
  rotation:
    note: rotation invalidates the old password immediately; the response is shown once
    operation: provisioningAccountControllerRegenerateToken
    supported: true
  scheme: basic
  sources:
  - openapi/yoast-myyoast-provisioning-openapi.yml
  type: http
- api: MyYoast (site + user authentication for Yoast SEO)
  description: MyYoast operates a full OpenID Connect provider. Yoast SEO enrols the customer's WordPress site as an OAuth client using RFC 7591 Dynamic Client Registration and then authenticates either the site (client_credentials) or a specific user (authorization code + PKCE), driven from WP-CLI via `wp yoast auth`.
  dynamic_client_registration:
    endpoint: https://my.yoast.com/api/oauth/reg
    spec: RFC 7591
    supported: true
  endpoints:
    authorization: https://my.yoast.com/api/oauth/auth
    end_session: https://my.yoast.com/api/oauth/session/end
    introspection: https://my.yoast.com/api/oauth/token/introspection
    jwks: https://my.yoast.com/api/oauth/jwks
    registration: https://my.yoast.com/api/oauth/reg
    revocation: https://my.yoast.com/api/oauth/token/revocation
    token: https://my.yoast.com/api/oauth/token
    userinfo: https://my.yoast.com/api/oauth/me
  grant_types:
  - authorization_code
  - refresh_token
  - client_credentials
  id_token_signing_algs:
  - EdDSA
  issuer: https://my.yoast.com
  key_rotation:
    note: '`wp yoast auth rotate-keys` rotates the registration or DPoP proof key pairs'
    supported: true
  name: myyoast-oidc
  openIdConnectUrl: https://my.yoast.com/.well-known/openid-configuration
  pkce:
    required_methods:
    - S256
  response_types:
  - code
  sender_constrained_tokens:
    dpop: true
    dpop_signing_algs:
    - ES256
    - EdDSA
  sources:
  - well-known/yoast-openid-configuration.json
  token_endpoint_auth_methods:
  - none
  - private_key_jwt
  token_endpoint_auth_signing_algs:
  - ES256
  - EdDSA
  - RS256
  type: openIdConnect
- api: Yoast REST API, Schema Aggregator API, Yoast SEO Abilities API
  description: No Yoast-issued credential exists for these. They are WordPress REST routes served by the customer's own install. The documented read paths (yoast/v1/get_head, yoast_head_json on wp/v2/posts and wp/v2/pages, the schema-aggregator routes) are reachable unauthenticated for public content; the WordPress Abilities API applies its own per-ability permission checks, whose required capability Yoast does not publish. Where authentication is needed it is WordPress's — cookie + nonce for first-party requests, Application Passwords or a JWT/OAuth plugin for machine clients.
  name: wordpress-host
  sources:
  - https://developer.yoast.com/customization/apis/rest-api/
  - https://developer.yoast.com/features/yoast-seo-abilities/overview/
  type: none
slug: yoast-authentication
source_filename: yoast-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: openapi/yoast-myyoast-provisioning-openapi.yml\ndocs:\n  - https://developer.yoast.com/customization/apis/rest-api/\n  - https://developer.yoast.com/features/wp-cli/auth/\n  - https://my.yoast.com/.well-known/openid-configuration\nnote: >-\n  Yoast has three distinct authentication stories, and conflating them is the usual\n  mistake. (1) The Yoast REST API, Schema Aggregator and Abilities endpoints run on the\n  CUSTOMER's WordPress install, so authentication is WordPress's, not Yoast's — the\n  get_head and yoast_head_json read paths are public on a public post, and anything\n  requiring a logged-in user rides WordPress cookies/nonces or Application Passwords.\n  Yoast documents no auth for the read-only REST surface because there is none to\n  document. (2) The MyYoast Provisioning API on my.yoast.com is HTTP Basic with\n  partner-issued credentials, self-rotatable via POST /api/provisioning/account/\n  regenerate-token.\
  \ (3) my.yoast.com is ALSO a full OpenID Connect provider — probed live\n  at /.well-known/openid-configuration — which is what Yoast SEO's `wp yoast auth`\n  WP-CLI commands use to enrol a site as an OAuth client via RFC 7591 dynamic client\n  registration and then obtain tokens. That third surface is the modern one and is\n  markedly stronger than the Basic Auth on the provisioning API it sits next to.\nsummary:\n  types:\n    - http\n    - openIdConnect\n    - none\n  strongest: openIdConnect\nschemes:\n  - name: basic\n    type: http\n    scheme: basic\n    api: MyYoast Provisioning API\n    description: >-\n      HTTP Basic authentication with provisioner credentials issued by Yoast to approved\n      provisioning partners. The password can be rotated with\n      POST /api/provisioning/account/regenerate-token, which immediately invalidates the\n      previous password.\n    sources:\n      - openapi/yoast-myyoast-provisioning-openapi.yml\n    rotation:\n      supported: true\n  \
  \    operation: provisioningAccountControllerRegenerateToken\n      note: rotation invalidates the old password immediately; the response is shown once\n  - name: myyoast-oidc\n    type: openIdConnect\n    api: MyYoast (site + user authentication for Yoast SEO)\n    issuer: https://my.yoast.com\n    openIdConnectUrl: https://my.yoast.com/.well-known/openid-configuration\n    description: >-\n      MyYoast operates a full OpenID Connect provider. Yoast SEO enrols the customer's\n      WordPress site as an OAuth client using RFC 7591 Dynamic Client Registration and\n      then authenticates either the site (client_credentials) or a specific user\n      (authorization code + PKCE), driven from WP-CLI via `wp yoast auth`.\n    endpoints:\n      authorization: https://my.yoast.com/api/oauth/auth\n      token: https://my.yoast.com/api/oauth/token\n      userinfo: https://my.yoast.com/api/oauth/me\n      jwks: https://my.yoast.com/api/oauth/jwks\n      registration: https://my.yoast.com/api/oauth/reg\n\
  \      introspection: https://my.yoast.com/api/oauth/token/introspection\n      revocation: https://my.yoast.com/api/oauth/token/revocation\n      end_session: https://my.yoast.com/api/oauth/session/end\n    grant_types:\n      - authorization_code\n      - refresh_token\n      - client_credentials\n    response_types:\n      - code\n    pkce:\n      required_methods:\n        - S256\n    token_endpoint_auth_methods:\n      - none\n      - private_key_jwt\n    token_endpoint_auth_signing_algs:\n      - ES256\n      - EdDSA\n      - RS256\n    id_token_signing_algs:\n      - EdDSA\n    sender_constrained_tokens:\n      dpop: true\n      dpop_signing_algs:\n        - ES256\n        - EdDSA\n    dynamic_client_registration:\n      supported: true\n      spec: RFC 7591\n      endpoint: https://my.yoast.com/api/oauth/reg\n    key_rotation:\n      supported: true\n      note: '`wp yoast auth rotate-keys` rotates the registration or DPoP proof key pairs'\n    sources:\n      - well-known/yoast-openid-configuration.json\n\
  \  - name: wordpress-host\n    type: none\n    api: Yoast REST API, Schema Aggregator API, Yoast SEO Abilities API\n    description: >-\n      No Yoast-issued credential exists for these. They are WordPress REST routes served\n      by the customer's own install. The documented read paths (yoast/v1/get_head,\n      yoast_head_json on wp/v2/posts and wp/v2/pages, the schema-aggregator routes) are\n      reachable unauthenticated for public content; the WordPress Abilities API applies\n      its own per-ability permission checks, whose required capability Yoast does not\n      publish. Where authentication is needed it is WordPress's — cookie + nonce for\n      first-party requests, Application Passwords or a JWT/OAuth plugin for machine\n      clients.\n    sources:\n      - https://developer.yoast.com/customization/apis/rest-api/\n      - https://developer.yoast.com/features/yoast-seo-abilities/overview/\ngaps:\n  - >-\n    Yoast does not publish which WordPress capability each Abilities\
  \ API ability\n    requires, so an integrator cannot tell in advance which role can read SEO scores.\n  - >-\n    The MyYoast Provisioning API remains HTTP Basic while the same host runs a modern\n    OIDC provider with DPoP; there is no documented path for a provisioner to move onto\n    OAuth.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/yoast/refs/heads/main/authentication/yoast-authentication.yml
summary_line: http/openIdConnect/none · 3 schemes
tags:
- SEO
- WordPress
- Content Optimization
- Schema
- Metadata
- Structured Data
- Headless CMS
- Content Analysis
- Agent Readiness
- Plugins
---
