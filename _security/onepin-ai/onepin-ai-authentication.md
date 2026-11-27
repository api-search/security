---
anonymous_access: false
api_key_in: []
auth_types: []
description: Onepin authenticates API requests using an API key supplied as a Bearer token in the Authorization header.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Onepin Authentication
name_suffix: Authentication
oauth_flows: []
overview: Onepin declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Onepin
provider_slug: onepin-ai
scheme_count: 1
schemes:
- evidence: Authenticate the Onepin SDK and CLI with an API key. Onepin uses API keys for all REST API, SDK, and CLI access.
  header: Authorization
  how_to_obtain: Create a key in the Onepin UI at app.onepin.ai → Settings → API → Create new key, then use `onepin login` or set the key via SDK, CLI flag, or ONEPIN_API_KEY environment variable.
  location: header
  name: API Key
  scopes:
  - templates:read
  - workflows:read
  - workflows:run
  - workflows:write
  - voices:read
  - voices:write
  - uploads:write
  - dictionary:read
  - dictionary:write
  - catalog:read
  - workspace:read
  type: http-bearer
slug: onepin-ai-authentication
source_filename: onepin-ai-authentication.yml
source_heading: Authentication Profile
source_url: https://onepin.ai/docs/get-started/authentication
source_yaml: "generated: '2026-11-19'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://onepin.ai/docs/get-started/authentication\nsources:\n- https://onepin.ai/docs/get-started/authentication\n- https://onepin.ai/docs/reference/api-reference/auth/whoami-api-v-1-auth-whoami-get\n- https://onepin.ai/docs/reference/api-reference/workspace-members/accept-invite-api-v-1-workspaces-invites-token-accept-post\n- https://onepin.ai/docs/get-started/quickstart\ndescription: Onepin authenticates API requests using an API key supplied as a Bearer token in the Authorization header.\nschemes:\n- type: http-bearer\n  name: API Key\n  evidence: Authenticate the Onepin SDK and CLI with an API key. Onepin uses API keys for all REST API, SDK, and CLI access.\n  location: header\n  header: Authorization\n  scopes:\n  - templates:read\n  - workflows:read\n  - workflows:run\n  - workflows:write\n  - voices:read\n  - voices:write\n  - uploads:write\n  - dictionary:read\n  - dictionary:write\n\
  \  - catalog:read\n  - workspace:read\n  how_to_obtain: Create a key in the Onepin UI at app.onepin.ai → Settings → API → Create new key, then use `onepin login` or set the key via\n    SDK, CLI flag, or ONEPIN_API_KEY environment variable.\nnote: The MCP server uses OAuth, but no OAuth endpoint URLs or flow details are provided on the referenced pages.\ndocs: https://onepin.ai/docs/get-started/authentication\n"
source_yaml_url: https://artifacts.apis.io/onepin-ai/authentication/onepin-ai-authentication.yml
summary_line: 1 scheme
tags:
- Text-to-Speech
- AI-voice
- Speech Production
---
