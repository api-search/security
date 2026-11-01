---
anonymous_access: false
api_key_in: []
api_specs:
- filename: mails-ai-account-api-openapi.yml
  format: yaml
  label: mails-ai Account API
  slug: mails-ai-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mails-ai/openapi/mails-ai-account-api-openapi.yml
- filename: mails-ai-agents-api-openapi.yml
  format: yaml
  label: mails-ai Agents API
  slug: mails-ai-agents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mails-ai/openapi/mails-ai-agents-api-openapi.yml
- filename: mails-ai-api-keys-api-openapi.yml
  format: yaml
  label: mails-ai API Keys API
  slug: mails-ai-api-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mails-ai/openapi/mails-ai-api-keys-api-openapi.yml
- filename: mails-ai-billing-api-openapi.yml
  format: yaml
  label: mails-ai Billing API
  slug: mails-ai-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mails-ai/openapi/mails-ai-billing-api-openapi.yml
- filename: mails-ai-connected-apps-api-openapi.yml
  format: yaml
  label: mails-ai Connected Apps API
  slug: mails-ai-connected-apps-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mails-ai/openapi/mails-ai-connected-apps-api-openapi.yml
- filename: mails-ai-domains-api-openapi.yml
  format: yaml
  label: mails-ai Domains API
  slug: mails-ai-domains-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mails-ai/openapi/mails-ai-domains-api-openapi.yml
- filename: mails-ai-drafts-api-openapi.yml
  format: yaml
  label: mails-ai Drafts API
  slug: mails-ai-drafts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mails-ai/openapi/mails-ai-drafts-api-openapi.yml
- filename: mails-ai-events-api-openapi.yml
  format: yaml
  label: mails-ai Events API
  slug: mails-ai-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mails-ai/openapi/mails-ai-events-api-openapi.yml
- filename: mails-ai-inbound-api-openapi.yml
  format: yaml
  label: mails-ai Inbound API
  slug: mails-ai-inbound-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mails-ai/openapi/mails-ai-inbound-api-openapi.yml
- filename: mails-ai-labels-api-openapi.yml
  format: yaml
  label: mails-ai Labels API
  slug: mails-ai-labels-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mails-ai/openapi/mails-ai-labels-api-openapi.yml
- filename: mails-ai-logs-api-openapi.yml
  format: yaml
  label: mails-ai Logs API
  slug: mails-ai-logs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mails-ai/openapi/mails-ai-logs-api-openapi.yml
- filename: mails-ai-messages-api-openapi.yml
  format: yaml
  label: mails-ai Messages API
  slug: mails-ai-messages-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mails-ai/openapi/mails-ai-messages-api-openapi.yml
- filename: mails-ai-metrics-api-openapi.yml
  format: yaml
  label: mails-ai Metrics API
  slug: mails-ai-metrics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mails-ai/openapi/mails-ai-metrics-api-openapi.yml
- filename: mails-ai-public-api-openapi.yml
  format: yaml
  label: mails-ai Public API
  slug: mails-ai-public-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mails-ai/openapi/mails-ai-public-api-openapi.yml
- filename: mails-ai-reputation-api-openapi.yml
  format: yaml
  label: mails-ai Reputation API
  slug: mails-ai-reputation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mails-ai/openapi/mails-ai-reputation-api-openapi.yml
- filename: mails-ai-search-api-openapi.yml
  format: yaml
  label: mails-ai Search API
  slug: mails-ai-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mails-ai/openapi/mails-ai-search-api-openapi.yml
- filename: mails-ai-suppression-api-openapi.yml
  format: yaml
  label: mails-ai Suppression API
  slug: mails-ai-suppression-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mails-ai/openapi/mails-ai-suppression-api-openapi.yml
- filename: mails-ai-threads-api-openapi.yml
  format: yaml
  label: mails-ai Threads API
  slug: mails-ai-threads-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mails-ai/openapi/mails-ai-threads-api-openapi.yml
- filename: mails-ai-webhooks-api-openapi.yml
  format: yaml
  label: mails-ai Webhooks API
  slug: mails-ai-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mails-ai/openapi/mails-ai-webhooks-api-openapi.yml
auth_types: []
description: Authentication — API keys, scopes, and the Bearer header
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Mails Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: mails-ai declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: mails-ai
provider_slug: mails-ai
scheme_count: 1
schemes:
- evidence: 'Every request to https://api.mails.ai authenticates with an API key in the standard bearer header: Authorization: Bearer mk_live_xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx'
  header: Authorization
  how_to_obtain: Sign in at app.mails.ai and mint a key under API keys, or create one programmatically using an existing key with the manage scope.
  location: header
  name: API Key
  type: apiKey
slug: mails-ai-authentication
source_filename: mails-ai-authentication.yml
source_heading: Authentication Profile
source_url: https://mails.ai/docs/authentication
source_yaml: "generated: '2026-10-31'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://mails.ai/docs/authentication\nsources:\n- https://mails.ai/docs/authentication\n- https://mails.ai/blog/email-oauth-token-management-ai-agents\n- https://mails.ai/docs/api-reference/api-keys/create-api-key\n- https://mails.ai/docs/api-reference/api-keys/list-api-keys\ndescription: Authentication — API keys, scopes, and the Bearer header\nschemes:\n- type: apiKey\n  name: API Key\n  evidence: 'Every request to https://api.mails.ai authenticates with an API key in the standard bearer header: Authorization: Bearer mk_live_xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx'\n  location: header\n  header: Authorization\n  how_to_obtain: Sign in at app.mails.ai and mint a key under API keys, or create one programmatically using an existing key with the manage scope.\ndocs: https://mails.ai/docs/authentication\n"
source_yaml_url: https://artifacts.apis.io/mails-ai/authentication/mails-ai-authentication.yml
summary_line: 1 scheme
tags:
- Company
- AI
- Email
- Infrastructure
- Agents
---
