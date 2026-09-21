---
anonymous_access: false
api_key_in: []
api_specs:
- filename: modal-labs-modal-web-endpoints-representative-api-openapi.yml
  format: yaml
  label: Modal Web Endpoints (Representative) API
  slug: modal-labs-modal-web-endpoints-representative-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/modal-labs/refs/heads/main/openapi/modal-labs-modal-web-endpoints-representative-api-openapi.yml
auth_types: []
description: Modal has THREE distinct authentication surfaces and they are easy to confuse. (1) The control plane — the gRPC API the SDKs and CLI speak — authenticates with a token id + token secret pair created by `modal token new` and stored in ~/.modal.toml. (2) Deployed web endpoints on *.modal.run authenticate INBOUND callers with Proxy Tokens presented as Modal-Key and Modal-Secret headers, enforced by Modal's edge proxy before the request reaches the container. (3) Modal signs OUTBOUND OIDC identity tokens so a running Function can prove who it is to an external service — Modal is the issuer there, not the verifier. There is no OAuth authorization-code flow and no user-facing OAuth scope surface, so scopes/ is deliberately absent.
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Modal Labs Authentication
name_suffix: Authentication
oauth_flows: []
overview: Modal declares 4 security scheme(s) across its OpenAPI definitions.
provider_name: Modal
provider_slug: modal-labs
scheme_count: 4
schemes:
- created_by: modal token new
  credential: token id + token secret
  docs: https://modal.com/docs/cli/latest/token
  env_vars:
  - MODAL_TOKEN_ID
  - MODAL_TOKEN_SECRET
  id: control-plane-token
  proto_evidence: token_id / token_secret fields on the client authentication messages in grpc/modal-labs-api.proto.
  rotation: Tokens are created and revoked via the CLI and the dashboard; multiple named profiles can hold separate token pairs.
  stored_at: ~/.modal.toml
  surface: gRPC control plane (api.modal.com)
  transport: gRPC request metadata
  type: apiKey
- client_helper: '`modal curl` calls an authenticated endpoint without hand-setting the headers.'
  credential: Proxy Token (key + secret)
  defaults:
  - authenticated_by_default: true
    opt_out: --unauthenticated on `modal endpoint create`, or unauthenticated=True on @app.server()
    surface: Endpoints and Servers
  - authenticated_by_default: false
    opt_in: requires_proxy_auth=True
    surface: Web Functions (@modal.fastapi_endpoint / asgi_app / wsgi_app / web_server)
  docs: https://modal.com/docs/guide/webhook-proxy-auth
  enforced_by: 'Modal''s edge proxy — an unauthenticated request is rejected with HTTP 401 and the body "modal-http: missing credentials for proxy authorization" before any user code runs.'
  headers:
  - Modal-Key
  - Modal-Secret
  id: proxy-token
  managed_by:
  - https://modal.com/settings/proxy-auth-tokens
  - modal workspace proxy-tokens
  surface: deployed web endpoints and Servers on *.modal.run
  transport: HTTP request headers
  type: apiKey
- algorithm: RS256
  audience: oidc.modal.com
  claims:
  - sub
  - aud
  - exp
  - iat
  - iss
  - jti
  - workspace_id
  - environment_id
  - environment_name
  - app_id
  - app_name
  - function_id
  - function_name
  - container_id
  delivery: Injected into the container as the MODAL_IDENTITY_TOKEN environment variable. Sandboxes must opt in with include_oidc_identity_token=True.
  direction: outbound
  discovery: https://oidc.modal.com/.well-known/openid-configuration
  docs: https://modal.com/docs/guide/oidc-integration
  id: oidc-workload-identity
  issuer: https://oidc.modal.com
  jwks: https://oidc.modal.com/.well-known/jwks.json
  scopes_supported:
  - openid
  surface: Modal Functions and Sandboxes authenticating to external services
  type: openIdConnect
- docs: https://modal.com/docs/guide/webhooks
  id: user-defined-endpoint-auth
  note: Documented pattern, not a Modal-enforced scheme — a developer validates a Bearer token in their own FastAPI handler against a value held in a modal.Secret. Recorded because the docs teach it, but the credential and its lifecycle belong to the developer, not to Modal.
  surface: inside a developer's own web endpoint
  type: http
