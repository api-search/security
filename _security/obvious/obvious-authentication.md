---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication via API key as Bearer token
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Obvious Authentication
name_suffix: Authentication
oauth_flows: []
overview: Obvious declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Obvious
provider_slug: obvious
scheme_count: 1
schemes:
- evidence: All requests to the Obvious API require authentication via an API key passed as a Bearer token in the Authorization header.
  header: Authorization
  how_to_obtain: API keys are created in workspace settings under Settings → Workspace → Integrations → External Access. Click Create External Access, enter a name, and copy the displayed key.
  location: header
  name: API Key
  type: http-bearer
slug: obvious-authentication
source_filename: obvious-authentication.yml
source_heading: Authentication Profile
source_url: https://help.obvious.ai/developer-api/authentication
source_yaml: "generated: '2026-10-24'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://help.obvious.ai/developer-api/authentication\nsources:\n- https://help.obvious.ai/developer-api/authentication\n- https://help.obvious.ai/account/two-factor-auth\n- https://help.obvious.ai/getting-started\n- https://help.obvious.ai/getting-started/sidebar-sections\ndescription: Authentication via API key as Bearer token\nschemes:\n- type: http-bearer\n  name: API Key\n  evidence: All requests to the Obvious API require authentication via an API key passed as a Bearer token in the Authorization header.\n  location: header\n  header: Authorization\n  how_to_obtain: API keys are created in workspace settings under Settings → Workspace → Integrations → External Access. Click Create External\n    Access, enter a name, and copy the displayed key.\nnote: No OAuth2 or other authentication schemes are documented.\ndocs: https://help.obvious.ai/developer-api/authentication\n"
source_yaml_url: https://artifacts.apis.io/obvious/authentication/obvious-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Data Analytics
- AI
- Enterprise
- APIs
---
