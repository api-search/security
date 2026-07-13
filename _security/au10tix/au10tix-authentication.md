---
api_key_in:
- header
api_specs:
- filename: au10tix-openapi.yml
  format: yaml
  label: AU10TIX Identity Verification API
  slug: au10tix-identity-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/au10tix/refs/heads/main/openapi/au10tix-openapi.yml
- filename: au10tix-openapi.yml
  format: yaml
  label: AU10TIX Document Authentication API
  slug: au10tix-document-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/au10tix/refs/heads/main/openapi/au10tix-openapi.yml
- filename: au10tix-openapi.yml
  format: yaml
  label: AU10TIX Face Comparison & Liveness API
  slug: au10tix-face-liveness-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/au10tix/refs/heads/main/openapi/au10tix-openapi.yml
- filename: au10tix-openapi.yml
  format: yaml
  label: AU10TIX Results API
  slug: au10tix-results-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/au10tix/refs/heads/main/openapi/au10tix-openapi.yml
- filename: au10tix-openapi.yml
  format: yaml
  label: AU10TIX Webhooks API
  slug: au10tix-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/au10tix/refs/heads/main/openapi/au10tix-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
method: derived
name: Au10Tix Authentication
name_suffix: Authentication
oauth_flows: []
overview: AU10TIX secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: AU10TIX
provider_slug: au10tix
scheme_count: 2
schemes:
- bearerFormat: JWT
  description: OAuth2 access token (JWT) presented as a Bearer token in the Authorization header on each request to the current BOS REST API.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/au10tix-openapi.yml
  type: http
- description: Legacy BOS integrations are secured by certificate-based authentication (mutual TLS); AU10TIX issues a unique client certificate to each calling party. Represented here as a security scheme placeholder because mutual TLS is configured at the transport layer rather than in a request header.
  in: header
  name: clientCertificate
  parameter: X-Client-Certificate
  sources:
  - openapi/au10tix-openapi.yml
  type: apiKey
slug: au10tix-authentication
source_filename: au10tix-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/au10tix-openapi.yml\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - header\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: OAuth2 access token (JWT) presented as a Bearer token in the Authorization header\n    on each request to the current BOS REST API.\n  sources:\n  - openapi/au10tix-openapi.yml\n- name: clientCertificate\n  type: apiKey\n  in: header\n  parameter: X-Client-Certificate\n  description: Legacy BOS integrations are secured by certificate-based authentication (mutual\n    TLS); AU10TIX issues a unique client certificate to each calling party. Represented here\n    as a security scheme placeholder because mutual TLS is configured at the transport layer\n    rather than in a request header.\n  sources:\n  - openapi/au10tix-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/au10tix/refs/heads/main/authentication/au10tix-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Identity Verification
- Document Authentication
- KYC
- Biometrics
- Fraud Detection
---
