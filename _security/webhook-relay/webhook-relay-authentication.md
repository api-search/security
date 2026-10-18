---
anonymous_access: false
api_key_in: []
api_specs:
- filename: webhook-relay-buckets-api-openapi.yml
  format: yaml
  label: Webhook Relay Buckets API
  slug: webhook-relay-buckets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/webhook-relay/refs/heads/main/openapi/webhook-relay-buckets-api-openapi.yml
- filename: webhook-relay-domains-api-openapi.yml
  format: yaml
  label: Webhook Relay Domains API
  slug: webhook-relay-domains-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/webhook-relay/refs/heads/main/openapi/webhook-relay-domains-api-openapi.yml
- filename: webhook-relay-functions-api-openapi.yml
  format: yaml
  label: Webhook Relay Functions API
  slug: webhook-relay-functions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/webhook-relay/refs/heads/main/openapi/webhook-relay-functions-api-openapi.yml
- filename: webhook-relay-inputs-api-openapi.yml
  format: yaml
  label: Webhook Relay Inputs API
  slug: webhook-relay-inputs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/webhook-relay/refs/heads/main/openapi/webhook-relay-inputs-api-openapi.yml
- filename: webhook-relay-logs-api-openapi.yml
  format: yaml
  label: Webhook Relay Logs API
  slug: webhook-relay-logs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/webhook-relay/refs/heads/main/openapi/webhook-relay-logs-api-openapi.yml
- filename: webhook-relay-outputs-api-openapi.yml
  format: yaml
  label: Webhook Relay Outputs API
  slug: webhook-relay-outputs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/webhook-relay/refs/heads/main/openapi/webhook-relay-outputs-api-openapi.yml
- filename: webhook-relay-tokens-api-openapi.yml
  format: yaml
  label: Webhook Relay Tokens API
  slug: webhook-relay-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/webhook-relay/refs/heads/main/openapi/webhook-relay-tokens-api-openapi.yml
- filename: webhook-relay-tunnels-api-openapi.yml
  format: yaml
  label: Webhook Relay Tunnels API
  slug: webhook-relay-tunnels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/webhook-relay/refs/heads/main/openapi/webhook-relay-tunnels-api-openapi.yml
auth_types: []
description: Authentication schemes published on the referenced pages
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Webhook Relay Authentication
name_suffix: Authentication
oauth_flows: []
overview: Webhook Relay declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Webhook Relay
provider_slug: webhook-relay
scheme_count: 1
schemes:
- evidence: 'Most applications use a standard bearer token format when sending HTTP requests. This involves setting an Authorization header: Authorization : Bearer <token>'
  header: Authorization
  location: header
  name: JWT
  type: http-bearer
slug: webhook-relay-authentication
source_filename: webhook-relay-authentication.yml
source_heading: Authentication Profile
source_url: https://webhookrelay.com/docs/account/mfa/
source_yaml: "generated: '2026-10-13'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://webhookrelay.com/docs/account/mfa/\nsources:\n- https://webhookrelay.com/docs/account/mfa/\n- https://webhookrelay.com/docs/webhooks/auth/jwt/\n- https://webhookrelay.com/blog/webhook-authentication/\n- https://webhookrelay.com/docs/webhooks/auth/jwt/\ndescription: Authentication schemes published on the referenced pages\nschemes:\n- type: http-bearer\n  name: JWT\n  evidence: 'Most applications use a standard bearer token format when sending HTTP requests. This involves setting an Authorization header: Authorization\n    : Bearer <token>'\n  location: header\n  header: Authorization\ndocs: https://webhookrelay.com/docs/account/mfa/\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/webhook-relay/refs/heads/main/authentication/webhook-relay-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Webhook
- API Gateway
- Integration
- Developer Tools
---
