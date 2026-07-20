---
api_key_in: []
auth_types:
- oauth2
- openIdConnect
- apiKey
- http
description: ''
kind: authentication
layout: security
method: searched
name: Episerver Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
- authorizationCode
overview: Episerver secures its APIs with oauth2, openIdConnect, apiKey, and http across 6 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials and authorizationCode flow(s).
provider_name: Episerver
provider_slug: episerver
scheme_count: 6
schemes:
- description: OpenID Connect via Opti ID. Access authorized on JWTs issued by Opti ID or a federated IdP; access decided from claims (sub, cg-roles, email). Bearer JWT in the Authorization header.
  name: OptiIdOIDC
  product: Optimizely Graph / platform
  type: openIdConnect
- description: Single-key access for read scenarios (public content delivery).
  in: query
  name: GraphSingleKey
  parameter_name: auth
  product: Optimizely Graph
  type: apiKey
- description: HMAC (app key + secret) signed requests for write/management scenarios.
  name: GraphHMAC
  product: Optimizely Graph
  scheme: hmac
  type: http
- description: Basic authentication for trusted backend service calls.
  name: BasicAuth
  product: Optimizely Graph / backend services
  scheme: basic
  type: http
- description: Personal access token / OAuth2 bearer token for the api.optimizely.com REST API.
  name: FeatureExperimentationApiToken
  product: Optimizely Feature Experimentation REST API
  scheme: bearer
  type: http
- description: Public/private API key for ODP REST and GraphQL endpoints.
  in: header
  name: OdpApiKey
  parameter_name: x-api-key
  product: Optimizely Data Platform (ODP)
  type: apiKey
slug: episerver-authentication
source_filename: episerver-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://docs.developers.optimizely.com/platform-optimizely/docs/authentication-with-oidc-for-optimizely-graph\ndocs:\n  - https://docs.developers.optimizely.com/platform-optimizely/docs/authentication-with-oidc-for-optimizely-graph\n  - https://docs.developers.optimizely.com/commerce-connect/docs/authorization-and-authentication\nnotes: >-\n  No OpenAPI is captured in this repo yet, so this profile is searched from the\n  Optimizely developer docs rather than derived. Optimizely's platform spans several\n  products with distinct auth models; Opti ID is the unifying OIDC identity platform.\nsummary:\n  types: [oauth2, openIdConnect, apiKey, http]\n  identity_platform: Opti ID (unified OIDC identity)\n  oauth2_flows: [clientCredentials, authorizationCode]\nschemes:\n  - name: OptiIdOIDC\n    type: openIdConnect\n    product: Optimizely Graph / platform\n    description: >-\n      OpenID Connect via Opti ID. Access authorized\
  \ on JWTs issued by Opti ID or a\n      federated IdP; access decided from claims (sub, cg-roles, email). Bearer JWT\n      in the Authorization header.\n  - name: GraphSingleKey\n    type: apiKey\n    in: query\n    parameter_name: auth\n    product: Optimizely Graph\n    description: Single-key access for read scenarios (public content delivery).\n  - name: GraphHMAC\n    type: http\n    scheme: hmac\n    product: Optimizely Graph\n    description: HMAC (app key + secret) signed requests for write/management scenarios.\n  - name: BasicAuth\n    type: http\n    scheme: basic\n    product: Optimizely Graph / backend services\n    description: Basic authentication for trusted backend service calls.\n  - name: FeatureExperimentationApiToken\n    type: http\n    scheme: bearer\n    product: Optimizely Feature Experimentation REST API\n    description: Personal access token / OAuth2 bearer token for the api.optimizely.com REST API.\n  - name: OdpApiKey\n    type: apiKey\n    in: header\n \
  \   parameter_name: x-api-key\n    product: Optimizely Data Platform (ODP)\n    description: Public/private API key for ODP REST and GraphQL endpoints.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/episerver/refs/heads/main/authentication/episerver-authentication.yml
summary_line: oauth2/openIdConnect/apiKey/http · 6 schemes
tags:
- Company
- Enterprise
- Content Management
- Digital Experience Platform
- CMS
- Commerce
- Experimentation
- Personalization
- GraphQL
- SDKs
---
