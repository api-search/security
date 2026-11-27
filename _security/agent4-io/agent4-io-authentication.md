---
anonymous_access: false
api_key_in: []
api_specs:
- filename: agent4-io-api-openapi.json
  format: json
  label: chatagent-platform Api API
  slug: chatagent-platform-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agent4-io/openapi/_original/agent4-io-api-openapi.json
auth_types: []
description: Authentication schemes for Agent4.io API
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Agent4.io Authentication
name_suffix: Authentication
oauth_flows: []
overview: Agent4.io declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: Agent4.io
provider_slug: agent4-io
scheme_count: 3
schemes:
- evidence: 'Acts as Tenant API key X-API-Key: tk_… (or Authorization: Bearer tk_… )'
  header: X-API-Key
  how_to_obtain: Your workspace's secret key for the platform API.
  location: header
  name: Tenant API key
  type: apiKey
- evidence: 'X-API-Key: tk_… + X-End-User: <your‑user‑id>'
  header: X-End-User
  how_to_obtain: Your backend holds the tenant key and asserts the end‑user identity per request.
  location: header
  name: Proxy‑mode end user
  type: apiKey
- evidence: 'Authorization: Bearer <jwt> An end user who signed in via /auth/login or OAuth'
  header: Authorization
  how_to_obtain: End user JWT issued after signing in via /auth/login or OAuth.
  location: header
  name: Platform end user JWT
  type: http-bearer
slug: agent4-io-authentication
source_filename: agent4-io-authentication.yml
source_heading: Authentication Profile
source_url: https://agent4.io/docs/api/authentication
source_yaml: "generated: '2026-11-01'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://agent4.io/docs/api/authentication\nsources:\n- https://agent4.io/docs/api/authentication\n- https://agent4.io/docs/tenant-guide/keys-and-tokens\n- https://agent4.io/docs/tenant-guide/token-usage\n- https://agent4.io/solutions/saas-onboarding\ndescription: Authentication schemes for Agent4.io API\nschemes:\n- type: apiKey\n  name: Tenant API key\n  evidence: 'Acts as Tenant API key X-API-Key: tk_… (or Authorization: Bearer tk_… )'\n  location: header\n  header: X-API-Key\n  how_to_obtain: Your workspace's secret key for the platform API.\n- type: apiKey\n  name: Proxy‑mode end user\n  evidence: 'X-API-Key: tk_… + X-End-User: <your‑user‑id>'\n  location: header\n  header: X-End-User\n  how_to_obtain: Your backend holds the tenant key and asserts the end‑user identity per request.\n- type: http-bearer\n  name: Platform end user JWT\n  evidence: 'Authorization: Bearer <jwt>\
  \ An end user who signed in via /auth/login or OAuth'\n  location: header\n  header: Authorization\n  how_to_obtain: End user JWT issued after signing in via /auth/login or OAuth.\nnote: No OAuth2 flows, JWT specific flow, or other schemes are documented on the referenced pages.\ndocs: https://agent4.io/docs/api/authentication\n"
source_yaml_url: https://artifacts.apis.io/agent4-io/authentication/agent4-io-authentication.yml
summary_line: 3 schemes
tags:
- Artificial Intelligence
- Automation
- Customer Engagement
- Software-as-a-Service
- Agent Platform
---
