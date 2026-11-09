---
anonymous_access: false
api_key_in: []
api_specs:
- filename: autoposting-ai-agents-api-openapi.yml
  format: yaml
  label: Autoposting.ai Agents API
  slug: autoposting-ai-agents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/autoposting-ai/openapi/autoposting-ai-agents-api-openapi.yml
- filename: autoposting-ai-api-keys-api-openapi.yml
  format: yaml
  label: Autoposting.ai API Keys API
  slug: autoposting-ai-api-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/autoposting-ai/openapi/autoposting-ai-api-keys-api-openapi.yml
- filename: autoposting-ai-auth-api-openapi.yml
  format: yaml
  label: Autoposting.ai Auth API
  slug: autoposting-ai-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/autoposting-ai/openapi/autoposting-ai-auth-api-openapi.yml
- filename: autoposting-ai-billing-api-openapi.yml
  format: yaml
  label: Autoposting.ai Billing API
  slug: autoposting-ai-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/autoposting-ai/openapi/autoposting-ai-billing-api-openapi.yml
- filename: autoposting-ai-brands-api-openapi.yml
  format: yaml
  label: Autoposting.ai Brands API
  slug: autoposting-ai-brands-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/autoposting-ai/openapi/autoposting-ai-brands-api-openapi.yml
- filename: autoposting-ai-carousels-api-openapi.yml
  format: yaml
  label: Autoposting.ai Carousels API
  slug: autoposting-ai-carousels-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/autoposting-ai/openapi/autoposting-ai-carousels-api-openapi.yml
- filename: autoposting-ai-clips-api-openapi.yml
  format: yaml
  label: Autoposting.ai Clips API
  slug: autoposting-ai-clips-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/autoposting-ai/openapi/autoposting-ai-clips-api-openapi.yml
- filename: autoposting-ai-knowledge-base-api-openapi.yml
  format: yaml
  label: Autoposting.ai Knowledge Base API
  slug: autoposting-ai-knowledge-base-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/autoposting-ai/openapi/autoposting-ai-knowledge-base-api-openapi.yml
- filename: autoposting-ai-notifications-api-openapi.yml
  format: yaml
  label: Autoposting.ai Notifications API
  slug: autoposting-ai-notifications-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/autoposting-ai/openapi/autoposting-ai-notifications-api-openapi.yml
- filename: autoposting-ai-organizations-api-openapi.yml
  format: yaml
  label: Autoposting.ai Organizations API
  slug: autoposting-ai-organizations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/autoposting-ai/openapi/autoposting-ai-organizations-api-openapi.yml
- filename: autoposting-ai-platform-oauth-api-openapi.yml
  format: yaml
  label: Autoposting.ai Platform OAuth API
  slug: autoposting-ai-platform-oauth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/autoposting-ai/openapi/autoposting-ai-platform-oauth-api-openapi.yml
- filename: autoposting-ai-posts-api-openapi.yml
  format: yaml
  label: Autoposting.ai Posts API
  slug: autoposting-ai-posts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/autoposting-ai/openapi/autoposting-ai-posts-api-openapi.yml
- filename: autoposting-ai-teams-api-openapi.yml
  format: yaml
  label: Autoposting.ai Teams API
  slug: autoposting-ai-teams-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/autoposting-ai/openapi/autoposting-ai-teams-api-openapi.yml
- filename: autoposting-ai-usage-api-openapi.yml
  format: yaml
  label: Autoposting.ai Usage API
  slug: autoposting-ai-usage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/autoposting-ai/openapi/autoposting-ai-usage-api-openapi.yml
- filename: autoposting-ai-webhooks-api-openapi.yml
  format: yaml
  label: Autoposting.ai Webhooks API
  slug: autoposting-ai-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/autoposting-ai/openapi/autoposting-ai-webhooks-api-openapi.yml
auth_types: []
description: Authentication methods supported by Autoposting.ai
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Autoposting Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Autoposting.ai declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: Autoposting.ai
provider_slug: autoposting-ai
scheme_count: 3
schemes:
- evidence: Bearer Token API Key CLI Login Issued on login. Carries full user-level permissions within the organization — suited for frontend apps and dashboard interactions.
  header: Authorization
  how_to_obtain: Obtain by POSTing email and password to https://app.autoposting.ai/api-proxy/auth/login and using the returned token.
  location: header
  name: Bearer Token
  type: http-bearer
- evidence: 'Org-scoped keys with declared permission scopes. Accepted via Authorization: Bearer or x-api-key header — recommended for all programmatic access.'
  header: Authorization
  how_to_obtain: Create a key via POST https://app.autoposting.ai/api-proxy/api-keys using an active session token.
  location: header
  name: API Key
  scopes:
  - posts:read
  - posts:write
  - brands:read
  - brands:write
  - clips:read
  - clips:write
  - carousels:read
  - carousels:write
  - kb:read
  - kb:write
  - agents:read
  - agents:write
  - webhooks:read
  - webhooks:write
  type: apiKey
- evidence: '# x-api-key header (alternative)'
  header: x-api-key
  location: header
  name: API Key (alternative header)
  type: apiKey
slug: autoposting-ai-authentication
source_filename: autoposting-ai-authentication.yml
source_heading: Authentication Profile
source_url: https://autopostingai.mintlify.app/authentication
source_yaml: "generated: '2026-11-02'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://autopostingai.mintlify.app/authentication\nsources:\n- https://autopostingai.mintlify.app/authentication\n- https://docs.autoposting.ai/api-reference/api-keys/create-an-api-key\n- https://docs.autoposting.ai/api-reference/api-keys/list-api-keys\n- https://docs.autoposting.ai/api-reference/api-keys/revoke-an-api-key\ndescription: Authentication methods supported by Autoposting.ai\nschemes:\n- type: http-bearer\n  name: Bearer Token\n  evidence: Bearer Token API Key CLI Login Issued on login. Carries full user-level permissions within the organization — suited for frontend\n    apps and dashboard interactions.\n  location: header\n  header: Authorization\n  how_to_obtain: Obtain by POSTing email and password to https://app.autoposting.ai/api-proxy/auth/login and using the returned token.\n- type: apiKey\n  name: API Key\n  evidence: 'Org-scoped keys with declared permission\
  \ scopes. Accepted via Authorization: Bearer or x-api-key header — recommended for all programmatic\n    access.'\n  location: header\n  header: Authorization\n  scopes:\n  - posts:read\n  - posts:write\n  - brands:read\n  - brands:write\n  - clips:read\n  - clips:write\n  - carousels:read\n  - carousels:write\n  - kb:read\n  - kb:write\n  - agents:read\n  - agents:write\n  - webhooks:read\n  - webhooks:write\n  how_to_obtain: Create a key via POST https://app.autoposting.ai/api-proxy/api-keys using an active session token.\n- type: apiKey\n  name: API Key (alternative header)\n  evidence: '# x-api-key header (alternative)'\n  location: header\n  header: x-api-key\nnote: No OAuth2 flows are documented.\ndocs: https://autopostingai.mintlify.app/authentication\n"
source_yaml_url: https://artifacts.apis.io/autoposting-ai/authentication/autoposting-ai-authentication.yml
summary_line: 3 schemes
tags:
- Artificial Intelligence
- Social Media
- Automation
- Marketing
- Developer Tools
- Company
---
