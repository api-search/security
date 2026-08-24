---
api_key_in:
- header
api_specs:
- filename: immutable-zkevm-openapi.json
  format: json
  label: Immutable zkEVM API
  slug: immutable-zkevm-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/immutable/refs/heads/main/openapi/immutable-zkevm-openapi.json
- filename: immutable-audience-openapi.json
  format: json
  label: Immutable Audience API
  slug: immutable-audience-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/immutable/refs/heads/main/openapi/immutable-audience-openapi.json
auth_types:
- apiKey
- http
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Immutable Authentication
name_suffix: Authentication
oauth_flows: []
overview: Immutable secures its APIs with apiKey, http, and openIdConnect across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Immutable
provider_slug: immutable
scheme_count: 4
schemes:
- docs: https://docs.immutable.com/docs/guides/advanced-setup/api-keys
  in: header
  issued_by: https://hub.immutable.com
  key_prefixes:
    publishable: pk_imapik-
    publishable_sandbox: pk_imapik-sandbox-
  name: ImmutableApiKey
  parameter: x-immutable-api-key
  sources:
  - openapi/immutable-audience-openapi.json
  - openapi/immutable-zkevm-openapi.json
  type: apiKey
- bearerFormat: JWT
  name: BearerAuth
  note: Passport user access token.
  scheme: bearer
  sources:
  - openapi/immutable-zkevm-openapi.json
  type: http
- bearerFormat: JWT
  name: BearerAuthWithClient
  note: Same JWT bearer shape as BearerAuth; the spec declares it separately for operations that additionally resolve the calling Passport client.
  scheme: bearer
  sources:
  - openapi/immutable-zkevm-openapi.json
  type: http
- bearerFormat: JWT
  name: OktaBearerAuth
  note: Declared in the spec for internal/administrative operations (e.g. the internal collection-metadata refresh). Not a scheme a public integrator obtains a token for.
  scheme: bearer
  sources:
  - openapi/immutable-zkevm-openapi.json
  type: http
slug: immutable-authentication
source_filename: immutable-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-23'\nmethod: searched\nsource: openapi/immutable-zkevm-openapi.json, openapi/immutable-audience-openapi.json\ndocs:\n- https://docs.immutable.com/docs/guides/advanced-setup/api-keys\n- https://docs.immutable.com/docs/products/passport/authentication\n- https://auth.immutable.com/.well-known/openid-configuration\nsummary:\n  types:\n  - apiKey\n  - http\n  - openIdConnect\n  api_key_in:\n  - header\n  models:\n  - name: Immutable API key\n    detail: >-\n      Two key classes issued per project in Immutable Hub. A PUBLISHABLE key\n      (prefix `pk_imapik-`, sandbox variant `pk_imapik-sandbox-`) initialises\n      client-side SDKs and is safe to expose. A SECRET key is server-side only\n      and is what the REST surface accepts in the `x-immutable-api-key` header —\n      minting, admin operations and webhook verification. Keys are rotated in\n      Hub under Settings -> API Keys, and rotation invalidates the old key\n      immediately.\n  - name: Passport\
  \ OIDC bearer token\n    detail: >-\n      User-scoped JWT access tokens minted by the Passport OpenID Connect\n      provider at auth.immutable.com and presented as `Authorization: Bearer`.\n      This is what the passport / passport-profile operations in the zkEVM API\n      require.\nschemes:\n- name: ImmutableApiKey\n  type: apiKey\n  in: header\n  parameter: x-immutable-api-key\n  key_prefixes:\n    publishable: pk_imapik-\n    publishable_sandbox: pk_imapik-sandbox-\n  issued_by: https://hub.immutable.com\n  sources:\n  - openapi/immutable-audience-openapi.json\n  - openapi/immutable-zkevm-openapi.json\n  docs: https://docs.immutable.com/docs/guides/advanced-setup/api-keys\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/immutable-zkevm-openapi.json\n  note: Passport user access token.\n- name: BearerAuthWithClient\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/immutable-zkevm-openapi.json\n  note: >-\n\
  \    Same JWT bearer shape as BearerAuth; the spec declares it separately for\n    operations that additionally resolve the calling Passport client.\n- name: OktaBearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/immutable-zkevm-openapi.json\n  note: >-\n    Declared in the spec for internal/administrative operations (e.g. the\n    internal collection-metadata refresh). Not a scheme a public integrator\n    obtains a token for.\nopenid_connect:\n  issuer: https://auth.immutable.com/\n  discovery: well-known/immutable-openid-configuration.json\n  authorization_endpoint: https://auth.immutable.com/authorize\n  token_endpoint: https://auth.immutable.com/oauth/token\n  device_authorization_endpoint: https://auth.immutable.com/oauth/device/code\n  userinfo_endpoint: https://auth.immutable.com/userinfo\n  jwks_uri: https://auth.immutable.com/.well-known/jwks.json\n  registration_endpoint: https://auth.immutable.com/oidc/register\n  revocation_endpoint: https://auth.immutable.com/oauth/revoke\n\
  \  pkce: true\n  code_challenge_methods:\n  - S256\n  - plain\n  grant_types:\n  - authorization_code\n  - refresh_token\n  - client_credentials\n  - implicit\n  - password\n  - urn:ietf:params:oauth:grant-type:device_code\n  - urn:ietf:params:oauth:grant-type:token-exchange\n  - urn:ietf:params:oauth:grant-type:jwt-bearer\n  token_endpoint_auth_methods:\n  - client_secret_basic\n  - client_secret_post\n  - private_key_jwt\n  - none\n  dpop_signing_alg_values_supported:\n  - ES256\n  note: >-\n    The discovery document's auth0.com-namespaced grant types show the provider\n    is an Auth0 tenant operated under Immutable's own auth.immutable.com issuer.\nunauthenticated_access:\n  observed: true\n  evidence: 'GET https://api.immutable.com/v1/chains returned HTTP 200 with no credentials on 2026-08-23'\n  note: >-\n    Public read endpoints on the zkEVM API (chains, collections, NFTs, orders)\n    answer anonymously but at a much lower rate limit — the observed anonymous\n    ceiling was\
  \ 5 requests per second. See rate-limits/immutable-rate-limits.yml.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/immutable/refs/heads/main/authentication/immutable-authentication.yml
summary_line: apiKey/http/openIdConnect · 4 schemes
tags:
- Company
- Gaming
- Blockchain
- NFT
- Web3
- Wallets
- Marketplace
- Analytics
- Attribution
- Customer Data Platform
- Authentication
- Developer Platform
---
