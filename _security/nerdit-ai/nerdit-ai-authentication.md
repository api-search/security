---
anonymous_access: false
api_key_in: []
api_specs:
- filename: nerdit-ai-account-api-openapi.yml
  format: yaml
  label: Nerdit Account API
  slug: nerdit-ai-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nerdit-ai/openapi/nerdit-ai-account-api-openapi.yml
- filename: nerdit-ai-audit-api-openapi.yml
  format: yaml
  label: Nerdit Audit API
  slug: nerdit-ai-audit-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nerdit-ai/openapi/nerdit-ai-audit-api-openapi.yml
- filename: nerdit-ai-auth-api-openapi.yml
  format: yaml
  label: Nerdit Auth API
  slug: nerdit-ai-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nerdit-ai/openapi/nerdit-ai-auth-api-openapi.yml
- filename: nerdit-ai-billing-api-openapi.yml
  format: yaml
  label: Nerdit Billing API
  slug: nerdit-ai-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nerdit-ai/openapi/nerdit-ai-billing-api-openapi.yml
- filename: nerdit-ai-email-api-openapi.yml
  format: yaml
  label: Nerdit Email API
  slug: nerdit-ai-email-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nerdit-ai/openapi/nerdit-ai-email-api-openapi.yml
- filename: nerdit-ai-github-api-openapi.yml
  format: yaml
  label: Nerdit GitHub API
  slug: nerdit-ai-github-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nerdit-ai/openapi/nerdit-ai-github-api-openapi.yml
- filename: nerdit-ai-health-api-openapi.yml
  format: yaml
  label: Nerdit Health API
  slug: nerdit-ai-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nerdit-ai/openapi/nerdit-ai-health-api-openapi.yml
- filename: nerdit-ai-link-api-openapi.yml
  format: yaml
  label: Nerdit Link API
  slug: nerdit-ai-link-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nerdit-ai/openapi/nerdit-ai-link-api-openapi.yml
- filename: nerdit-ai-nodes-api-openapi.yml
  format: yaml
  label: Nerdit Nodes API
  slug: nerdit-ai-nodes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nerdit-ai/openapi/nerdit-ai-nodes-api-openapi.yml
- filename: nerdit-ai-oauth-api-openapi.yml
  format: yaml
  label: Nerdit OAuth API
  slug: nerdit-ai-oauth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nerdit-ai/openapi/nerdit-ai-oauth-api-openapi.yml
- filename: nerdit-ai-projects-api-openapi.yml
  format: yaml
  label: Nerdit Projects API
  slug: nerdit-ai-projects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nerdit-ai/openapi/nerdit-ai-projects-api-openapi.yml
- filename: nerdit-ai-replace-api-openapi.yml
  format: yaml
  label: Nerdit Replace API
  slug: nerdit-ai-replace-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nerdit-ai/openapi/nerdit-ai-replace-api-openapi.yml
- filename: nerdit-ai-security-api-openapi.yml
  format: yaml
  label: Nerdit Security API
  slug: nerdit-ai-security-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nerdit-ai/openapi/nerdit-ai-security-api-openapi.yml
auth_types: []
description: Clients authenticate to the Engine API using a bearer token that is stored in the service‑user configuration and sent in the HTTP Authorization header.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Nerdit Authentication
name_suffix: Authentication
oauth_flows: []
overview: Nerdit declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Nerdit
provider_slug: nerdit-ai
scheme_count: 1
schemes:
- evidence: Use encrypted transport for remote bearer tokens.
  header: Authorization
  how_to_obtain: Create a scoped token with the `nerdit token create` CLI command; the plaintext token is shown once and must be stored in the client configuration.
  location: header
  name: Engine token
  type: http-bearer
slug: nerdit-ai-authentication
source_filename: nerdit-ai-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.nerdit.ai/engine/security.md
source_yaml: "generated: '2026-11-19'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.nerdit.ai/engine/security.md\nsources:\n- https://docs.nerdit.ai/engine/security.md\n- https://docs.nerdit.ai/engine/api/auth/auth-check.md\n- https://docs.nerdit.ai/engine/api/tokens/list-tokens.md\n- https://docs.nerdit.ai/engine/api/tokens/create-token.md\ndescription: Clients authenticate to the Engine API using a bearer token that is stored in the service‑user configuration and sent in the HTTP\n  Authorization header.\nschemes:\n- type: http-bearer\n  name: Engine token\n  evidence: Use encrypted transport for remote bearer tokens.\n  location: header\n  header: Authorization\n  how_to_obtain: Create a scoped token with the `nerdit token create` CLI command; the plaintext token is shown once and must be stored in the\n    client configuration.\nnote: No OAuth flows, API key, or other authentication mechanisms are documented on the provided pages.\ndocs: https://docs.nerdit.ai/engine/security.md\n"
source_yaml_url: https://artifacts.apis.io/nerdit-ai/authentication/nerdit-ai-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Artificial Intelligence
- Cloud
- Platform
- SmallSoftware
- Developer Tools
---
