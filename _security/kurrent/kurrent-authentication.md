---
api_key_in: []
api_specs:
- filename: kurrent-kurrentdb-http-api-openapi.yml
  format: yaml
  label: KurrentDB HTTP API
  slug: kurrentdb-http-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kurrent/refs/heads/main/openapi/kurrent-kurrentdb-http-api-openapi.yml
auth_types:
- http
- mutualTLS
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Kurrent Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
- deviceCode
overview: Kurrent secures its APIs with http, mutualTLS, and openIdConnect across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, clientCredentials, and deviceCode flow(s).
provider_name: Kurrent
provider_slug: kurrent
scheme_count: 3
schemes:
- description: KurrentDB supports HTTP Basic authentication for the HTTP API. Credentials are supplied per request; the default administrative user is created at first start. Authorization is enforced by access control lists set on stream metadata ($acl with $r/$w/$d/$mr/$mw entries) and by the default ACL on the $settings stream.
  docs: https://docs.kurrent.io/server/v26.1/http-api/security.html
  name: basicAuth
  scheme: basic
  sources:
  - openapi/kurrent-kurrentdb-http-api-openapi.yml
  surface: KurrentDB HTTP API
  type: http
- description: X.509 client-certificate authentication, introduced with EventStoreDB 24.2, lets clients and nodes authenticate with certificates instead of a username and password.
  docs: https://docs.kurrent.io/server/v26.1/security/
  name: clientCertificate
  sources:
  - https://www.kurrent.io/releases
  surface: KurrentDB server (commercial editions)
  type: mutualTLS
- description: Kurrent Cloud authenticates users and machine clients through its OpenID Connect provider, which supports the authorization code flow with PKCE, client credentials, the device authorization grant, refresh tokens and multi-factor challenges.
  issuer: https://identity.eventstore.com/
  name: KurrentCloudOIDC
  openIdConnectUrl: https://identity.eventstore.com/.well-known/openid-configuration
  scopes: scopes/kurrent-scopes.yml
  sources:
  - well-known/kurrent-openid-configuration.json
  - well-known/kurrent-oauth-authorization-server.json
  surface: Kurrent Cloud console and control plane
  type: openIdConnect
slug: kurrent-authentication
source_filename: kurrent-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: openapi/kurrent-kurrentdb-http-api-openapi.yml\ndocs: https://docs.kurrent.io/server/v26.1/http-api/security.html\nnotes: >-\n  Kurrent has two distinct authentication surfaces. The KurrentDB database itself authenticates\n  with HTTP Basic credentials (or X.509 client certificates in the commercial editions) and\n  authorizes with per-stream access control lists plus, since 24.10, policy-based authorization.\n  Kurrent Cloud — the managed control plane and console — authenticates with OpenID Connect\n  against identity.eventstore.com. The derived spec profile covers only the first; the docs pass\n  added the rest.\nsummary:\n  types:\n  - http\n  - mutualTLS\n  - openIdConnect\n  http_schemes:\n  - basic\n  api_key_in: []\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\n  - deviceCode\nschemes:\n- name: basicAuth\n  type: http\n  scheme: basic\n  surface: KurrentDB HTTP API\n  description: >-\n    KurrentDB\
  \ supports HTTP Basic authentication for the HTTP API. Credentials are supplied per\n    request; the default administrative user is created at first start. Authorization is enforced\n    by access control lists set on stream metadata ($acl with $r/$w/$d/$mr/$mw entries) and by the\n    default ACL on the $settings stream.\n  docs: https://docs.kurrent.io/server/v26.1/http-api/security.html\n  sources:\n  - openapi/kurrent-kurrentdb-http-api-openapi.yml\n- name: clientCertificate\n  type: mutualTLS\n  surface: KurrentDB server (commercial editions)\n  description: >-\n    X.509 client-certificate authentication, introduced with EventStoreDB 24.2, lets clients and\n    nodes authenticate with certificates instead of a username and password.\n  docs: https://docs.kurrent.io/server/v26.1/security/\n  sources:\n  - https://www.kurrent.io/releases\n- name: KurrentCloudOIDC\n  type: openIdConnect\n  surface: Kurrent Cloud console and control plane\n  issuer: https://identity.eventstore.com/\n\
  \  openIdConnectUrl: https://identity.eventstore.com/.well-known/openid-configuration\n  description: >-\n    Kurrent Cloud authenticates users and machine clients through its OpenID Connect provider,\n    which supports the authorization code flow with PKCE, client credentials, the device\n    authorization grant, refresh tokens and multi-factor challenges.\n  scopes: scopes/kurrent-scopes.yml\n  sources:\n  - well-known/kurrent-openid-configuration.json\n  - well-known/kurrent-oauth-authorization-server.json\nauthorization:\n  model: access-control-lists\n  description: >-\n    Per-stream ACLs are written into stream metadata; a default ACL applies from the $settings\n    stream. KurrentDB 24.10 added policy-based authorization as a commercial feature for\n    expressing access rules centrally rather than per stream.\n  docs: https://docs.kurrent.io/server/v26.1/http-api/security.html\nsdk_authentication:\n  description: >-\n    Client SDKs carry credentials in the connection string\
  \ (for example\n    kurrentdb://user:password@host:2113) or per call. Each SDK has a dedicated authentication page\n    in the client documentation.\n  docs: https://docs.kurrent.io/clients/\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kurrent/refs/heads/main/authentication/kurrent-authentication.yml
summary_line: http/mutualTLS/openIdConnect · 3 schemes
tags:
- Company
- Database
- Event Sourcing
- Event Streaming
- Event Driven Architecture
- CQRS
- Data Infrastructure
- Developer Tools
- Cloud
- Open Source
- gRPC
- Agentic AI
---
