---
api_key_in: []
auth_types:
- mutualTLS
- http-bearer
- oauth2
- openIdConnect
- saml
- http-basic
- scim
description: ''
kind: authentication
layout: security
method: searched
name: Engflow Authentication
name_suffix: Authentication
oauth_flows:
- deviceCode
- authorizationCode
- implicit
- hybrid
overview: EngFlow secures its APIs with mutualTLS, http-bearer, oauth2, openIdConnect, saml, http-basic, and scim across 7 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the deviceCode, authorizationCode, implicit, and hybrid flow(s).
provider_name: EngFlow
provider_slug: engflow
scheme_count: 7
schemes:
- description: Clients present X.509 client certificates; the CA trusted to authenticate clients is set via --tls_trusted_certificate. Authorization derives from the certificate Subject Alternative Names or Common Name.
  name: mTLS
  transport:
  - grpc
  - http
  type: mutualTLS
- bearerFormat: JWT
  description: The cluster issues and validates its own JWTs. Tokens are minted manually in the web UI (--experimental_jwt_auth) or via the engflow_auth credential helper using an OAuth2 device flow.
  header: 'Authorization: Bearer <token>'
  name: JWT Bearer Token
  scheme: bearer
  transport:
  - grpc
  - http
  type: http
- config:
  - --oidc_issuers
  - --oidc_role_mapping
  - --oidc_config
  description: External identity providers issue tokens the cluster federates. HTTP login supports Authorization Code, Implicit, and Hybrid flows.
  name: OIDC Federation
  transport:
  - grpc
  - http
  type: openIdConnect
- config:
  - --saml_config
  description: Enterprise SSO via SAML for browser/HTTP access.
  name: SAML Login
  transport:
  - http
  type: saml
- deprecated: true
  description: GitHub Personal Access Tokens or the GitHub Actions GITHUB_TOKEN (deprecated auth path).
  header: 'Authorization: Bearer $GITHUB_TOKEN'
  name: GitHub Token
  scheme: bearer
  transport:
  - grpc
  - http
  type: http
- config:
  - --basic_auth_htpasswd
  description: htpasswd file in APR1 format referenced via --basic_auth_htpasswd.
  name: Basic Auth
  scheme: basic
  transport:
  - http
  type: http
- description: Clusters expose SCIM 2.0 provisioning at /api/scim/v2/ for identity-provider user/group provisioning, secured with an OAuth bearer token.
  endpoint: /api/scim/v2/
  name: SCIM 2.0 Provisioning
  scheme: bearer
  transport:
  - http
  type: http
slug: engflow-authentication
source_filename: engflow-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://docs.engflow.com/re/config/authentication.html\ndocs: https://docs.engflow.com/re/config/authentication.html\nsummary:\n  types: [mutualTLS, http-bearer, oauth2, openIdConnect, saml, http-basic, scim]\n  transport: [grpc, http]\n  api_key_in: []\n  oauth2_flows: [deviceCode, authorizationCode, implicit, hybrid]\nschemes:\n- name: mTLS\n  type: mutualTLS\n  transport: [grpc, http]\n  description: >-\n    Clients present X.509 client certificates; the CA trusted to authenticate\n    clients is set via --tls_trusted_certificate. Authorization derives from the\n    certificate Subject Alternative Names or Common Name.\n- name: JWT Bearer Token\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  transport: [grpc, http]\n  header: 'Authorization: Bearer <token>'\n  description: >-\n    The cluster issues and validates its own JWTs. Tokens are minted manually in\n    the web UI (--experimental_jwt_auth) or via the engflow_auth\
  \ credential\n    helper using an OAuth2 device flow.\n- name: OIDC Federation\n  type: openIdConnect\n  transport: [grpc, http]\n  config: [--oidc_issuers, --oidc_role_mapping, --oidc_config]\n  description: >-\n    External identity providers issue tokens the cluster federates. HTTP login\n    supports Authorization Code, Implicit, and Hybrid flows.\n- name: SAML Login\n  type: saml\n  transport: [http]\n  config: [--saml_config]\n  description: Enterprise SSO via SAML for browser/HTTP access.\n- name: GitHub Token\n  type: http\n  scheme: bearer\n  transport: [grpc, http]\n  header: 'Authorization: Bearer $GITHUB_TOKEN'\n  deprecated: true\n  description: >-\n    GitHub Personal Access Tokens or the GitHub Actions GITHUB_TOKEN (deprecated\n    auth path).\n- name: Basic Auth\n  type: http\n  scheme: basic\n  transport: [http]\n  config: [--basic_auth_htpasswd]\n  description: htpasswd file in APR1 format referenced via --basic_auth_htpasswd.\n- name: SCIM 2.0 Provisioning\n  type: http\n\
  \  scheme: bearer\n  transport: [http]\n  endpoint: /api/scim/v2/\n  description: >-\n    Clusters expose SCIM 2.0 provisioning at /api/scim/v2/ for identity-provider\n    user/group provisioning, secured with an OAuth bearer token.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/engflow/refs/heads/main/authentication/engflow-authentication.yml
summary_line: mutualTLS/http-bearer/oauth2/openIdConnect/saml/http-basic/scim · 7 schemes
tags:
- Company
- Remote Execution
- Remote Caching
- Build Systems
- Bazel
- CI/CD
- Developer Tools
- gRPC
- Protocol Buffers
- DevOps
- Continuous Integration
---
