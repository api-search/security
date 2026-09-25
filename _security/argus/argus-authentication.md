---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication profile for the ARGUS platform (Altus Group). No public ARGUS API reference or OpenAPI is published, so nothing here is derived from a contract — every entry below was read off a live, anonymous discovery document or the platform's own front-end configuration. Two distinct identity surfaces exist, and they are not the same system.
kind: authentication
layout: security
mechanism_count: 2
method: probed
name: Argus Authentication
name_suffix: Authentication
oauth_flows: []
overview: ARGUS declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: ARGUS
provider_slug: argus
scheme_count: 2
schemes:
- applies_to:
  - ARGUS Intelligence Platform
  - ARGUS ValueInsight
  authorization_endpoint: https://login.microsoftonline.com/4299aec5-b3b8-413e-a612-88e3c0b4c972/oauth2/v2.0/authorize
  flow: authorization_code
  id: argus-intelligence-entra-oidc
  id_token_signing_alg: RS256
  issuer: https://login.microsoftonline.com/4299aec5-b3b8-413e-a612-88e3c0b4c972/v2.0
  jwks_uri: https://login.microsoftonline.com/4299aec5-b3b8-413e-a612-88e3c0b4c972/discovery/v2.0/keys
  name: ARGUS Intelligence Platform — Microsoft Entra ID (OIDC)
  note: Single-tenant Entra ID application. The platform front-end acquires a token for the resource scope above and presents it to the service prefixes listed under gated_surfaces. Anonymous callers receive HTTP 403 "Missing Authentication Token" from the fronting AWS API Gateway.
  openIdConnectUrl: https://login.microsoftonline.com/4299aec5-b3b8-413e-a612-88e3c0b4c972/v2.0/.well-known/openid-configuration
  pkce: S256
  resource_scope: api://4e11f0c5-761c-4021-a96f-82e2df6c73a9/.default
  scopes_supported:
  - openid
  - profile
  - email
  - offline_access
  subject_type: pairwise
  tenant_region_scope: EU
  token_endpoint: https://login.microsoftonline.com/4299aec5-b3b8-413e-a612-88e3c0b4c972/oauth2/v2.0/token
  token_format: JWT
  type: openIdConnect
- applies_to:
  - ARGUS support community and knowledge base
  authorization_endpoint: https://service.altusgroup.com/services/oauth2/authorize
  dpop_supported: true
  flow: authorization_code
  grant_types:
  - authorization_code
  - refresh_token
  id: argus-support-community-oidc
  id_token_signing_alg: RS256
  introspection_endpoint: https://service.altusgroup.com/services/oauth2/introspect
  issuer: https://service.altusgroup.com
  jwks_uri: https://service.altusgroup.com/id/keys
  name: ARGUS Support Community — Salesforce Experience Cloud (OIDC)
  note: This is the stock Salesforce Experience Cloud identity provider running under an Altus Group host. Its advertised scopes are the Salesforce platform set (api, web, chatter_api, pardot_api, cdp_*, einstein_gpt_api, mcp_api and so on), not ARGUS product scopes — it authenticates support-community users, not ARGUS API consumers. Recorded because it is the only OIDC discovery document the ARGUS estate serves from its own domain; see scopes/ for why no ARGUS scope catalog is published.
  openIdConnectUrl: https://service.altusgroup.com/.well-known/openid-configuration
  pkce: S256
  registration_endpoint: https://service.altusgroup.com/services/oauth2/register
  revocation_endpoint: https://service.altusgroup.com/services/oauth2/revoke
  token_endpoint: https://service.altusgroup.com/services/oauth2/token
  token_endpoint_auth_methods:
  - client_secret_post
  - client_secret_basic
  - private_key_jwt
  type: openIdConnect
  userinfo_endpoint: https://service.altusgroup.com/services/oauth2/userinfo
