---
anonymous_access: false
api_key_in: []
api_specs:
- filename: optimly-ai-api-keys-api-openapi.yml
  format: yaml
  label: Optimly Api Keys API
  slug: optimly-ai-api-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/optimly-ai/openapi/optimly-ai-api-keys-api-openapi.yml
- filename: optimly-ai-attribution-api-openapi.yml
  format: yaml
  label: Optimly Attribution API
  slug: optimly-ai-attribution-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/optimly-ai/openapi/optimly-ai-attribution-api-openapi.yml
- filename: optimly-ai-brand-api-openapi.yml
  format: yaml
  label: Optimly Brand API
  slug: optimly-ai-brand-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/optimly-ai/openapi/optimly-ai-brand-api-openapi.yml
- filename: optimly-ai-brands-api-openapi.yml
  format: yaml
  label: Optimly Brands API
  slug: optimly-ai-brands-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/optimly-ai/openapi/optimly-ai-brands-api-openapi.yml
- filename: optimly-ai-feedback-api-openapi.yml
  format: yaml
  label: Optimly Feedback API
  slug: optimly-ai-feedback-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/optimly-ai/openapi/optimly-ai-feedback-api-openapi.yml
- filename: optimly-ai-healthz-api-openapi.yml
  format: yaml
  label: Optimly Healthz API
  slug: optimly-ai-healthz-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/optimly-ai/openapi/optimly-ai-healthz-api-openapi.yml
- filename: optimly-ai-internal-api-openapi.yml
  format: yaml
  label: Optimly Internal API
  slug: optimly-ai-internal-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/optimly-ai/openapi/optimly-ai-internal-api-openapi.yml
- filename: optimly-ai-marketing-api-openapi.yml
  format: yaml
  label: Optimly Marketing API
  slug: optimly-ai-marketing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/optimly-ai/openapi/optimly-ai-marketing-api-openapi.yml
- filename: optimly-ai-marketing-preferences-api-openapi.yml
  format: yaml
  label: Optimly Marketing Preferences API
  slug: optimly-ai-marketing-preferences-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/optimly-ai/openapi/optimly-ai-marketing-preferences-api-openapi.yml
- filename: optimly-ai-me-api-openapi.yml
  format: yaml
  label: Optimly Me API
  slug: optimly-ai-me-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/optimly-ai/openapi/optimly-ai-me-api-openapi.yml
- filename: optimly-ai-notification-preferences-api-openapi.yml
  format: yaml
  label: Optimly Notification Preferences API
  slug: optimly-ai-notification-preferences-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/optimly-ai/openapi/optimly-ai-notification-preferences-api-openapi.yml
- filename: optimly-ai-oauth-api-openapi.yml
  format: yaml
  label: Optimly OAuth API
  slug: optimly-ai-oauth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/optimly-ai/openapi/optimly-ai-oauth-api-openapi.yml
- filename: optimly-ai-onboarding-api-openapi.yml
  format: yaml
  label: Optimly Onboarding API
  slug: optimly-ai-onboarding-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/optimly-ai/openapi/optimly-ai-onboarding-api-openapi.yml
- filename: optimly-ai-optimly-api-openapi.yml
  format: yaml
  label: Optimly Optimly API
  slug: optimly-ai-optimly-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/optimly-ai/openapi/optimly-ai-optimly-api-openapi.yml
- filename: optimly-ai-public-api-openapi.yml
  format: yaml
  label: Optimly Public API
  slug: optimly-ai-public-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/optimly-ai/openapi/optimly-ai-public-api-openapi.yml
- filename: optimly-ai-readyz-api-openapi.yml
  format: yaml
  label: Optimly Readyz API
  slug: optimly-ai-readyz-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/optimly-ai/openapi/optimly-ai-readyz-api-openapi.yml
- filename: optimly-ai-recommendations-api-openapi.yml
  format: yaml
  label: Optimly Recommendations API
  slug: optimly-ai-recommendations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/optimly-ai/openapi/optimly-ai-recommendations-api-openapi.yml
