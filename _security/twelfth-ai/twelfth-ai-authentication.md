---
anonymous_access: false
api_key_in: []
api_specs:
- filename: twelfth-ai-tasks-api-openapi.yml
  format: yaml
  label: twelfth-ai Tasks API
  slug: twelfth-ai-tasks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/twelfth-ai/openapi/twelfth-ai-tasks-api-openapi.yml
- filename: twelfth-ai-workspace-api-openapi.yml
  format: yaml
  label: twelfth-ai Workspace API
  slug: twelfth-ai-workspace-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/twelfth-ai/openapi/twelfth-ai-workspace-api-openapi.yml
auth_types: []
description: Authentication schemes for Twelfth AI
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Twelfth Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: twelfth-ai declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: twelfth-ai
provider_slug: twelfth-ai
scheme_count: 1
schemes:
- evidence: Servers, scripts and automations authenticate to the Twelfth REST API with a bearer key .
  header: Authorization
  how_to_obtain: Owners and admins create and revoke workspace keys from Settings → AI & agents; the key is shown once when created.
  location: header
  name: Authorization
  type: http-bearer
slug: twelfth-ai-authentication
source_filename: twelfth-ai-authentication.yml
source_heading: Authentication Profile
source_url: https://twelfth.ai/docs/settings/ai-and-agents/api-keys
source_yaml: "generated: '2026-10-20'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://twelfth.ai/docs/settings/ai-and-agents/api-keys\nsources:\n- https://twelfth.ai/docs/settings/ai-and-agents/api-keys\n- https://twelfth.ai/docs/signing-in\n- https://twelfth.ai/docs/getting-started/\n- https://twelfth.ai/docs/getting-started\ndescription: Authentication schemes for Twelfth AI\nschemes:\n- type: http-bearer\n  name: Authorization\n  evidence: Servers, scripts and automations authenticate to the Twelfth REST API with a bearer key .\n  location: header\n  header: Authorization\n  how_to_obtain: Owners and admins create and revoke workspace keys from Settings → AI & agents; the key is shown once when created.\nnote: No OAuth2 or other authentication methods are documented on the provided pages.\ndocs: https://twelfth.ai/docs/settings/ai-and-agents/api-keys\n"
source_yaml_url: https://artifacts.apis.io/twelfth-ai/authentication/twelfth-ai-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Retail
- Commerce
- AI
- Workspace
---
