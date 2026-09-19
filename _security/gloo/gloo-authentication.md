---
anonymous_access: true
api_key_in:
- cookie
api_specs:
- filename: gloo-api-products-api-openapi.yml
  format: yaml
  label: Gloo API Products API
  slug: gloo-api-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gloo/refs/heads/main/openapi/gloo-api-products-api-openapi.yml
- filename: gloo-applications-api-openapi.yml
  format: yaml
  label: Gloo Applications API
  slug: gloo-applications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gloo/refs/heads/main/openapi/gloo-applications-api-openapi.yml
- filename: gloo-me-api-openapi.yml
  format: yaml
  label: Gloo Me API
  slug: gloo-me-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gloo/refs/heads/main/openapi/gloo-me-api-openapi.yml
- filename: gloo-subscriptions-api-openapi.yml
  format: yaml
  label: Gloo Subscriptions API
  slug: gloo-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gloo/refs/heads/main/openapi/gloo-subscriptions-api-openapi.yml
- filename: gloo-teams-api-openapi.yml
  format: yaml
  label: Gloo Teams API
  slug: gloo-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gloo/refs/heads/main/openapi/gloo-teams-api-openapi.yml
- filename: gloo-user-api-openapi.yml
  format: yaml
  label: Gloo User API
  slug: gloo-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gloo/refs/heads/main/openapi/gloo-user-api-openapi.yml
- filename: gloo-webhooks-api-openapi.yml
  format: yaml
  label: Gloo Webhooks API
  slug: gloo-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gloo/refs/heads/main/openapi/gloo-webhooks-api-openapi.yml
- filename: gloo-apis-api-openapi.yml
  format: yaml
  label: Gloo AP Is API
  slug: gloo-apis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gloo/refs/heads/main/openapi/gloo-apis-api-openapi.yml
auth_types:
- apiKey
description: 'Gloo''s callable HTTP surface is the Gloo Portal server API (and its Gloo Platform predecessor). Both authenticate the CALLER as a developer-portal end user with an OIDC id token carried in a cookie — they do NOT use a bearer API key of their own. The API keys and OAuth client credentials these endpoints mint are credentials for the APIs the portal fronts, not for the portal API itself. The Gloo Portal IdP Connect API and the AI Gateway guardrail webhook publish no securityScheme at all: IdP Connect takes an optional `token` header naming the originating user and is expected to run inside the cluster, and the guardrail webhook is an endpoint the operator implements and protects themselves.'
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Gloo Authentication
name_suffix: Authentication
oauth_flows: []
overview: Gloo secures its APIs with apiKey across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Gloo
provider_slug: gloo
scheme_count: 3
schemes:
- applies_to:
  - gloo:gloo-portal
  - gloo:gloo-mesh
  description: id token cookie from the identity provider used to authenticate the user
  failure_modes:
  - meaning: The user's identity token is invalid.
    status: 401
  - meaning: The identity token is valid but the user is missing claims or permission for this operation.
    status: 403
  in: cookie
  name: identityToken
  parameter: id_token
  sources:
  - openapi/gloo-portal-server-openapi.yaml
  - openapi/gloo-platform-portal-openapi.yaml
  type: apiKey
- applies_to:
  - gloo:gloo-portal
  description: Token of origin user invoking the request. Declared as an optional header parameter on both Gloo Portal IdP Connect operations rather than as a securityScheme.
  in: header
  name: token
  parameter: token
  sources:
  - openapi/gloo-portal-idp-connect-openapi.yaml
  type: header
- applies_to:
  - gloo:gloo-gateway
  description: The AI Gateway guardrail webhook contract declares no security scheme. It describes an endpoint the OPERATOR stands up and that kgateway / agentgateway / Gloo Gateway calls; protecting it is the operator's responsibility.
  name: none
  sources:
  - openapi/gloo-ai-gateway-guardrail-webhook-openapi.yaml
  type: none
