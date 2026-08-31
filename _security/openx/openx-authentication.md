---
api_key_in:
- header
auth_types:
- oauth2
- openIdConnect
- apiKey
- http
description: ''
kind: authentication
layout: security
method: searched
name: Openx Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- refreshToken
overview: OpenX secures its APIs with oauth2, openIdConnect, apiKey, and http across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and refreshToken flow(s).
provider_name: OpenX
provider_slug: openx
scheme_count: 4
schemes:
- applies_to: OpenX Platform API, OpenX Reporting API, OpenX MCP server
  base_url: https://api.openx.com/api/v1/ox/4.0
  flows:
  - authorizationUrl: https://api.openx.com/oauth2/v1/authorize
    code_challenge_method: S256
    flow: authorizationCode
    refreshUrl: https://api.openx.com/oauth2/v1/token
    revocationUrl: https://api.openx.com/oauth2/v1/revoke
    scopes:
      api: Access the OpenX Platform API on the user's behalf
      email: User email claim
      offline_access: Issue a refresh token
      openid: OIDC authentication
      profile: User profile claims
    tokenUrl: https://api.openx.com/oauth2/v1/token
  id_token_signing_alg: RS256
  identity_provider:
    name: Google Cloud Identity Platform (identitytoolkit.googleapis.com)
    note: This is a resource-owner-password step in front of an authorization-code flow. The user's raw password transits the client application.
    step: The caller first exchanges the user's email + password at https://identitytoolkit.googleapis.com/v1/accounts:signInWithPassword for an idToken, then presents that idToken to the OpenX authorize / consent endpoints. OpenX publishes a fixed identity_provider_key for this call in its docs; it is not recorded here.
  name: OpenXPlatformOAuth2
  request_headers:
  - name: Authorization
    required: true
    value: Bearer <access_token>
  - name: X-Openx-Instance
    note: OpenX is multi-tenant per instance; the bearer token alone does not select a tenant.
    required: true
    value: the hostname of the instance the user is registered in
  source: https://docs.openx.com/developers/api-authentication/
  subject_types:
  - pairwise
  token_endpoint_auth_methods:
  - none
  - client_secret_basic
  - client_secret_post
  type: oauth2
