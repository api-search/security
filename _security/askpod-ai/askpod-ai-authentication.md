---
anonymous_access: false
api_key_in: []
auth_types: []
description: Authentication methods for Pod
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Askpod Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Pod declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Pod
provider_slug: askpod-ai
scheme_count: 2
schemes:
- evidence: Your MCP client will start Pod's OAuth flow when it connects.
  name: Pod OAuth
  type: oauth2
- evidence: '-H "Authorization: Bearer $POD_API_KEY"'
  header: Authorization
  location: header
  name: API Key
  type: http-bearer
slug: askpod-ai-authentication
source_filename: askpod-ai-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.askpod.ai/quickstart.md
source_yaml: "generated: '2026-11-02'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.askpod.ai/quickstart.md\nsources:\n- https://docs.askpod.ai/quickstart.md\n- https://docs.askpod.ai/quickstart\ndescription: Authentication methods for Pod\nschemes:\n- type: oauth2\n  name: Pod OAuth\n  evidence: Your MCP client will start Pod's OAuth flow when it connects.\n- type: http-bearer\n  name: API Key\n  evidence: '-H \"Authorization: Bearer $POD_API_KEY\"'\n  location: header\n  header: Authorization\ndocs: https://docs.askpod.ai/quickstart.md\n"
source_yaml_url: https://artifacts.apis.io/askpod-ai/authentication/askpod-ai-authentication.yml
summary_line: 2 schemes
tags:
- Artificial Intelligence
- Platform
- Reviews
- Knowledge Base
- Community
- Documentation
---
