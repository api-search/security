---
api_key_in:
- header
auth_types:
- oauth2
- openIdConnect
- saml
- apiKey
- preSharedSecret
description: ''
kind: authentication
layout: security
method: searched
name: Codafication Authentication
name_suffix: Authentication
oauth_flows: []
overview: Codafication secures its APIs with oauth2, openIdConnect, saml, apiKey, and preSharedSecret across 4 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Codafication
provider_slug: codafication
scheme_count: 4
schemes:
- connections:
  - SAML 2.0
  - Active Directory
  description: All end-user authentication for Unity Platform applications is handled by Auth0. The Portal SDK (UnitySDK React component) handles user login and token renewal, and authorizes the GraphQL client used for calls to the platform.
  name: Auth0 user authentication
  provider: Auth0
  source: https://docs.unitycloud.io/#security
  type: openIdConnect
- description: A Unity Token is required to communicate with the Unity Platform. Tokens are created from the in-product Developer Portal under "Developer Portal > API Tokens". No public self-serve issuance surface is published.
  in: header
  issued_via: Developer Portal > API Tokens (in-product, tenant-scoped)
  name: Unity Token
  source: https://docs.unitycloud.io/#configuration
  type: apiKey
- configured_in:
  - Unity SDK constructor (authenticationSecret)
  - Unity Developer Portal extension configuration
  description: Backend extensions authenticate to the Unity Platform with a pre-shared key passed as the authenticationSecret field of the Unity SDK constructor. The same key must be registered on both sides - in the extension configuration and in the Unity Developer Portal - for all requests and actions from that extension.
  name: Extension authenticationSecret
  source: https://docs.unitycloud.io/#configuration
  type: preSharedSecret
- applies_to: https://<CloudDomain>/graphql/v2/<extensionName>/<endpoint>
  description: Extension REST endpoints registered with unity.post/unity.get are private and require an authorization token in the request header. Endpoints registered with publicPost/publicGet are callable with no Unity authorization.
  name: Private REST endpoint authorization header
  scheme: bearer
  source: https://docs.unitycloud.io/#rest-endpoints
  type: http
slug: codafication-authentication
source_filename: codafication-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: searched\nsource: https://docs.unitycloud.io/\ndocs: https://docs.unitycloud.io/#security\nnote: >-\n  Derived by reading the public Unity Platform SDK reference. There is no OpenAPI\n  document to mechanically derive securitySchemes from, so every scheme below is\n  transcribed from what the documentation states. Nothing was inferred from the\n  gated application hosts.\nsummary:\n  types:\n  - oauth2\n  - openIdConnect\n  - saml\n  - apiKey\n  - preSharedSecret\n  api_key_in:\n  - header\n  identity_provider: Auth0\n  multi_tenant: true\n  authorization_model: role-based access control with granular permissions\nschemes:\n- name: Auth0 user authentication\n  type: openIdConnect\n  provider: Auth0\n  description: >-\n    All end-user authentication for Unity Platform applications is handled by Auth0.\n    The Portal SDK (UnitySDK React component) handles user login and token renewal,\n    and authorizes the GraphQL client used for calls to\
  \ the platform.\n  connections:\n  - SAML 2.0\n  - Active Directory\n  source: https://docs.unitycloud.io/#security\n- name: Unity Token\n  type: apiKey\n  in: header\n  description: >-\n    A Unity Token is required to communicate with the Unity Platform. Tokens are\n    created from the in-product Developer Portal under \"Developer Portal > API Tokens\".\n    No public self-serve issuance surface is published.\n  issued_via: Developer Portal > API Tokens (in-product, tenant-scoped)\n  source: https://docs.unitycloud.io/#configuration\n- name: Extension authenticationSecret\n  type: preSharedSecret\n  description: >-\n    Backend extensions authenticate to the Unity Platform with a pre-shared key passed\n    as the authenticationSecret field of the Unity SDK constructor. The same key must be\n    registered on both sides - in the extension configuration and in the Unity Developer\n    Portal - for all requests and actions from that extension.\n  configured_in:\n  - Unity SDK constructor\
  \ (authenticationSecret)\n  - Unity Developer Portal extension configuration\n  source: https://docs.unitycloud.io/#configuration\n- name: Private REST endpoint authorization header\n  type: http\n  scheme: bearer\n  description: >-\n    Extension REST endpoints registered with unity.post/unity.get are private and\n    require an authorization token in the request header. Endpoints registered with\n    publicPost/publicGet are callable with no Unity authorization.\n  applies_to: https://<CloudDomain>/graphql/v2/<extensionName>/<endpoint>\n  source: https://docs.unitycloud.io/#rest-endpoints\nauthorization:\n  model: RBAC\n  description: >-\n    The Unity API is the centralised point of control for role-based access control and\n    granular permissions in a multi-tenant environment. All GraphQL queries and mutations\n    are secure by default and can be whitelisted to users across multiple authentication\n    connections. Permissions are grouped into internal security roles scoped to a\
  \ tenant,\n    which are then mapped to external security roles supplied by the customer's enterprise\n    user directory, giving customers automatic user onboarding under their own role names.\n  tenant_scoped: true\n  external_role_mapping: true\n  source: https://docs.unitycloud.io/#security\nprovisioning:\n  scim:\n    host: https://scim.codafication.com/\n    status: 0\n    note: >-\n      Host resolves (34.116.97.51) but the TCP connection times out for anonymous\n      clients, consistent with an IP-allowlisted enterprise SCIM endpoint. No SCIM\n      behaviour is documented publicly and none was assumed.\nnot_published:\n- OAuth 2.0 authorization server metadata (/.well-known/oauth-authorization-server returns the site bot challenge)\n- OpenID Connect discovery document (/.well-known/openid-configuration returns the site bot challenge)\n- A scopes / permissions reference listing named scope strings\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/codafication/refs/heads/main/authentication/codafication-authentication.yml
summary_line: oauth2/openIdConnect/saml/apiKey/preSharedSecret · 4 schemes
tags:
- Insurance
- Australia
- Insurtech
- Claims
- Claims Management
- Property and Casualty
- FNOL
- Supply Chain
- GraphQL
- Webhook
- SDK
- Extensions
- Multi Tenant
- Partner Gated
---