- applies_to: OpenXSelect GraphQL API (https://api.openx.com/oa/graphql)
  expiration: 90 days (default and only documented value); a new key must be created on expiry
  in: header
  issuance: OpenXSelect UI > username menu > Settings > API Keys > Create New API Key
  name: OpenXSelectApiKey
  note: An unauthenticated POST to https://api.openx.com/oa/graphql returns HTTP 401 with an Apigee fault "Failed to resolve API Key variable request.header.x-apikey" (errorcode steps.oauth.v2.FailedToResolveAPIKey), confirming the gateway and the header name. The published docs say the same call returns 400; the observed status is 401.
  parameter_name: x-apikey
  rotation: manual
  scope: organization-wide (keys are issued for the whole organization)
  source: https://docs.openx.com/openxselect/oxs-api-get-started/
  type: apiKey
- applies_to: OX3 / OX4 Platform API via the OpenX-published OX3 client libraries
  client_header: X-OpenX-Client
  credentials:
  - Username
  - Password
  - Consumer Key
  - Consumer Secret
  - OAuth Realm
  endpoints:
    access_token: https://sso.openx.com/api/index/token
    authorize: https://sso.openx.com/login/process
    request_token: https://sso.openx.com/api/index/initiate
  name: OpenXLegacyOAuth1
  note: sso.openx.com — the host every OpenX-published OX3 client library signs against — returned HTTP 502 on 2026-08-13. The OAuth 1.0 path documented at /developers/api-get-started-auth/ and implemented in github.com/openx/ox-api-client-py cannot currently complete a login.
  scheme: oauth1
  session_cookie: openx3_access_token
  source: https://docs.openx.com/developers/api-get-started-auth/
  status: broken
  type: http
- applies_to: OpenXBuild Real-Time Bidstream API (partner-implemented enrichment service)
  name: OpenXBuildEnrichmentService
  note: The enrichment container runs inside OpenX's own Kubernetes namespace with egress blocked, so the POST /openrtb25 and ARTF gRPC surfaces are secured by network placement and GCP workload identity rather than by an API credential. Object-store access is granted to partner-supplied GCP principals.
  source: https://docs.openx.com/marketers/openxbuild/oxb-rtb-api-spec/
  type: none
slug: openx-authentication
source_filename: openx-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: searched\nsource: https://docs.openx.com/developers/api-authentication/\ndocs:\n  - https://docs.openx.com/developers/api-authentication/\n  - https://docs.openx.com/developers/api-get-started-auth/\n  - https://docs.openx.com/openxselect/oxs-api-get-started/\n  - https://api.openx.com/.well-known/openid-configuration\n  - https://api.openx.com/.well-known/oauth-protected-resource\nnote: >-\n  OpenX publishes no OpenAPI, so this profile is read from the provider's own\n  authentication documentation and from the live OIDC/OAuth discovery documents\n  served at api.openx.com. Three distinct auth models are in production at once,\n  and a fourth (OAuth 1.0) is documented but its host is down.\nsummary:\n  types: [oauth2, openIdConnect, apiKey, http]\n  api_key_in: [header]\n  oauth2_flows: [authorizationCode, refreshToken]\n  pkce: S256\n  bearer_in: [header]\nschemes:\n  - name: OpenXPlatformOAuth2\n    type: oauth2\n    applies_to: OpenX Platform\
  \ API, OpenX Reporting API, OpenX MCP server\n    source: https://docs.openx.com/developers/api-authentication/\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://api.openx.com/oauth2/v1/authorize\n        tokenUrl: https://api.openx.com/oauth2/v1/token\n        refreshUrl: https://api.openx.com/oauth2/v1/token\n        revocationUrl: https://api.openx.com/oauth2/v1/revoke\n        code_challenge_method: S256\n        scopes:\n          api: Access the OpenX Platform API on the user's behalf\n          openid: OIDC authentication\n          email: User email claim\n          profile: User profile claims\n          offline_access: Issue a refresh token\n    identity_provider:\n      name: Google Cloud Identity Platform (identitytoolkit.googleapis.com)\n      step: >-\n        The caller first exchanges the user's email + password at\n        https://identitytoolkit.googleapis.com/v1/accounts:signInWithPassword\n        for an idToken, then presents that idToken\
  \ to the OpenX authorize /\n        consent endpoints. OpenX publishes a fixed identity_provider_key for\n        this call in its docs; it is not recorded here.\n      note: >-\n        This is a resource-owner-password step in front of an authorization-code\n        flow. The user's raw password transits the client application.\n    request_headers:\n      - name: Authorization\n        value: Bearer <access_token>\n        required: true\n      - name: X-Openx-Instance\n        value: the hostname of the instance the user is registered in\n        required: true\n        note: >-\n          OpenX is multi-tenant per instance; the bearer token alone does not\n          select a tenant.\n    base_url: https://api.openx.com/api/v1/ox/4.0\n    token_endpoint_auth_methods: [none, client_secret_basic, client_secret_post]\n    id_token_signing_alg: RS256\n    subject_types: [pairwise]\n  - name: OpenXSelectApiKey\n    type: apiKey\n    in: header\n    parameter_name: x-apikey\n    applies_to:\
  \ OpenXSelect GraphQL API (https://api.openx.com/oa/graphql)\n    source: https://docs.openx.com/openxselect/oxs-api-get-started/\n    issuance: OpenXSelect UI > username menu > Settings > API Keys > Create New API Key\n    scope: organization-wide (keys are issued for the whole organization)\n    expiration: 90 days (default and only documented value); a new key must be created on expiry\n    rotation: manual\n    note: >-\n      An unauthenticated POST to https://api.openx.com/oa/graphql returns\n      HTTP 401 with an Apigee fault\n      \"Failed to resolve API Key variable request.header.x-apikey\"\n      (errorcode steps.oauth.v2.FailedToResolveAPIKey), confirming the gateway\n      and the header name. The published docs say the same call returns 400;\n      the observed status is 401.\n  - name: OpenXLegacyOAuth1\n    type: http\n    scheme: oauth1\n    applies_to: OX3 / OX4 Platform API via the OpenX-published OX3 client libraries\n    source: https://docs.openx.com/developers/api-get-started-auth/\n\
  \    credentials: [Username, Password, Consumer Key, Consumer Secret, OAuth Realm]\n    endpoints:\n      request_token: https://sso.openx.com/api/index/initiate\n      authorize: https://sso.openx.com/login/process\n      access_token: https://sso.openx.com/api/index/token\n    session_cookie: openx3_access_token\n    client_header: X-OpenX-Client\n    status: broken\n    note: >-\n      sso.openx.com — the host every OpenX-published OX3 client library signs\n      against — returned HTTP 502 on 2026-08-13. The OAuth 1.0 path documented\n      at /developers/api-get-started-auth/ and implemented in\n      github.com/openx/ox-api-client-py cannot currently complete a login.\n  - name: OpenXBuildEnrichmentService\n    type: none\n    applies_to: OpenXBuild Real-Time Bidstream API (partner-implemented enrichment service)\n    source: https://docs.openx.com/marketers/openxbuild/oxb-rtb-api-spec/\n    note: >-\n      The enrichment container runs inside OpenX's own Kubernetes namespace with\n\
  \      egress blocked, so the POST /openrtb25 and ARTF gRPC surfaces are secured\n      by network placement and GCP workload identity rather than by an API\n      credential. Object-store access is granted to partner-supplied GCP\n      principals.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/openx/refs/heads/main/authentication/openx-authentication.yml
summary_line: oauth2/openIdConnect/apiKey/http · 4 schemes
tags:
- Advertising
- Programmatic Advertising
- Ad Exchange
- Supply Side Platform
- SSP
- Real Time Bidding
- OpenRTB
- Header Bidding
- Prebid
- AdTech
- CTV
- Video Advertising
- Display Advertising
- Curation
- Identity
- GraphQL
- gRPC
- MCP
- Reporting
- Audience Targeting
---
