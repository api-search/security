---
anonymous_access: false
api_key_in: []
api_specs:
- filename: bugmojo-com-openapi-generated.yml
  format: yaml
  label: BugMojo API
  slug: bugmojo-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bugmojo-com/openapi/_ae-authored/bugmojo-com-openapi-generated.yml
auth_types: []
description: BugMojo supports authentication via browser‑based OAuth flow (default) and via API keys for non‑interactive clients.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Bugmojo Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: BugMojo declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: BugMojo
provider_slug: bugmojo-com
scheme_count: 1
schemes:
- evidence: 'Send it as Authorization: Bearer bm_key_… to /api/mcp , exactly where an OAuth token would go.'
  header: Authorization
  how_to_obtain: Create an API key in Settings → API Keys; it starts with bm_key_ and is shown once.
  location: header
  name: API Key
  type: apiKey
slug: bugmojo-com-authentication
source_filename: bugmojo-com-authentication.yml
source_heading: Authentication Profile
source_url: https://www.bugmojo.com/help/ai-agents-and-mcp/agent-access-and-security-model
source_yaml: "generated: '2026-11-03'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://www.bugmojo.com/help/ai-agents-and-mcp/agent-access-and-security-model\nsources:\n- https://www.bugmojo.com/help/ai-agents-and-mcp/agent-access-and-security-model\n- https://www.bugmojo.com/blog/guides/how-to-fix-unexpected-token-in-json\n- https://www.bugmojo.com/blog/engineering/presigned-upload-pipeline-for-screenshots\n- https://www.bugmojo.com/help/getting-started/what-is-bugmojo\ndescription: BugMojo supports authentication via browser‑based OAuth flow (default) and via API keys for non‑interactive clients.\nschemes:\n- type: apiKey\n  name: API Key\n  evidence: 'Send it as Authorization: Bearer bm_key_… to /api/mcp , exactly where an OAuth token would go.'\n  location: header\n  header: Authorization\n  how_to_obtain: Create an API key in Settings → API Keys; it starts with bm_key_ and is shown once.\nnote: The page describes a browser‑based OAuth flow but does not\
  \ publish the token or authorize URLs, so no OAuth scheme is listed.\ndocs: https://www.bugmojo.com/help/ai-agents-and-mcp/agent-access-and-security-model\n"
source_yaml_url: https://artifacts.apis.io/bugmojo-com/authentication/bugmojo-com-authentication.yml
summary_line: 1 scheme
tags:
- Bug Tracking
- Artificial Intelligence
- Developer Tools
- Session Replay
- Open Source
---