- filename: optimly-ai-reports-api-openapi.yml
  format: yaml
  label: Optimly Reports API
  slug: optimly-ai-reports-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/optimly-ai/openapi/optimly-ai-reports-api-openapi.yml
- filename: optimly-ai-vault-api-openapi.yml
  format: yaml
  label: Optimly Vault API
  slug: optimly-ai-vault-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/optimly-ai/openapi/optimly-ai-vault-api-openapi.yml
- filename: optimly-ai-webhooks-api-openapi.yml
  format: yaml
  label: Optimly Webhooks API
  slug: optimly-ai-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/optimly-ai/openapi/optimly-ai-webhooks-api-openapi.yml
- filename: optimly-ai-well-known-api-openapi.yml
  format: yaml
  label: Optimly .well Known API
  slug: optimly-ai-well-known-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/optimly-ai/openapi/optimly-ai-well-known-api-openapi.yml
auth_types: []
description: Optimly MCP connector authentication
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Optimly Authentication
name_suffix: Authentication
oauth_flows: []
overview: Optimly declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Optimly
provider_slug: optimly-ai
scheme_count: 2
schemes:
- evidence: 'Authentication Authorization: Bearer — an organization sk_live_… key, a brand-scoped one, or an oat_ OAuth access token'
  header: Authorization
  how_to_obtain: Create a key in the application under Connections and use it as the Bearer token, or obtain an OAuth access token via the OAuth consent flow.
  location: header
  name: Bearer
  type: http-bearer
- authorize_url: https://app.optimly.ai/.well-known/oauth-authorization-server
  evidence: 'The connector discovers the flow on its own: an unauthenticated request answers 401 with a WWW-Authenticate header naming the resource metadata at https://app.optimly.ai/.well-known/oauth-protected-resource , which in turn advertises the authorization server at https://app.optimly.ai/.well-known/oauth-authorization-server . PKCE with S256 is required.'
  flows:
  - authorization_code
  header: Authorization
  how_to_obtain: Run `claude mcp login optimly` to complete the OAuth consent screen in the browser, which follows the discovered PKCE authorization code flow.
  location: header
  name: OAuth
  type: oauth2
slug: optimly-ai-authentication
source_filename: optimly-ai-authentication.yml
source_heading: Authentication Profile
source_url: https://optimly.ai/docs/mcp
source_yaml: "generated: '2026-11-20'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://optimly.ai/docs/mcp\nsources:\n- https://optimly.ai/docs/mcp\n- https://optimly.ai/docs/public-data\ndescription: Optimly MCP connector authentication\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: 'Authentication Authorization: Bearer — an organization sk_live_… key, a brand-scoped one, or an oat_ OAuth access token'\n  location: header\n  header: Authorization\n  how_to_obtain: Create a key in the application under Connections and use it as the Bearer token, or obtain an OAuth access token via the OAuth\n    consent flow.\n- type: oauth2\n  name: OAuth\n  evidence: 'The connector discovers the flow on its own: an unauthenticated request answers 401 with a WWW-Authenticate header naming the resource\n    metadata at https://app.optimly.ai/.well-known/oauth-protected-resource , which in turn advertises the authorization server at https://app.optimly.ai/.well-known/oauth-authorization-server\n\
  \    . PKCE with S256 is required.'\n  location: header\n  header: Authorization\n  flows:\n  - authorization_code\n  authorize_url: https://app.optimly.ai/.well-known/oauth-authorization-server\n  how_to_obtain: Run `claude mcp login optimly` to complete the OAuth consent screen in the browser, which follows the discovered PKCE authorization\n    code flow.\ndocs: https://optimly.ai/docs/mcp\n"
source_yaml_url: https://artifacts.apis.io/optimly-ai/authentication/optimly-ai-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Artificial Intelligence
- BrandIndex
- Data API
- Platform
---
