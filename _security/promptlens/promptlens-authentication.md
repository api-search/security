---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication methods published for PromptLens
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Promptlens Authentication
name_suffix: Authentication
oauth_flows: []
overview: PromptLens declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: PromptLens
provider_slug: promptlens
scheme_count: 3
schemes:
- evidence: Management requests use a Clerk OAuth access token with the management scope and the canonical https://www.promptlens.io/api/v1 resource.
  flows:
  - authorization_code
  how_to_obtain: Register a client and use the authorization‑code flow with PKCE as described in the documentation.
  name: Clerk OAuth
  scopes:
  - management
  type: oauth2
- evidence: A retrieval key grants read access to saved configuration for one prompt.
  how_to_obtain: Create the key in the PromptLens dashboard under the prompt’s key controls.
  name: Prompt‑scoped retrieval key
  type: apiKey
- evidence: A separate organization ingestion key; see trace ingestion.
  how_to_obtain: Create the key via the trace ingestion documentation.
  name: Trace ingestion key
  type: apiKey
slug: promptlens-authentication
source_filename: promptlens-authentication.yml
source_heading: Authentication Profile
source_url: https://www.promptlens.io/auth.md
source_yaml: "generated: '2026-10-18'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://www.promptlens.io/auth.md\nsources:\n- https://www.promptlens.io/auth.md\n- https://www.promptlens.io/docs/api-reference\n- https://www.promptlens.io/docs/integrations/keys\n- https://www.promptlens.io/docs/mcp\ndescription: Authentication methods published for PromptLens\nschemes:\n- type: oauth2\n  name: Clerk OAuth\n  evidence: Management requests use a Clerk OAuth access token with the management scope and the canonical https://www.promptlens.io/api/v1 resource.\n  flows:\n  - authorization_code\n  scopes:\n  - management\n  how_to_obtain: Register a client and use the authorization‑code flow with PKCE as described in the documentation.\n- type: apiKey\n  name: Prompt‑scoped retrieval key\n  evidence: A retrieval key grants read access to saved configuration for one prompt.\n  how_to_obtain: Create the key in the PromptLens dashboard under the prompt’s key controls.\n\
  - type: apiKey\n  name: Trace ingestion key\n  evidence: A separate organization ingestion key; see trace ingestion.\n  how_to_obtain: Create the key via the trace ingestion documentation.\ndocs: https://www.promptlens.io/auth.md\n"
source_yaml_url: https://artifacts.apis.io/promptlens/authentication/promptlens-authentication.yml
summary_line: 3 schemes
tags:
- Company
- Artificial Intelligence
- Monitoring
- Testing
- LLM
- Observability
---