slug: modal-labs-authentication
source_filename: modal-labs-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-18'\nmethod: searched\nsource: https://modal.com/docs/guide/webhook-proxy-auth + https://modal.com/docs/guide/webhooks + https://modal.com/docs/cli/latest/token + grpc/modal-labs-api.proto\nprovider: Modal\nproviderId: modal-labs\ndescription: >-\n  Modal has THREE distinct authentication surfaces and they are easy to confuse.\n  (1) The control plane — the gRPC API the SDKs and CLI speak — authenticates\n  with a token id + token secret pair created by `modal token new` and stored in\n  ~/.modal.toml. (2) Deployed web endpoints on *.modal.run authenticate INBOUND\n  callers with Proxy Tokens presented as Modal-Key and Modal-Secret headers,\n  enforced by Modal's edge proxy before the request reaches the container.\n  (3) Modal signs OUTBOUND OIDC identity tokens so a running Function can prove\n  who it is to an external service — Modal is the issuer there, not the verifier.\n  There is no OAuth authorization-code flow and no user-facing OAuth scope\n \
  \ surface, so scopes/ is deliberately absent.\nschemes:\n- id: control-plane-token\n  type: apiKey\n  surface: gRPC control plane (api.modal.com)\n  credential: token id + token secret\n  transport: gRPC request metadata\n  proto_evidence: >-\n    token_id / token_secret fields on the client authentication messages in\n    grpc/modal-labs-api.proto.\n  created_by: modal token new\n  stored_at: ~/.modal.toml\n  env_vars:\n  - MODAL_TOKEN_ID\n  - MODAL_TOKEN_SECRET\n  docs: https://modal.com/docs/cli/latest/token\n  rotation: >-\n    Tokens are created and revoked via the CLI and the dashboard; multiple named\n    profiles can hold separate token pairs.\n- id: proxy-token\n  type: apiKey\n  surface: deployed web endpoints and Servers on *.modal.run\n  credential: Proxy Token (key + secret)\n  transport: HTTP request headers\n  headers:\n  - Modal-Key\n  - Modal-Secret\n  enforced_by: >-\n    Modal's edge proxy — an unauthenticated request is rejected with HTTP 401 and\n    the body \"modal-http:\
  \ missing credentials for proxy authorization\" before any\n    user code runs.\n  defaults:\n  - surface: Endpoints and Servers\n    authenticated_by_default: true\n    opt_out: --unauthenticated on `modal endpoint create`, or unauthenticated=True on @app.server()\n  - surface: Web Functions (@modal.fastapi_endpoint / asgi_app / wsgi_app / web_server)\n    authenticated_by_default: false\n    opt_in: requires_proxy_auth=True\n  managed_by:\n  - https://modal.com/settings/proxy-auth-tokens\n  - modal workspace proxy-tokens\n  client_helper: >-\n    `modal curl` calls an authenticated endpoint without hand-setting the headers.\n  docs: https://modal.com/docs/guide/webhook-proxy-auth\n- id: oidc-workload-identity\n  type: openIdConnect\n  direction: outbound\n  surface: Modal Functions and Sandboxes authenticating to external services\n  discovery: https://oidc.modal.com/.well-known/openid-configuration\n  jwks: https://oidc.modal.com/.well-known/jwks.json\n  issuer: https://oidc.modal.com\n\
  \  audience: oidc.modal.com\n  algorithm: RS256\n  scopes_supported:\n  - openid\n  claims:\n  - sub\n  - aud\n  - exp\n  - iat\n  - iss\n  - jti\n  - workspace_id\n  - environment_id\n  - environment_name\n  - app_id\n  - app_name\n  - function_id\n  - function_name\n  - container_id\n  delivery: >-\n    Injected into the container as the MODAL_IDENTITY_TOKEN environment variable.\n    Sandboxes must opt in with include_oidc_identity_token=True.\n  docs: https://modal.com/docs/guide/oidc-integration\n- id: user-defined-endpoint-auth\n  type: http\n  surface: inside a developer's own web endpoint\n  note: >-\n    Documented pattern, not a Modal-enforced scheme — a developer validates a\n    Bearer token in their own FastAPI handler against a value held in a\n    modal.Secret. Recorded because the docs teach it, but the credential and its\n    lifecycle belong to the developer, not to Modal.\n  docs: https://modal.com/docs/guide/webhooks\nenterprise_identity:\n  sso:\n  - name: Okta SSO\n\
  \    url: https://modal.com/docs/guide/okta-sso\n  - name: Microsoft Entra SSO\n    url: https://modal.com/docs/guide/entra-sso\n  - name: Custom SAML SSO\n    url: https://modal.com/docs/guide/saml-sso\n  provisioning:\n    standard: SCIM 2.0\n    base_url_shape: https://modal.com/api/<your-workspace>/scim/v2\n    status: Beta\n    url: https://modal.com/docs/guide/scim\n  authorization:\n    model: RBAC\n    url: https://modal.com/docs/guide/rbac\n    note: >-\n      Roles are represented per Environment; service users and user groups are\n      separate first-class principals.\noauth_scopes: false\noauth_scopes_note: >-\n  No OAuth authorization server and no user-consent flow exist, so there is no\n  scope surface to document. scopes/ is intentionally not written — see the\n  \"scopes/ is OAuth-only\" rule in the pipeline contract.\nmaintainers:\n- FN: Kin Lane\n  email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/modal-labs/refs/heads/main/authentication/modal-labs-authentication.yml
summary_line: 4 schemes
tags:
- Serverless
- Compute
- GPU
- AI Infrastructure
- Sandbox
- Infrastructure as Code
---
