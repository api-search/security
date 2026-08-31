---
api_key_in: []
api_specs:
- filename: yieldmo-canned-reports-api-openapi.yml
  format: yaml
  label: Yieldmo Canned Reports API
  slug: yieldmo-canned-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yieldmo/refs/heads/main/openapi/yieldmo-canned-reports-api-openapi.yml
- filename: yieldmo-dcs-api-openapi.yml
  format: yaml
  label: Yieldmo Dcs API
  slug: yieldmo-dcs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yieldmo/refs/heads/main/openapi/yieldmo-dcs-api-openapi.yml
- filename: yieldmo-manage-api-openapi.yml
  format: yaml
  label: Yieldmo Manage API
  slug: yieldmo-manage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yieldmo/refs/heads/main/openapi/yieldmo-manage-api-openapi.yml
- filename: yieldmo-mcp-api-openapi.yml
  format: yaml
  label: Yieldmo MCP API
  slug: yieldmo-mcp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yieldmo/refs/heads/main/openapi/yieldmo-mcp-api-openapi.yml
- filename: yieldmo-ping-api-openapi.yml
  format: yaml
  label: Yieldmo Ping API
  slug: yieldmo-ping-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yieldmo/refs/heads/main/openapi/yieldmo-ping-api-openapi.yml
- filename: yieldmo-register-api-openapi.yml
  format: yaml
  label: Yieldmo Register API
  slug: yieldmo-register-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yieldmo/refs/heads/main/openapi/yieldmo-register-api-openapi.yml
- filename: yieldmo-well-known-api-openapi.yml
  format: yaml
  label: Yieldmo .well Known API
  slug: yieldmo-well-known-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yieldmo/refs/heads/main/openapi/yieldmo-well-known-api-openapi.yml
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: probed
name: Yieldmo Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- implicit
overview: Yieldmo secures its APIs with oauth2 and openIdConnect across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and implicit flow(s).
provider_name: Yieldmo
provider_slug: yieldmo
scheme_count: 2
schemes:
- dynamic_client_registration:
    note: The OpenAPI labels this handler "Fake Registration Mcp" (operationId fake_registration_mcp_register_post), which suggests it satisfies MCP client-registration expectations without provisioning a distinct Cognito app client. Behaviour unverified — the endpoint returns 404 when called on the bare host path.
    registration_endpoint: https://api.yieldmo.com/dcs/mcp/register
    spec: RFC 7591
    supported: true
  end_session_endpoint: https://yieldmo-cuba.auth.us-east-1.amazoncognito.com/logout
  flows:
  - authorizationUrl: https://yieldmo-cuba.auth.us-east-1.amazoncognito.com/oauth2/authorize
    flow: authorizationCode
    refreshUrl: https://yieldmo-cuba.auth.us-east-1.amazoncognito.com/oauth2/token
    scopes:
      email: Email address claim
      openid: OpenID Connect subject identifier
      profile: Basic profile claims
    tokenUrl: https://yieldmo-cuba.auth.us-east-1.amazoncognito.com/oauth2/token
  - authorizationUrl: https://yieldmo-cuba.auth.us-east-1.amazoncognito.com/oauth2/authorize
    flow: implicit
    note: response_types_supported includes "token", so the implicit flow is advertised.
  id_token_signing_alg:
  - RS256
  issuer: https://api.yieldmo.com/dcs/mcp
  jwks_uri: https://cognito-idp.us-east-1.amazonaws.com/us-east-1_vZfEMm5aZ/.well-known/jwks.json
  name: mcp-oauth2
  protected_resource: https://api.yieldmo.com/dcs/mcp
  revocation_endpoint: https://yieldmo-cuba.auth.us-east-1.amazoncognito.com/oauth2/revoke
  sources:
  - well-known/yieldmo-oauth-authorization-server.json
  - well-known/yieldmo-openid-configuration.json
  - well-known/yieldmo-oauth-protected-resource.json
  subject_types:
  - public
  token_endpoint_auth_methods:
  - none
  - client_secret_basic
  - client_secret_post
  type: oauth2
  userinfo_endpoint: https://yieldmo-cuba.auth.us-east-1.amazoncognito.com/oauth2/userInfo
- name: mcp-openid-connect
  note: The OIDC discovery document is served at the RFC 8414 path on the API host and is byte-identical to the oauth-authorization-server document. It is not a fully conformant OIDC provider configuration — issuer is https://api.yieldmo.com/dcs/mcp while every endpoint lives on the Cognito domain, and required OIDC metadata such as claims_supported is absent.
  openIdConnectUrl: https://api.yieldmo.com/.well-known/openid-configuration
  sources:
  - well-known/yieldmo-openid-configuration.json
  type: openIdConnect