slug: gloo-authentication
source_filename: gloo-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-12'\nmethod: searched\nsource: >-\n  Derived from openapi/gloo-portal-server-openapi.yaml and\n  openapi/gloo-platform-portal-openapi.yaml, then upgraded from the Solo.io credential\n  management documentation at\n  https://docs.solo.io/gateway/latest/portal/guides/frontend-portal/credential-management/\ndocs: https://docs.solo.io/gateway/latest/portal/guides/frontend-portal/credential-management/\nprovider: Gloo\nproviderId: gloo\ndescription: >-\n  Gloo's callable HTTP surface is the Gloo Portal server API (and its Gloo Platform\n  predecessor). Both authenticate the CALLER as a developer-portal end user with an OIDC id\n  token carried in a cookie — they do NOT use a bearer API key of their own. The API keys and\n  OAuth client credentials these endpoints mint are credentials for the APIs the portal\n  fronts, not for the portal API itself. The Gloo Portal IdP Connect API and the AI Gateway\n  guardrail webhook publish no securityScheme at all: IdP Connect\
  \ takes an optional `token`\n  header naming the originating user and is expected to run inside the cluster, and the\n  guardrail webhook is an endpoint the operator implements and protects themselves.\nsummary:\n  types:\n    - apiKey\n  api_key_in:\n    - cookie\n  oauth2: false\n  openid_connect: true\n  openid_connect_note: >-\n    OIDC is the real identity mechanism, but it is configured on the gateway (extauth /\n    OIDC policy) rather than declared as an openIdConnect securityScheme in the spec. The\n    spec only sees its output: the id_token cookie.\n  mutual_tls: false\n  unauthenticated_operations: true\n  unauthenticated_note: >-\n    Several Portal operations declare `security: [{identityToken: []}, {}]` — an explicit\n    empty requirement — because a portal can be configured for public, anonymous browsing of\n    its API catalog. GetCurrentUser, ListAPIs, GetApiSchema and GetUsagePlans all allow it.\nschemes:\n  - name: identityToken\n    type: apiKey\n    in: cookie\n\
  \    parameter: id_token\n    description: id token cookie from the identity provider used to authenticate the user\n    sources:\n      - openapi/gloo-portal-server-openapi.yaml\n      - openapi/gloo-platform-portal-openapi.yaml\n    applies_to:\n      - gloo:gloo-portal\n      - gloo:gloo-mesh\n    failure_modes:\n      - status: 401\n        meaning: The user's identity token is invalid.\n      - status: 403\n        meaning: The identity token is valid but the user is missing claims or permission for this operation.\n  - name: token\n    type: header\n    in: header\n    parameter: token\n    description: >-\n      Token of origin user invoking the request. Declared as an optional header parameter on\n      both Gloo Portal IdP Connect operations rather than as a securityScheme.\n    sources:\n      - openapi/gloo-portal-idp-connect-openapi.yaml\n    applies_to:\n      - gloo:gloo-portal\n  - name: none\n    type: none\n    description: >-\n      The AI Gateway guardrail webhook contract\
  \ declares no security scheme. It describes an\n      endpoint the OPERATOR stands up and that kgateway / agentgateway / Gloo Gateway calls;\n      protecting it is the operator's responsibility.\n    sources:\n      - openapi/gloo-ai-gateway-guardrail-webhook-openapi.yaml\n    applies_to:\n      - gloo:gloo-gateway\ncredentials_minted_by_the_api:\n  - kind: API key\n    operations:\n      - CreateApplicationAPIKey\n      - ListApplicationAPIKeys\n      - DeleteAPIKey\n    note: >-\n      The plaintext key is returned only once, at creation. The APIKey schema says so\n      explicitly (\"Is returned only once when the API key is created\"). There is no\n      retrieve-key-again operation; a lost key must be deleted and re-issued.\n  - kind: OAuth2 client credentials\n    operations:\n      - GenerateApplicationOAuthCredential\n      - GetApplicationOAuthCredential\n      - DeleteOAuthCredential\n      - CreateOAuthApplication\n      - DeleteOAuthApplication\n    note: >-\n      Client\
  \ secrets are shown once at creation and are NOT stored in the Portal database —\n      Solo's own spec says an administrator must retrieve a lost secret from the OIDC provider.\n      CreateOAuthApplication / DeleteOAuthApplication live in the separate IdP Connect service.\ndocs_pages:\n  - url: https://docs.solo.io/gateway/latest/portal/guides/frontend-portal/credential-management/\n    status: 200\n    covers: API key and OAuth credential management for portal consumers\n  - url: https://docs.solo.io/gateway/latest/portal/guides/frontend-portal/credential-management/oauth/\n    status: 200\n    covers: OAuth credential provisioning through Gloo Portal IdP Connect\n  - url: https://docs.solo.io/gateway/latest/security/\n    status: 200\n    covers: Gateway-level authentication and authorization policy (OIDC, JWT, ext-auth, API key)\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gloo/refs/heads/main/authentication/gloo-authentication.yml
summary_line: apiKey · 3 schemes
tags:
- API Gateway
- Cloud-Native
- Developer Portal
- Envoy
- Istio
- Kubernetes
- Kubernetes Gateway API
- Open-Source
- Service Mesh
---
