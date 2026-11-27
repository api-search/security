---
anonymous_access: false
api_key_in: []
api_specs:
- filename: hyperresearch-ai-account-api-openapi.yml
  format: yaml
  label: Hyperresearch Account API
  slug: hyperresearch-ai-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hyperresearch-ai/openapi/hyperresearch-ai-account-api-openapi.yml
- filename: hyperresearch-ai-agent-connections-api-openapi.yml
  format: yaml
  label: Hyperresearch agent connections API
  slug: hyperresearch-ai-agent-connections-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hyperresearch-ai/openapi/hyperresearch-ai-agent-connections-api-openapi.yml
- filename: hyperresearch-ai-answers-api-openapi.yml
  format: yaml
  label: Hyperresearch Answers API
  slug: hyperresearch-ai-answers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hyperresearch-ai/openapi/hyperresearch-ai-answers-api-openapi.yml
- filename: hyperresearch-ai-auth-api-openapi.yml
  format: yaml
  label: Hyperresearch Auth API
  slug: hyperresearch-ai-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hyperresearch-ai/openapi/hyperresearch-ai-auth-api-openapi.yml
- filename: hyperresearch-ai-billing-api-openapi.yml
  format: yaml
  label: Hyperresearch Billing API
  slug: hyperresearch-ai-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hyperresearch-ai/openapi/hyperresearch-ai-billing-api-openapi.yml
- filename: hyperresearch-ai-demo-api-openapi.yml
  format: yaml
  label: Hyperresearch Demo API
  slug: hyperresearch-ai-demo-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hyperresearch-ai/openapi/hyperresearch-ai-demo-api-openapi.yml
- filename: hyperresearch-ai-keys-api-openapi.yml
  format: yaml
  label: Hyperresearch Keys API
  slug: hyperresearch-ai-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hyperresearch-ai/openapi/hyperresearch-ai-keys-api-openapi.yml
- filename: hyperresearch-ai-meta-api-openapi.yml
  format: yaml
  label: Hyperresearch Meta API
  slug: hyperresearch-ai-meta-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hyperresearch-ai/openapi/hyperresearch-ai-meta-api-openapi.yml
- filename: hyperresearch-ai-projects-api-openapi.yml
  format: yaml
  label: Hyperresearch Projects API
  slug: hyperresearch-ai-projects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hyperresearch-ai/openapi/hyperresearch-ai-projects-api-openapi.yml
- filename: hyperresearch-ai-runs-api-openapi.yml
  format: yaml
  label: Hyperresearch Runs API
  slug: hyperresearch-ai-runs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hyperresearch-ai/openapi/hyperresearch-ai-runs-api-openapi.yml
- filename: hyperresearch-ai-scholar-api-openapi.yml
  format: yaml
  label: Hyperresearch Scholar API
  slug: hyperresearch-ai-scholar-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hyperresearch-ai/openapi/hyperresearch-ai-scholar-api-openapi.yml
- filename: hyperresearch-ai-usage-api-openapi.yml
  format: yaml
  label: Hyperresearch Usage API
  slug: hyperresearch-ai-usage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hyperresearch-ai/openapi/hyperresearch-ai-usage-api-openapi.yml
- filename: hyperresearch-ai-vault-api-openapi.yml
  format: yaml
  label: Hyperresearch Vault API
  slug: hyperresearch-ai-vault-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hyperresearch-ai/openapi/hyperresearch-ai-vault-api-openapi.yml
- filename: hyperresearch-ai-verify-api-openapi.yml
  format: yaml
  label: Hyperresearch Verify API
  slug: hyperresearch-ai-verify-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hyperresearch-ai/openapi/hyperresearch-ai-verify-api-openapi.yml
- filename: hyperresearch-ai-webhooks-api-openapi.yml
  format: yaml
  label: Hyperresearch Webhooks API
  slug: hyperresearch-ai-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hyperresearch-ai/openapi/hyperresearch-ai-webhooks-api-openapi.yml
- filename: hyperresearch-ai-workspaces-api-openapi.yml
  format: yaml
  label: Hyperresearch Workspaces API
  slug: hyperresearch-ai-workspaces-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/hyperresearch-ai/openapi/hyperresearch-ai-workspaces-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Hyperresearch Authentication
name_suffix: Authentication
oauth_flows: []
overview: Hyperresearch declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Hyperresearch
provider_slug: hyperresearch-ai
scheme_count: 2
schemes:
- evidence: Bearer keys are shown once. Grant only the scopes an integration needs, rotate them from the console, and never place them in browser URLs.
  header: Authorization
  how_to_obtain: Create an API key via the API or console; the secret is returned once and used as a Bearer token.
  location: header
  name: API Key
  type: http-bearer
- evidence: Signing in to the console creates an HttpOnly session.
  how_to_obtain: Sign in to the Hyperresearch console to receive an HttpOnly session cookie.
  location: cookie
  name: Session cookie
  type: other
slug: hyperresearch-ai-authentication
source_filename: hyperresearch-ai-authentication.yml
source_heading: Authentication Profile
source_url: https://hyperresearch.ai/docs/authentication
source_yaml: "generated: '2026-11-12'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://hyperresearch.ai/docs/authentication\nsources:\n- https://hyperresearch.ai/docs/authentication\n- https://hyperresearch.ai/docs/authentication\n- https://hyperresearch.ai/docs/api/operations/listapikeys\n- https://hyperresearch.ai/docs/api/operations/createapikey\nschemes:\n- type: http-bearer\n  name: API Key\n  evidence: Bearer keys are shown once. Grant only the scopes an integration needs, rotate them from the console, and never place them in browser\n    URLs.\n  location: header\n  header: Authorization\n  how_to_obtain: Create an API key via the API or console; the secret is returned once and used as a Bearer token.\n- type: other\n  name: Session cookie\n  evidence: Signing in to the console creates an HttpOnly session.\n  location: cookie\n  how_to_obtain: Sign in to the Hyperresearch console to receive an HttpOnly session cookie.\ndocs: https://hyperresearch.ai/docs/authentication\n"
source_yaml_url: https://artifacts.apis.io/hyperresearch-ai/authentication/hyperresearch-ai-authentication.yml
summary_line: 2 schemes
tags:
- Artificial Intelligence
- Search
- Research
- Data
---
