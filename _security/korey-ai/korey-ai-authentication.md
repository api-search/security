---
anonymous_access: false
api_key_in: []
api_specs:
- filename: korey-ai-identity-api-openapi.yml
  format: yaml
  label: Korey Identity API
  slug: korey-ai-identity-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/korey-ai/openapi/korey-ai-identity-api-openapi.yml
- filename: korey-ai-threads-api-openapi.yml
  format: yaml
  label: Korey Threads API
  slug: korey-ai-threads-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/korey-ai/openapi/korey-ai-threads-api-openapi.yml
auth_types: []
description: Authentication methods published by Korey
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Korey Authentication
name_suffix: Authentication
oauth_flows: []
overview: Korey declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Korey
provider_slug: korey-ai
scheme_count: 2
schemes:
- authorize_url: https://api.korey.ai/oauth/authorize
  evidence: Korey supports OAuth 2.0 so third-party tools — editor extensions, scripts, CI jobs — can ask for your permission before accessing the Korey API on your behalf.
  flows:
  - authorization_code
  how_to_obtain: Register an OAuth client in Settings → OAuth Clients, then use the client ID (and secret for confidential clients) to perform the authorization code flow.
  name: OAuth 2.0
  scopes:
  - threads:read
  - threads:read:own
  - threads:write
  type: oauth2
- evidence: API Tokens API tokens let scripts, CI jobs, and other tools talk to the Korey API on your behalf.
  header: Authorization
  how_to_obtain: Create a token via Settings → Profile → API Tokens, then copy the token and use it as a Bearer token in the Authorization header.
  location: header
  name: API Token
  type: http-bearer
slug: korey-ai-authentication
source_filename: korey-ai-authentication.yml
source_heading: Authentication Profile
source_url: https://korey.ai/docs/developers/oauth/
source_yaml: "generated: '2026-11-14'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://korey.ai/docs/developers/oauth/\nsources:\n- https://korey.ai/docs/developers/oauth/\n- https://korey.ai/docs/developers/api-tokens/\n- https://korey.ai/docs/getting-started/what-korey-does-best/\n- https://korey.ai/docs/getting-started/quick-start/\ndescription: Authentication methods published by Korey\nschemes:\n- type: oauth2\n  name: OAuth 2.0\n  evidence: Korey supports OAuth 2.0 so third-party tools — editor extensions, scripts, CI jobs — can ask for your permission before accessing\n    the Korey API on your behalf.\n  flows:\n  - authorization_code\n  authorize_url: https://api.korey.ai/oauth/authorize\n  scopes:\n  - threads:read\n  - threads:read:own\n  - threads:write\n  how_to_obtain: Register an OAuth client in Settings → OAuth Clients, then use the client ID (and secret for confidential clients) to perform\n    the authorization code flow.\n- type: http-bearer\n\
  \  name: API Token\n  evidence: API Tokens API tokens let scripts, CI jobs, and other tools talk to the Korey API on your behalf.\n  location: header\n  header: Authorization\n  how_to_obtain: Create a token via Settings → Profile → API Tokens, then copy the token and use it as a Bearer token in the Authorization header.\ndocs: https://korey.ai/docs/developers/oauth/\n"
source_yaml_url: https://artifacts.apis.io/korey-ai/authentication/korey-ai-authentication.yml
summary_line: 2 schemes
tags:
- AI Agents
- Product Teams
- Approval Workflow
- Collaboration
---
