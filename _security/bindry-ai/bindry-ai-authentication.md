---
anonymous_access: false
api_key_in: []
api_specs:
- filename: bindry-ai-openapi-generated.yml
  format: yaml
  label: Bindry API
  slug: bindry-ai-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bindry-ai/openapi/_ae-authored/bindry-ai-openapi-generated.yml
auth_types: []
description: Bindry uses API keys that are provided as an environment variable named BINDRY_API_TOKEN.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Bindry Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Bindry declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Bindry
provider_slug: bindry-ai
scheme_count: 1
schemes:
- evidence: Put it in BINDRY_API_TOKEN Set it as an environment variable rather than pasting it into a command — both /bindry-sync and /bindry-connect read the same variable, and it's the only credential either one needs.
  name: API Key
  type: other
slug: bindry-ai-authentication
source_filename: bindry-ai-authentication.yml
source_heading: Authentication Profile
source_url: https://bindry.ai/api-keys
source_yaml: "generated: '2026-11-02'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://bindry.ai/api-keys\nsources:\n- https://bindry.ai/api-keys\n- https://bindry.ai/plugins/claude-code\n- https://bindry.ai/plugins/codex\n- https://bindry.ai/plugins/copilot\ndescription: Bindry uses API keys that are provided as an environment variable named BINDRY_API_TOKEN.\nschemes:\n- type: other\n  name: API Key\n  evidence: Put it in BINDRY_API_TOKEN Set it as an environment variable rather than pasting it into a command — both /bindry-sync and /bindry-connect\n    read the same variable, and it's the only credential either one needs.\nnote: No OAuth2, HTTP basic, bearer, JWT, HMAC, or mTLS schemes are documented on the provided pages.\ndocs: https://bindry.ai/api-keys\n"
source_yaml_url: https://artifacts.apis.io/bindry-ai/authentication/bindry-ai-authentication.yml
summary_line: 1 scheme
tags:
- Artificial Intelligence
- Package Manager
- Skills
- Developer Tools
- Open Source
- Company
---
