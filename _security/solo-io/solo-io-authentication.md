---
api_key_in:
- cookie
api_specs:
- filename: solo-io-api-keys-api-openapi.yml
  format: yaml
  label: Solo.io API Keys API
  slug: solo-io-api-keys-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/solo-io/refs/heads/main/openapi/solo-io-api-keys-api-openapi.yml
- filename: solo-io-api-products-api-openapi.yml
  format: yaml
  label: Solo.io API Products API
  slug: solo-io-api-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/solo-io/refs/heads/main/openapi/solo-io-api-products-api-openapi.yml
- filename: solo-io-apis-api-openapi.yml
  format: yaml
  label: Solo.io AP Is API
  slug: solo-io-apis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/solo-io/refs/heads/main/openapi/solo-io-apis-api-openapi.yml
- filename: solo-io-applications-api-openapi.yml
  format: yaml
  label: Solo.io Applications API
  slug: solo-io-applications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/solo-io/refs/heads/main/openapi/solo-io-applications-api-openapi.yml
- filename: solo-io-apps-api-openapi.yml
  format: yaml
  label: Solo.io Apps API
  slug: solo-io-apps-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/solo-io/refs/heads/main/openapi/solo-io-apps-api-openapi.yml
- filename: solo-io-auth-api-openapi.yml
  format: yaml
  label: Solo.io Auth API
  slug: solo-io-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/solo-io/refs/heads/main/openapi/solo-io-auth-api-openapi.yml
- filename: solo-io-health-api-openapi.yml
  format: yaml
  label: Solo.io Health API
  slug: solo-io-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/solo-io/refs/heads/main/openapi/solo-io-health-api-openapi.yml
- filename: solo-io-me-api-openapi.yml
  format: yaml
  label: Solo.io Me API
  slug: solo-io-me-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/solo-io/refs/heads/main/openapi/solo-io-me-api-openapi.yml
- filename: solo-io-metadata-api-openapi.yml
  format: yaml
  label: Solo.io Metadata API
  slug: solo-io-metadata-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/solo-io/refs/heads/main/openapi/solo-io-metadata-api-openapi.yml
- filename: solo-io-oauth-credentials-api-openapi.yml
  format: yaml
  label: Solo.io OAUTH Credentials API
  slug: solo-io-oauth-credentials-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/solo-io/refs/heads/main/openapi/solo-io-oauth-credentials-api-openapi.yml
- filename: solo-io-subscriptions-api-openapi.yml
  format: yaml
  label: Solo.io Subscriptions API
  slug: solo-io-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/solo-io/refs/heads/main/openapi/solo-io-subscriptions-api-openapi.yml
- filename: solo-io-teams-api-openapi.yml
  format: yaml
  label: Solo.io Teams API
  slug: solo-io-teams-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/solo-io/refs/heads/main/openapi/solo-io-teams-api-openapi.yml
- filename: solo-io-user-api-openapi.yml
  format: yaml
  label: Solo.io User API
  slug: solo-io-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/solo-io/refs/heads/main/openapi/solo-io-user-api-openapi.yml
- filename: solo-io-users-api-openapi.yml
  format: yaml
  label: Solo.io Users API
  slug: solo-io-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/solo-io/refs/heads/main/openapi/solo-io-users-api-openapi.yml
- filename: solo-io-webhooks-api-openapi.yml
  format: yaml
  label: Solo.io Webhooks API
  slug: solo-io-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/solo-io/refs/heads/main/openapi/solo-io-webhooks-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Solo Io Authentication
name_suffix: Authentication
oauth_flows: []
overview: Solo.io secures its APIs with apiKey and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Solo.io
provider_slug: solo-io
scheme_count: 3
schemes:
- description: id token cookie from the identity provider used to authenticate the user
  in: cookie
  name: identityToken
  parameter: id_token
  sources:
  - openapi/solo-io-gloo-platform-portal-openapi.yml
  - openapi/solo-io-portal-backend-openapi.yml
  - openapi/solo-io-portal-server-openapi.yml
  type: apiKey
- description: Bearer token passed in the Authorization header
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/solo-io-portal-backend-openapi.yml
  type: http
- description: access_token cookie set by the identity provider after OIDC login
  in: cookie
  name: accessToken
  parameter: access_token
  sources:
  - openapi/solo-io-portal-backend-openapi.yml
  type: apiKey
slug: solo-io-authentication
source_filename: solo-io-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: derived\nsource: openapi/solo-io-gloo-platform-portal-openapi.yml, openapi/solo-io-portal-backend-openapi.yml,\n  openapi/solo-io-portal-server-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - cookie\nschemes:\n- name: identityToken\n  type: apiKey\n  in: cookie\n  parameter: id_token\n  description: id token cookie from the identity provider used to authenticate the user\n  sources:\n  - openapi/solo-io-gloo-platform-portal-openapi.yml\n  - openapi/solo-io-portal-backend-openapi.yml\n  - openapi/solo-io-portal-server-openapi.yml\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: Bearer token passed in the Authorization header\n  sources:\n  - openapi/solo-io-portal-backend-openapi.yml\n- name: accessToken\n  type: apiKey\n  in: cookie\n  parameter: access_token\n  description: access_token cookie set by the identity provider after OIDC login\n  sources:\n  - openapi/solo-io-portal-backend-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/solo-io/refs/heads/main/authentication/solo-io-authentication.yml
summary_line: apiKey/http · 3 schemes
tags:
- Company
- API Gateway
- Service Mesh
- Kubernetes
- Istio
- Envoy
- AI Gateway
- Agentic AI
- MCP
- Developer Portal
- Cloud-Native
- Open-Source
---