slug: argus-authentication
source_filename: argus-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "specification: API Commons Authentication\nspecificationVersion: '0.1'\ngenerated: '2026-09-14'\nmethod: probed\nsource: >-\n  https://service.altusgroup.com/.well-known/openid-configuration (HTTP 200),\n  https://login.microsoftonline.com/4299aec5-b3b8-413e-a612-88e3c0b4c972/v2.0/.well-known/openid-configuration\n  (HTTP 200), and https://platform.altusintelligence.com/config.js (HTTP 200), which names\n  the Entra tenant, client id and scope the ARGUS Intelligence Platform front-end requests.\nprovider: ARGUS\nproviderId: argus\ndescription: >-\n  Authentication profile for the ARGUS platform (Altus Group). No public ARGUS API\n  reference or OpenAPI is published, so nothing here is derived from a contract — every\n  entry below was read off a live, anonymous discovery document or the platform's own\n  front-end configuration. Two distinct identity surfaces exist, and they are not the same\n  system.\nschemes:\n  - id: argus-intelligence-entra-oidc\n    name: ARGUS Intelligence\
  \ Platform — Microsoft Entra ID (OIDC)\n    type: openIdConnect\n    flow: authorization_code\n    pkce: S256\n    openIdConnectUrl: >-\n      https://login.microsoftonline.com/4299aec5-b3b8-413e-a612-88e3c0b4c972/v2.0/.well-known/openid-configuration\n    issuer: https://login.microsoftonline.com/4299aec5-b3b8-413e-a612-88e3c0b4c972/v2.0\n    authorization_endpoint: >-\n      https://login.microsoftonline.com/4299aec5-b3b8-413e-a612-88e3c0b4c972/oauth2/v2.0/authorize\n    token_endpoint: >-\n      https://login.microsoftonline.com/4299aec5-b3b8-413e-a612-88e3c0b4c972/oauth2/v2.0/token\n    jwks_uri: >-\n      https://login.microsoftonline.com/4299aec5-b3b8-413e-a612-88e3c0b4c972/discovery/v2.0/keys\n    tenant_region_scope: EU\n    token_format: JWT\n    id_token_signing_alg: RS256\n    subject_type: pairwise\n    scopes_supported:\n      - openid\n      - profile\n      - email\n      - offline_access\n    resource_scope: api://4e11f0c5-761c-4021-a96f-82e2df6c73a9/.default\n    applies_to:\n\
  \      - ARGUS Intelligence Platform\n      - ARGUS ValueInsight\n    note: >-\n      Single-tenant Entra ID application. The platform front-end acquires a token for the\n      resource scope above and presents it to the service prefixes listed under\n      gated_surfaces. Anonymous callers receive HTTP 403 \"Missing Authentication Token\"\n      from the fronting AWS API Gateway.\n  - id: argus-support-community-oidc\n    name: ARGUS Support Community — Salesforce Experience Cloud (OIDC)\n    type: openIdConnect\n    flow: authorization_code\n    pkce: S256\n    openIdConnectUrl: https://service.altusgroup.com/.well-known/openid-configuration\n    issuer: https://service.altusgroup.com\n    authorization_endpoint: https://service.altusgroup.com/services/oauth2/authorize\n    token_endpoint: https://service.altusgroup.com/services/oauth2/token\n    introspection_endpoint: https://service.altusgroup.com/services/oauth2/introspect\n    revocation_endpoint: https://service.altusgroup.com/services/oauth2/revoke\n\
  \    userinfo_endpoint: https://service.altusgroup.com/services/oauth2/userinfo\n    jwks_uri: https://service.altusgroup.com/id/keys\n    registration_endpoint: https://service.altusgroup.com/services/oauth2/register\n    id_token_signing_alg: RS256\n    dpop_supported: true\n    token_endpoint_auth_methods:\n      - client_secret_post\n      - client_secret_basic\n      - private_key_jwt\n    grant_types:\n      - authorization_code\n      - refresh_token\n    applies_to:\n      - ARGUS support community and knowledge base\n    note: >-\n      This is the stock Salesforce Experience Cloud identity provider running under an\n      Altus Group host. Its advertised scopes are the Salesforce platform set (api, web,\n      chatter_api, pardot_api, cdp_*, einstein_gpt_api, mcp_api and so on), not ARGUS\n      product scopes — it authenticates support-community users, not ARGUS API consumers.\n      Recorded because it is the only OIDC discovery document the ARGUS estate serves from\n     \
  \ its own domain; see scopes/ for why no ARGUS scope catalog is published.\ngated_surfaces:\n  - name: ARGUS Intelligence Platform core service\n    base: https://platform.altusintelligence.com/core-service-v1\n    anonymous_status: 403\n    anonymous_body: '{\"message\":\"Missing Authentication Token\"}'\n  - name: ARGUS Intelligence Platform backend\n    base: https://platform.altusintelligence.com/backend-v1\n    anonymous_status: 403\n  - name: ARGUS Intelligence Platform stewardship / file upload\n    base: https://platform.altusintelligence.com/stewardship-v1\n    anonymous_status: 403\n  - name: ARGUS Intelligence Platform master data service\n    base: https://platform.altusintelligence.com/mdmapisvc-v1\n    anonymous_status: 403\n  - name: ARGUS Intelligence Platform derived domains\n    base: https://platform.altusintelligence.com/derived_domains-v1\n    anonymous_status: 403\n  - name: ARGUS Intelligence Platform stress testing\n    base: https://platform.altusintelligence.com/stress-testing-v1\n\
  \    anonymous_status: 403\n    note: >-\n      These are the versioned service prefixes the ARGUS Intelligence Platform front-end\n      calls, read from the provider's own config.js. They back the application UI; Altus\n      Group does not publish a reference or a spec for them. Every /swagger/v1/swagger.json\n      and /openapi.json probe under them returned 403.\nargus_api:\n  name: ARGUS API\n  documented_auth: not published\n  note: >-\n    Altus Group markets an \"ARGUS API\" integration gateway for cloud-enabled ARGUS\n    solutions, but publishes no public authentication reference, no base URL, and no spec.\n    The product page that described it (/argus/products/integration-solutions and\n    /solutions/argus-integrations/) now 301s to https://www.altusgroup.com/argus/, and the\n    integration-solutions download page 301s to the general downloads index. Access is\n    obtained through a customer account and the support community. Nothing is asserted here\n    about its scheme\
  \ because nothing is published.\nmaintainers:\n  - FN: Kin Lane\n    email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/argus/refs/heads/main/authentication/argus-authentication.yml
summary_line: 2 schemes
tags:
- Altus Group
- Asset Management
- Commercial Real Estate
- Fund Management
- Portfolio Management
- Real Estate Software
- Valuation
---
