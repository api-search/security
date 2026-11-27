---
anonymous_access: false
api_key_in: []
api_specs:
- filename: syntheticbrew-ai-getting-started-openapi-generated.yml
  format: yaml
  label: SyntheticBrew getting started API
  slug: getting-started-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/syntheticbrew-ai/openapi/_ae-authored/syntheticbrew-ai-getting-started-openapi-generated.yml
- filename: syntheticbrew-ai-integration-openapi-generated.yml
  format: yaml
  label: SyntheticBrew integration API
  slug: integration-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/syntheticbrew-ai/openapi/_ae-authored/syntheticbrew-ai-integration-openapi-generated.yml
auth_types: []
description: Authentication methods for SyntheticBrew
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: SyntheticBrew Authentication
name_suffix: Authentication
oauth_flows: []
overview: SyntheticBrew declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: SyntheticBrew
provider_slug: syntheticbrew-ai
scheme_count: 3
schemes:
- evidence: 'Send `Authorization: Bearer <access_token>` on every API request.'
  header: Authorization
  location: header
  name: Bearer JWT
  type: http-bearer
- evidence: 'Send `Authorization: Bearer <access_token>` on every API request.'
  header: Authorization
  location: header
  name: Scoped API tokens
  type: http-bearer
- authorize_url: https://app.syntheticbrew.ai/admin/oauth/consent
  evidence: 'Run `authorization_code` + PKCE (S256): the user consents at `https://app.syntheticbrew.ai/admin/oauth/consent`, tokens come from `https://app.syntheticbrew.ai/oauth/token`.'
  flows:
  - authorization_code
  - refresh_token
  how_to_obtain: Dynamic client registration via POST https://app.syntheticbrew.ai/oauth/register
  name: MCP OAuth
  scopes:
  - provision
  - manage
  - offline_access
  token_url: https://app.syntheticbrew.ai/oauth/token
  type: oauth2
slug: syntheticbrew-ai-authentication
source_filename: syntheticbrew-ai-authentication.yml
source_heading: Authentication Profile
source_url: https://syntheticbrew.ai/auth.md
source_yaml: "generated: '2026-11-25'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://syntheticbrew.ai/auth.md\nsources:\n- https://syntheticbrew.ai/auth.md\n- https://syntheticbrew.ai/.well-known/oauth-protected-resource\n- https://app.syntheticbrew.ai/.well-known/oauth-authorization-server\n- https://syntheticbrew.ai/docs/admin/api-keys\ndescription: Authentication methods for SyntheticBrew\nschemes:\n- type: http-bearer\n  name: Bearer JWT\n  evidence: 'Send `Authorization: Bearer <access_token>` on every API request.'\n  location: header\n  header: Authorization\n- type: http-bearer\n  name: Scoped API tokens\n  evidence: 'Send `Authorization: Bearer <access_token>` on every API request.'\n  location: header\n  header: Authorization\n- type: oauth2\n  name: MCP OAuth\n  evidence: 'Run `authorization_code` + PKCE (S256): the user consents at `https://app.syntheticbrew.ai/admin/oauth/consent`, tokens come from\n    `https://app.syntheticbrew.ai/oauth/token`.'\n\
  \  flows:\n  - authorization_code\n  - refresh_token\n  token_url: https://app.syntheticbrew.ai/oauth/token\n  authorize_url: https://app.syntheticbrew.ai/admin/oauth/consent\n  scopes:\n  - provision\n  - manage\n  - offline_access\n  how_to_obtain: Dynamic client registration via POST https://app.syntheticbrew.ai/oauth/register\ndocs: https://syntheticbrew.ai/auth.md\n"
source_yaml_url: https://artifacts.apis.io/syntheticbrew-ai/authentication/syntheticbrew-ai-authentication.yml
summary_line: 3 schemes
tags:
- AI
- Infrastructure
- Enterprise
- Agents
- NoCode
---
