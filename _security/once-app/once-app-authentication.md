---
anonymous_access: false
api_key_in: []
api_specs:
- filename: once-app-accounts-api-openapi.yml
  format: yaml
  label: ONCE Accounts API
  slug: once-app-accounts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/once-app/openapi/once-app-accounts-api-openapi.yml
- filename: once-app-agent-auth-api-openapi.yml
  format: yaml
  label: ONCE Agent Auth API
  slug: once-app-agent-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/once-app/openapi/once-app-agent-auth-api-openapi.yml
- filename: once-app-audio-api-openapi.yml
  format: yaml
  label: ONCE Audio API
  slug: once-app-audio-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/once-app/openapi/once-app-audio-api-openapi.yml
- filename: once-app-auth-api-openapi.yml
  format: yaml
  label: ONCE Auth API
  slug: once-app-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/once-app/openapi/once-app-auth-api-openapi.yml
- filename: once-app-cover-art-api-openapi.yml
  format: yaml
  label: ONCE Cover Art API
  slug: once-app-cover-art-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/once-app/openapi/once-app-cover-art-api-openapi.yml
- filename: once-app-credits-api-openapi.yml
  format: yaml
  label: ONCE Credits API
  slug: once-app-credits-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/once-app/openapi/once-app-credits-api-openapi.yml
- filename: once-app-distribution-stores-api-openapi.yml
  format: yaml
  label: ONCE Distribution Stores API
  slug: once-app-distribution-stores-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/once-app/openapi/once-app-distribution-stores-api-openapi.yml
- filename: once-app-drafts-api-openapi.yml
  format: yaml
  label: ONCE Drafts API
  slug: once-app-drafts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/once-app/openapi/once-app-drafts-api-openapi.yml
- filename: once-app-files-api-openapi.yml
  format: yaml
  label: ONCE Files API
  slug: once-app-files-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/once-app/openapi/once-app-files-api-openapi.yml
- filename: once-app-fraud-api-openapi.yml
  format: yaml
  label: ONCE Fraud API
  slug: once-app-fraud-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/once-app/openapi/once-app-fraud-api-openapi.yml
- filename: once-app-language-script-codes-api-openapi.yml
  format: yaml
  label: ONCE Language Script Codes API
  slug: once-app-language-script-codes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/once-app/openapi/once-app-language-script-codes-api-openapi.yml
- filename: once-app-me-api-openapi.yml
  format: yaml
  label: ONCE Me API
  slug: once-app-me-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/once-app/openapi/once-app-me-api-openapi.yml
- filename: once-app-metadata-rules-api-openapi.yml
  format: yaml
  label: ONCE Metadata Rules API
  slug: once-app-metadata-rules-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/once-app/openapi/once-app-metadata-rules-api-openapi.yml
- filename: once-app-once-rest-api-api-openapi.yml
  format: yaml
  label: ONCE ONCE REST API
  slug: once-app-once-rest-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/once-app/openapi/once-app-once-rest-api-api-openapi.yml
- filename: once-app-pricing-api-openapi.yml
  format: yaml
  label: ONCE Pricing API
  slug: once-app-pricing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/once-app/openapi/once-app-pricing-api-openapi.yml
- filename: once-app-release-schema-api-openapi.yml
  format: yaml
  label: ONCE Release Schema API
  slug: once-app-release-schema-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/once-app/openapi/once-app-release-schema-api-openapi.yml
- filename: once-app-releases-api-openapi.yml
  format: yaml
  label: ONCE Releases API
  slug: once-app-releases-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/once-app/openapi/once-app-releases-api-openapi.yml
- filename: once-app-status-api-openapi.yml
  format: yaml
  label: ONCE Status API
  slug: once-app-status-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/once-app/openapi/once-app-status-api-openapi.yml
- filename: once-app-uploads-api-openapi.yml
  format: yaml
  label: ONCE Uploads API
  slug: once-app-uploads-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/once-app/openapi/once-app-uploads-api-openapi.yml
- filename: once-app-webhooks-api-openapi.yml
  format: yaml
  label: ONCE Webhooks API
  slug: once-app-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/once-app/openapi/once-app-webhooks-api-openapi.yml
auth_types: []
description: Authentication – REST API – ONCE Docs
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: ONCE Authentication
name_suffix: Authentication
oauth_flows: []
overview: ONCE declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: ONCE
provider_slug: once-app
scheme_count: 2
schemes:
- evidence: 'Every request (except a few public discovery endpoints) requires an OAuth 2.1 access token with scope once:mcp , sent as a bearer token: Authorization: Bearer <access_token>'
  header: Authorization
  how_to_obtain: 'Personal Access Token: create one from your ONCE account in seconds.'
  location: header
  name: Bearer
  type: http-bearer
- authorize_url: https://beta.once.app/oauth/authorize
  evidence: 'For interactive apps, use the standard OAuth 2.1 authorization-code flow with PKCE:'
  flows:
  - authorization_code
  how_to_obtain: Send the user to https://beta.once.app/oauth/authorize with response_type=code, client_id, redirect_uri, scope=once:mcp, and code_challenge; then exchange the code at POST /v1/auth/token with the matching code_verifier.
  name: OAuth 2.1 Browser flow (PKCE)
  scopes:
  - once:mcp
  token_url: https://once.app/v1/auth/token
  type: oauth2
slug: once-app-authentication
source_filename: once-app-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.once.app/rest-api/authentication
source_yaml: "generated: '2026-11-19'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.once.app/rest-api/authentication\nsources:\n- https://docs.once.app/rest-api/authentication\n- https://docs.once.app/user-guide/getting-started\n- https://docs.once.app/mcp/agents\ndescription: Authentication – REST API – ONCE Docs\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: 'Every request (except a few public discovery endpoints) requires an OAuth 2.1 access token with scope once:mcp , sent as a bearer\n    token: Authorization: Bearer <access_token>'\n  location: header\n  header: Authorization\n  how_to_obtain: 'Personal Access Token: create one from your ONCE account in seconds.'\n- type: oauth2\n  name: OAuth 2.1 Browser flow (PKCE)\n  evidence: 'For interactive apps, use the standard OAuth 2.1 authorization-code flow with PKCE:'\n  flows:\n  - authorization_code\n  token_url: https://once.app/v1/auth/token\n  authorize_url: https://beta.once.app/oauth/authorize\n\
  \  scopes:\n  - once:mcp\n  how_to_obtain: Send the user to https://beta.once.app/oauth/authorize with response_type=code, client_id, redirect_uri, scope=once:mcp, and\n    code_challenge; then exchange the code at POST /v1/auth/token with the matching code_verifier.\ndocs: https://docs.once.app/rest-api/authentication\nnote: 1 extracted row(s) were dropped because their quote was not on the page.\n"
source_yaml_url: https://artifacts.apis.io/once-app/authentication/once-app-authentication.yml
summary_line: 2 schemes
tags:
- Music
- Distribution
- Platform
- Artists
- Artificial Intelligence
---
