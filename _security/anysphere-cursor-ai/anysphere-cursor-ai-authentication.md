---
anonymous_access: false
api_key_in: []
api_specs:
- filename: anysphere-cursor-ai-originservice-api-openapi.yml
  format: yaml
  label: Anysphere Cursor Ai Origin Service API
  slug: anysphere-cursor-ai-originservice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/anysphere-cursor-ai/refs/heads/main/openapi/anysphere-cursor-ai-originservice-api-openapi.yml
auth_types: []
description: Authentication methods published for Anysphere Cursor AI
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Anysphere Cursor Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Anysphere Cursor Ai declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Anysphere Cursor Ai
provider_slug: anysphere-cursor-ai
scheme_count: 1
schemes:
- evidence: 'Service accounts authenticate using their API key. Use the key in the Authorization header when making requests to the Cloud Agents API :'
  header: Authorization
  how_to_obtain: API key generated when creating a service account; copy immediately as it is shown only once.
  location: header
  name: Authorization
  type: http-bearer
slug: anysphere-cursor-ai-authentication
source_filename: anysphere-cursor-ai-authentication.yml
source_heading: Authentication Profile
source_url: https://cursor.com/docs/account/enterprise/service-accounts
source_yaml: "generated: '2026-09-25'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://cursor.com/docs/account/enterprise/service-accounts\nsources:\n- https://cursor.com/docs/account/enterprise/service-accounts\n- https://cursor.com/docs/get-started/quickstart\n- https://cursor.com/docs/cloud-agent/setup\ndescription: Authentication methods published for Anysphere Cursor AI\nschemes:\n- type: http-bearer\n  name: Authorization\n  evidence: 'Service accounts authenticate using their API key. Use the key in the Authorization header when making requests to the Cloud Agents\n    API :'\n  location: header\n  header: Authorization\n  how_to_obtain: API key generated when creating a service account; copy immediately as it is shown only once.\nnote: No OAuth2, apiKey, or other authentication schemes are documented on the provided pages.\ndocs: https://cursor.com/docs/account/enterprise/service-accounts\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/anysphere-cursor-ai/refs/heads/main/authentication/anysphere-cursor-ai-authentication.yml
summary_line: 1 scheme
tags:
- Company
- AI
- Coding
- Developer-Tools
- Automation
- Platform
---
