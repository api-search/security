---
api_key_in:
- cookie
api_specs:
- filename: solo-io-portal-server-openapi.yml
  format: yaml
  label: Gloo Portal Server API
  slug: portal-server
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/solo-io/refs/heads/main/openapi/solo-io-portal-server-openapi.yml
- filename: solo-io-portal-backend-openapi.yml
  format: yaml
  label: Gloo Portal Backend API
  slug: portal-backend
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/solo-io/refs/heads/main/openapi/solo-io-portal-backend-openapi.yml
- filename: solo-io-gloo-platform-portal-openapi.yml
  format: yaml
  label: Gloo Platform Portal API
  slug: gloo-platform-portal
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/solo-io/refs/heads/main/openapi/solo-io-gloo-platform-portal-openapi.yml
- filename: solo-io-portal-idp-connect-openapi.yml
  format: yaml
  label: Gloo Portal IdP Connect API
  slug: portal-idp-connect
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/solo-io/refs/heads/main/openapi/solo-io-portal-idp-connect-openapi.yml
- filename: solo-io-ai-gateway-guardrail-webhook-openapi.yml
  format: yaml
  label: AI Gateway Guardrail Webhook API
  slug: ai-guardrail-webhook
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/solo-io/refs/heads/main/openapi/solo-io-ai-gateway-guardrail-webhook-openapi.yml
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
- Model Context Protocol
- Developer Portal
- Cloud Native
- Open Source
---
