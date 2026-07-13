---
api_key_in: []
api_specs:
- filename: barndoor-openapi.yml
  format: yaml
  label: Barndoor Platform API
  slug: platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/barndoor/refs/heads/main/openapi/barndoor-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Barndoor Authentication
name_suffix: Authentication
oauth_flows: []
overview: Barndoor secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Barndoor
provider_slug: barndoor
scheme_count: 1
schemes:
- bearerFormat: JWT
  description: 'JWT token obtained through Auth0 OAuth 2.0 flow with PKCE.


    The token should be included in the Authorization header:

    `Authorization: Bearer <your-jwt-token>`


    Use the Barndoor SDK''s `loginInteractive()` function to obtain tokens automatically.'
  name: BearerAuth
  scheme: bearer
  sources:
  - openapi/barndoor-openapi.yml
  type: http
slug: barndoor-authentication
source_filename: barndoor-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-11'\nmethod: derived\nsource: openapi/barndoor-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: |-\n    JWT token obtained through Auth0 OAuth 2.0 flow with PKCE.\n\n    The token should be included in the Authorization header:\n    `Authorization: Bearer <your-jwt-token>`\n\n    Use the Barndoor SDK's `loginInteractive()` function to obtain tokens automatically.\n  sources:\n  - openapi/barndoor-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/barndoor/refs/heads/main/authentication/barndoor-authentication.yml
summary_line: http · 1 scheme
tags:
- AI Agents
- AI Governance
- Agentic AI
- MCP
- Model Context Protocol
- Policy Enforcement
- OAuth
- Identity
- Security
- Audit
- Control Plane
---
