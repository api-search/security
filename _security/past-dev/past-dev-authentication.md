---
anonymous_access: false
api_key_in: []
api_specs:
- filename: past-dev-audiences-api-openapi.yml
  format: yaml
  label: past-dev Audiences API
  slug: past-dev-audiences-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/past-dev/openapi/past-dev-audiences-api-openapi.yml
- filename: past-dev-debugging-api-openapi.yml
  format: yaml
  label: past-dev Debugging API
  slug: past-dev-debugging-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/past-dev/openapi/past-dev-debugging-api-openapi.yml
- filename: past-dev-identities-api-openapi.yml
  format: yaml
  label: past-dev Identities API
  slug: past-dev-identities-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/past-dev/openapi/past-dev-identities-api-openapi.yml
- filename: past-dev-ingestion-api-openapi.yml
  format: yaml
  label: past-dev Ingestion API
  slug: past-dev-ingestion-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/past-dev/openapi/past-dev-ingestion-api-openapi.yml
- filename: past-dev-management-api-openapi.yml
  format: yaml
  label: past-dev Management API
  slug: past-dev-management-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/past-dev/openapi/past-dev-management-api-openapi.yml
- filename: past-dev-recall-api-openapi.yml
  format: yaml
  label: past-dev Recall API
  slug: past-dev-recall-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/past-dev/openapi/past-dev-recall-api-openapi.yml
- filename: past-dev-webhooks-api-openapi.yml
  format: yaml
  label: past-dev Webhooks API
  slug: past-dev-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/past-dev/openapi/past-dev-webhooks-api-openapi.yml
auth_types: []
description: Authentication methods for past-dev Memory API
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Past Dev Authentication
name_suffix: Authentication
oauth_flows: []
overview: past-dev declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: past-dev
provider_slug: past-dev
scheme_count: 3
schemes:
- evidence: 'Authorization: Bearer $PAST_API_KEY'
  header: Authorization
  how_to_obtain: Created on the API keys screen of the console at https://app.past.dev or via POST /api/v1/projects/{slug}/keys
  location: header
  name: Project key
  type: http-bearer
- evidence: 'Authorization: Bearer $PAST_API_KEY'
  header: Authorization
  how_to_obtain: Created under Settings → Organization → Management key in the console by an Owner or Admin at https://app.past.dev
  location: header
  name: Management key
  type: http-bearer
- evidence: 'WWW-Authenticate: Bearer resource_metadata="https://app.past.dev/.well-known/oauth-protected-resource/api/v1"'
  header: Authorization
  how_to_obtain: Agent registers via the agent_auth flow described at https://api.past.dev/auth.md, exchanging an identity assertion for a short‑lived access token from the authorization server https://sso.past.dev
  location: header
  name: Agent token
  scopes:
  - memory:read
  - memory:write
  type: oauth2
slug: past-dev-authentication
source_filename: past-dev-authentication.yml
source_heading: Authentication Profile
source_url: https://past.dev/docs/memory-api/authentication
source_yaml: "generated: '2026-10-31'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://past.dev/docs/memory-api/authentication\nsources:\n- https://past.dev/docs/memory-api/authentication\n- https://past.dev/docs/memory-api/authentication/llms.txt\n- https://past.dev/auth.md\n- https://past.dev/tools/token-cost-calculator\ndescription: Authentication methods for past-dev Memory API\nschemes:\n- type: http-bearer\n  name: Project key\n  evidence: 'Authorization: Bearer $PAST_API_KEY'\n  location: header\n  header: Authorization\n  how_to_obtain: Created on the API keys screen of the console at https://app.past.dev or via POST /api/v1/projects/{slug}/keys\n- type: http-bearer\n  name: Management key\n  evidence: 'Authorization: Bearer $PAST_API_KEY'\n  location: header\n  header: Authorization\n  how_to_obtain: Created under Settings → Organization → Management key in the console by an Owner or Admin at https://app.past.dev\n- type: oauth2\n  name: Agent token\n\
  \  evidence: 'WWW-Authenticate: Bearer resource_metadata=\"https://app.past.dev/.well-known/oauth-protected-resource/api/v1\"'\n  location: header\n  header: Authorization\n  scopes:\n  - memory:read\n  - memory:write\n  how_to_obtain: Agent registers via the agent_auth flow described at https://api.past.dev/auth.md, exchanging an identity assertion for a short‑lived\n    access token from the authorization server https://sso.past.dev\ndocs: https://past.dev/docs/memory-api/authentication\n"
source_yaml_url: https://artifacts.apis.io/past-dev/authentication/past-dev-authentication.yml
summary_line: 3 schemes
tags:
- AI
- Memory
- API
- Platform
- Developer
---