slug: yieldmo-authentication
source_filename: yieldmo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: >-\n  https://api.yieldmo.com/.well-known/oauth-authorization-server and\n  https://api.yieldmo.com/.well-known/openid-configuration (both HTTP 200, anonymous), plus the\n  WWW-Authenticate challenge returned by https://api.yieldmo.com/dcs/mcp\ndocs: null\ndocs_note: >-\n  Yieldmo publishes no developer authentication page. The auth model below was read entirely off the\n  wire from the provider's own discovery documents — it is observed, not documented.\n\nsummary:\n  types: [oauth2, openIdConnect]\n  api_key_in: []\n  oauth2_flows: [authorizationCode, implicit]\n  bearer_methods: [header]\n  identity_provider: Amazon Cognito\n  spec_declares_security: false\n\nschemes:\n  - name: mcp-oauth2\n    type: oauth2\n    protected_resource: https://api.yieldmo.com/dcs/mcp\n    issuer: https://api.yieldmo.com/dcs/mcp\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://yieldmo-cuba.auth.us-east-1.amazoncognito.com/oauth2/authorize\n\
  \        tokenUrl: https://yieldmo-cuba.auth.us-east-1.amazoncognito.com/oauth2/token\n        refreshUrl: https://yieldmo-cuba.auth.us-east-1.amazoncognito.com/oauth2/token\n        scopes:\n          openid: OpenID Connect subject identifier\n          profile: Basic profile claims\n          email: Email address claim\n      - flow: implicit\n        authorizationUrl: https://yieldmo-cuba.auth.us-east-1.amazoncognito.com/oauth2/authorize\n        note: response_types_supported includes \"token\", so the implicit flow is advertised.\n    token_endpoint_auth_methods: [none, client_secret_basic, client_secret_post]\n    dynamic_client_registration:\n      supported: true\n      spec: RFC 7591\n      registration_endpoint: https://api.yieldmo.com/dcs/mcp/register\n      note: >-\n        The OpenAPI labels this handler \"Fake Registration Mcp\" (operationId\n        fake_registration_mcp_register_post), which suggests it satisfies MCP client-registration\n        expectations without provisioning\
  \ a distinct Cognito app client. Behaviour unverified — the\n        endpoint returns 404 when called on the bare host path.\n    revocation_endpoint: https://yieldmo-cuba.auth.us-east-1.amazoncognito.com/oauth2/revoke\n    end_session_endpoint: https://yieldmo-cuba.auth.us-east-1.amazoncognito.com/logout\n    userinfo_endpoint: https://yieldmo-cuba.auth.us-east-1.amazoncognito.com/oauth2/userInfo\n    jwks_uri: https://cognito-idp.us-east-1.amazonaws.com/us-east-1_vZfEMm5aZ/.well-known/jwks.json\n    id_token_signing_alg: [RS256]\n    subject_types: [public]\n    sources:\n      - well-known/yieldmo-oauth-authorization-server.json\n      - well-known/yieldmo-openid-configuration.json\n      - well-known/yieldmo-oauth-protected-resource.json\n\n  - name: mcp-openid-connect\n    type: openIdConnect\n    openIdConnectUrl: https://api.yieldmo.com/.well-known/openid-configuration\n    note: >-\n      The OIDC discovery document is served at the RFC 8414 path on the API host and is byte-identical\n\
  \      to the oauth-authorization-server document. It is not a fully conformant OIDC provider\n      configuration — issuer is https://api.yieldmo.com/dcs/mcp while every endpoint lives on the\n      Cognito domain, and required OIDC metadata such as claims_supported is absent.\n    sources: [well-known/yieldmo-openid-configuration.json]\n\nchallenge:\n  observed_on: https://api.yieldmo.com/dcs/mcp\n  http_status: 401\n  www_authenticate: >-\n    Bearer error=\"invalid_token\", error_description=\"Authentication required\",\n    resource_metadata=\"https://api.yieldmo.com/.well-known/oauth-protected-resource/dcs/mcp\"\n  note: >-\n    The resource_metadata URL advertised in the challenge (path-suffixed, per RFC 9728 §3) returns\n    404; the metadata is only retrievable at the unsuffixed /.well-known/oauth-protected-resource.\n    That is a real conformance defect an agent following the challenge would hit.\n\nother_surfaces:\n  - surface: Yieldmo JavaScript SDK (ads.yieldmo.com)\n   \
  \ auth: none\n    note: >-\n      Publisher-side ad serving. Identity is the placement ID issued by Yieldmo account management;\n      there is no credential in the browser call path.\n    source: https://github.com/yieldmo/yieldmo-js-sdk/wiki/Single-page-apps\n  - surface: Prebid.js bid adapter (biddercode yieldmo)\n    auth: none\n    note: >-\n      Authorization is commercial, not technical — the placementId is provisioned by a Yieldmo\n      account manager. Prebid docs state \"reach out to your Yieldmo account's person or\n      support@yieldmo.com\" before the adapter can be used.\n    source: https://docs.prebid.org/dev-docs/bidders/yieldmo.html\n  - surface: YMax console (apps.yieldmo.com/auth)\n    auth: interactive login\n    note: Human sign-in for the Yieldmo platform; presumed to sit on the same Cognito pool, unverified.\n\nx-evidence:\n  fetched: '2026-08-12'\n  probes:\n    - {url: 'https://api.yieldmo.com/.well-known/oauth-authorization-server', status: 200}\n    - {url:\
  \ 'https://api.yieldmo.com/.well-known/openid-configuration', status: 200}\n    - {url: 'https://api.yieldmo.com/.well-known/oauth-protected-resource', status: 200}\n    - {url: 'https://api.yieldmo.com/.well-known/oauth-protected-resource/dcs/mcp', status: 404}\n    - {url: 'https://api.yieldmo.com/dcs/mcp', status: 401}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/yieldmo/refs/heads/main/authentication/yieldmo-authentication.yml
summary_line: oauth2/openIdConnect · 2 schemes
tags:
- Advertising
- Programmatic
- Native Advertising
- Ad Exchange
- Publisher Monetization
- Header Bidding
- Contextual Targeting
- Ad Formats
- Supply-Side Platform
- SSP
- Campaign Reporting
- Attention Analytics
- MCP
- Prebid
- AdTech
---
