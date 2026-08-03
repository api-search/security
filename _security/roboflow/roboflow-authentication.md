---
api_key_in:
- query
- header
- body
api_specs:
- filename: roboflow-inference-openapi.json
  format: json
  label: Roboflow Inference Server API
  slug: inference
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/roboflow/refs/heads/main/openapi/roboflow-inference-openapi.json
auth_types:
- apiKey
- http
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Roboflow Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Roboflow secures its APIs with apiKey, http, oauth2, and openIdConnect across 5 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Roboflow
provider_slug: roboflow
scheme_count: 5
schemes:
- description: Workspace-scoped Roboflow API key passed as a query parameter on REST and inference calls.
  docs: https://docs.roboflow.com/reference/authentication/authentication/find-your-roboflow-api-key.md
  in: query
  name: api_key
  parameter: api_key
  type: apiKey
- description: The same API key may be sent in the JSON request body on POST calls.
  in: body
  name: api_key_body
  parameter: api_key
  type: apiKey
- description: 'Authorization: Bearer <api_key> header form accepted by the REST API, and the required form for OAuth access tokens on the MCP server.'
  name: bearer
  scheme: bearer
  type: http
- description: '"Sign in with Roboflow" — OAuth 2.1 authorization code + PKCE with RFC 7591 dynamic client registration. Used by the hosted MCP server.'
  flows:
    authorizationCode:
      authorizationUrl: https://app.roboflow.com/oauth/authorize
      refreshUrl: https://app.roboflow.com/oauth/token
      scope_count: 67
      tokenUrl: https://app.roboflow.com/oauth/token
  introspection_endpoint: https://app.roboflow.com/oauth/introspect
  name: oauth2
  registration_endpoint: https://app.roboflow.com/oauth/register
  revocation_endpoint: https://app.roboflow.com/oauth/revoke
  source: well-known/roboflow-oauth-authorization-server.json
  type: oauth2
- id_token_signing_alg_values_supported:
  - RS256
  issuer: https://app.roboflow.com
  jwks_uri: https://app.roboflow.com/.well-known/jwks.json
  name: openIdConnect
  openIdConnectUrl: https://app.roboflow.com/.well-known/openid-configuration
  source: well-known/roboflow-openid-configuration.json
  type: openIdConnect
slug: roboflow-authentication
source_filename: roboflow-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: searched\ndocs: https://docs.roboflow.com/reference/authentication/authentication.md\nsource: https://docs.roboflow.com/reference/platform/rest-api/authenticate-with-the-rest-api.md\nsummary:\n  types:\n  - apiKey\n  - http\n  - oauth2\n  - openIdConnect\n  api_key_in:\n  - query\n  - header\n  - body\n  oauth2_flows:\n  - authorizationCode\n  pkce:\n  - S256\n  dynamic_client_registration: true\n  scoped_api_keys: true\nschemes:\n- name: api_key\n  type: apiKey\n  in: query\n  parameter: api_key\n  description: Workspace-scoped Roboflow API key passed as a query parameter on REST and inference calls.\n  docs: https://docs.roboflow.com/reference/authentication/authentication/find-your-roboflow-api-key.md\n- name: api_key_body\n  type: apiKey\n  in: body\n  parameter: api_key\n  description: The same API key may be sent in the JSON request body on POST calls.\n- name: bearer\n  type: http\n  scheme: bearer\n  description: 'Authorization: Bearer\
  \ <api_key> header form accepted by the REST API, and the required\n    form for OAuth access tokens on the MCP server.'\n- name: oauth2\n  type: oauth2\n  flows:\n    authorizationCode:\n      authorizationUrl: https://app.roboflow.com/oauth/authorize\n      tokenUrl: https://app.roboflow.com/oauth/token\n      refreshUrl: https://app.roboflow.com/oauth/token\n      scope_count: 67\n  description: '\"Sign in with Roboflow\" — OAuth 2.1 authorization code + PKCE with RFC 7591 dynamic client\n    registration. Used by the hosted MCP server.'\n  registration_endpoint: https://app.roboflow.com/oauth/register\n  introspection_endpoint: https://app.roboflow.com/oauth/introspect\n  revocation_endpoint: https://app.roboflow.com/oauth/revoke\n  source: well-known/roboflow-oauth-authorization-server.json\n- name: openIdConnect\n  type: openIdConnect\n  openIdConnectUrl: https://app.roboflow.com/.well-known/openid-configuration\n  issuer: https://app.roboflow.com\n  jwks_uri: https://app.roboflow.com/.well-known/jwks.json\n\
  \  id_token_signing_alg_values_supported:\n  - RS256\n  source: well-known/roboflow-openid-configuration.json\nkey_management:\n  scoped_api_keys: https://docs.roboflow.com/reference/authentication/authentication/scoped-api-keys.md\n  manage: https://docs.roboflow.com/reference/authentication/authentication/manage-api-keys.md\n  console: https://app.roboflow.com/settings/api\nenterprise:\n  sso: https://docs.roboflow.com/platform/enterprise-features/single-sign-on-sso.md\n  rbac: https://docs.roboflow.com/platform/enterprise-features/role-based-access-control.md\n  scim_group_sync: Active Directory group sync for SSO (changelog, May 2026)\nnotes: The public Inference Server OpenAPI declares no securitySchemes — inference auth is carried by\n  the api_key query parameter documented in the platform docs, not in the spec.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/roboflow/refs/heads/main/authentication/roboflow-authentication.yml
summary_line: apiKey/http/oauth2/openIdConnect · 5 schemes
tags:
- Computer Vision
- Machine Learning
- Artificial Intelligence
- Object Detection
- Image Annotation
- Model Training
- Inference
- MLOps
- Edge AI
- Datasets
---
