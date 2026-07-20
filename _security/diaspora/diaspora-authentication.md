---
api_key_in: []
api_specs:
- filename: diaspora-api-openapi.yml
  format: yaml
  label: diaspora* API
  slug: diaspora-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/diaspora/refs/heads/main/openapi/diaspora-api-openapi.yml
auth_types:
- openIdConnect
description: diaspora* authenticates API clients with OpenID Connect Core 1.0. Because diaspora* is decentralized, a manual application registration on a single pod is not sufficient, so the project also implements OpenID Connect Discovery 1.0 and OpenID Connect Dynamic Client Registration 1.0 — an application discovers a pod's endpoints and registers itself at runtime against pods it has never seen before. There is no static API key and no shared client credential across the network.
kind: authentication
layout: security
method: searched
name: Diaspora Authentication
name_suffix: Authentication
oauth_flows: []
overview: Diaspora secures its APIs with openIdConnect across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Diaspora
provider_slug: diaspora
scheme_count: 1
schemes:
- description: OpenID Connect Core 1.0 using either the Authorization Code Flow or the Implicit Flow. The openid scope is mandatory; public:read is always granted to any authorized client.
  name: openIdConnect
  openIdConnectUrl: https://diaspora.social/.well-known/openid-configuration
  sources:
  - openapi/diaspora-api-openapi.yml
  - https://diaspora.github.io/api-documentation/authentication.html
  type: openIdConnect
slug: diaspora-authentication
source_filename: diaspora-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: searched\nsource: >-\n  https://diaspora.github.io/api-documentation/authentication.html — the official diaspora* API\n  authentication documentation, corroborated by a live fetch of\n  https://diaspora.social/.well-known/openid-configuration (HTTP 200) and\n  openapi/diaspora-api-openapi.yml.\ndocs: https://diaspora.github.io/api-documentation/authentication.html\ndescription: >-\n  diaspora* authenticates API clients with OpenID Connect Core 1.0. Because diaspora* is\n  decentralized, a manual application registration on a single pod is not sufficient, so the\n  project also implements OpenID Connect Discovery 1.0 and OpenID Connect Dynamic Client\n  Registration 1.0 — an application discovers a pod's endpoints and registers itself at runtime\n  against pods it has never seen before. There is no static API key and no shared client\n  credential across the network.\n\nsummary:\n  types:\n  - openIdConnect\n  primary: openIdConnect\n  static_api_keys:\
  \ false\n  per_pod_registration: true\n\nschemes:\n- name: openIdConnect\n  type: openIdConnect\n  openIdConnectUrl: https://diaspora.social/.well-known/openid-configuration\n  description: >-\n    OpenID Connect Core 1.0 using either the Authorization Code Flow or the Implicit Flow. The\n    openid scope is mandatory; public:read is always granted to any authorized client.\n  sources:\n  - openapi/diaspora-api-openapi.yml\n  - https://diaspora.github.io/api-documentation/authentication.html\n\ndiscovery:\n  supported: true\n  spec: OpenID Connect Discovery 1.0\n  well_known_path: /.well-known/openid-configuration\n  note: >-\n    Discovery is per-pod. The document returned also advertises the scopes the pod supports.\n  probed:\n    url: https://diaspora.social/.well-known/openid-configuration\n    status: 200\n    file: well-known/diaspora-openid-configuration.json\n\ndynamic_client_registration:\n  supported: true\n  spec: OpenID Connect Dynamic Client Registration 1.0\n  registration_endpoint_path:\
  \ /api/openid_connect/clients\n  method: POST\n  minimal_request_fields:\n  - client_name\n  - redirect_uris\n  returns:\n  - client_id\n  - client_secret\n  rationale: >-\n    Decentralization: an application cannot be manually pre-registered on every pod in the\n    network, so it registers itself on first contact with an unknown pod.\n\nflows:\n- id: authorization_code\n  name: Authorization Code Flow\n  spec: http://openid.net/specs/openid-connect-core-1_0.html#CodeFlowAuth\n  typical_client: Native client applications\n  description: >-\n    After authorization the client receives an authorization code and exchanges it for an access\n    token at the token endpoint.\n- id: implicit\n  name: Implicit Flow\n  spec: http://openid.net/specs/openid-connect-core-1_0.html#ImplicitFlowAuth\n  typical_client: Browser-based applications\n  description: >-\n    After authorization the access token is returned directly to the redirect endpoint via the\n    user agent.\n\nendpoints:\n  note: >-\n\
  \    Paths are identical on every pod; only the host varies. The values below are the live values\n    discovered on the diaspora.social pod.\n  authorization_endpoint: https://diaspora.social/api/openid_connect/authorizations/new\n  token_endpoint: https://diaspora.social/api/openid_connect/access_tokens\n  userinfo_endpoint: https://diaspora.social/api/openid_connect/user_info\n  registration_endpoint: https://diaspora.social/api/openid_connect/clients\n  jwks_uri: https://diaspora.social/api/openid_connect/jwks.json\n\ntoken_endpoint_auth_methods_supported:\n- client_secret_basic\n- client_secret_post\n- private_key_jwt\n\nid_token_signing_alg_values_supported:\n- RS256\n\nsubject_types_supported:\n- public\n- pairwise\n\nclaims_supported:\n- sub\n- name\n- nickname\n- profile\n- picture\n\ntoken_transmission:\n- style: header\n  example: 'Authorization: Bearer <access token>'\n  preferred: true\n- style: query_parameter\n  example: https://example.com/api/v0/example?access_token=<access\
  \ token>\n- style: form_parameter\n  content_type: application/x-www-form-urlencoded\n  example: access_token=<access token>\n\nerrors:\n- status: 401\n  meaning: >-\n    No token or an invalid token was supplied. All API endpoints require authentication.\n- status: 403\n  meaning: >-\n    The client tried to access an endpoint whose OAuth scope was not part of the authorization\n    grant.\n\nrelated:\n  scopes: scopes/diaspora-scopes.yml\n  conventions: conventions/diaspora-conventions.yml\n  well_known: well-known/diaspora-well-known.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/diaspora/refs/heads/main/authentication/diaspora-authentication.yml
summary_line: openIdConnect · 1 scheme
tags:
- Company
- Social
- Social Networking
- Decentralized
- Federated
- Open Source
- Privacy
- Fediverse
- Messaging
- OpenID Connect
---
