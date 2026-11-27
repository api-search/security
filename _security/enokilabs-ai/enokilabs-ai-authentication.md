---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication methods for Enoki Labs API
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Enoki Labs Authentication
name_suffix: Authentication
oauth_flows: []
overview: Enoki Labs declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Enoki Labs
provider_slug: enokilabs-ai
scheme_count: 1
schemes:
- evidence: Enoki's REST API authenticates with a workspace API key, passed as a Bearer token
  header: Authorization
  how_to_obtain: Create a key in the Enoki app under Settings → API Keys; the full key (prefixed `egk_`) is shown once and must be copied securely.
  location: header
  name: Workspace API Key
  type: http-bearer
slug: enokilabs-ai-authentication
source_filename: enokilabs-ai-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.enokilabs.ai/api-keys.md
source_yaml: "generated: '2026-11-06'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.enokilabs.ai/api-keys.md\nsources:\n- https://docs.enokilabs.ai/api-keys.md\n- https://docs.enokilabs.ai/quickstart.md\ndescription: Authentication methods for Enoki Labs API\nschemes:\n- type: http-bearer\n  name: Workspace API Key\n  evidence: Enoki's REST API authenticates with a workspace API key, passed as a Bearer token\n  location: header\n  header: Authorization\n  how_to_obtain: Create a key in the Enoki app under Settings → API Keys; the full key (prefixed `egk_`) is shown once and must be copied securely.\nnote: No OAuth2, apiKey, or other authentication schemes are documented on the provided pages.\ndocs: https://docs.enokilabs.ai/api-keys.md\n"
source_yaml_url: https://artifacts.apis.io/enokilabs-ai/authentication/enokilabs-ai-authentication.yml
summary_line: 1 scheme
tags:
- Artificial Intelligence
- Security
- Testing
- Automation
- Platform
---
