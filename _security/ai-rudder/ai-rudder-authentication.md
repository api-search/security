---
anonymous_access: false
api_key_in: []
api_specs:
- filename: ai-rudder-openapi-generated.yml
  format: yaml
  label: AI Rudder API
  slug: ai-rudder-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ai-rudder/openapi/_ae-authored/ai-rudder-openapi-generated.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Ai Rudder Authentication
name_suffix: Authentication
oauth_flows: []
overview: AI Rudder declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: AI Rudder
provider_slug: ai-rudder
scheme_count: 1
schemes:
- evidence: Obtain the token and add it to the request header of other APIs.
  header: Authorization
  how_to_obtain: Contact us to get your APPKey and APPSecret.
  location: header
  name: Bearer
  token_url: https://api.airudder.com/service/cloud/auth
  type: http-bearer
slug: ai-rudder-authentication
source_filename: ai-rudder-authentication.yml
source_heading: Authentication Profile
source_url: https://api-docs.airudder.com/api-44712004.md
source_yaml: "generated: '2026-10-25'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://api-docs.airudder.com/api-44712004.md\nsources:\n- https://api-docs.airudder.com/api-44712004.md\n- https://api-docs.airudder.com/api-334041765.md\n- https://developer.airudder.com/api-44712004\n- https://developer.airudder.com/api-334041765\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: Obtain the token and add it to the request header of other APIs.\n  location: header\n  header: Authorization\n  token_url: https://api.airudder.com/service/cloud/auth\n  how_to_obtain: Contact us to get your APPKey and APPSecret.\ndocs: https://api-docs.airudder.com/api-44712004.md\n"
source_yaml_url: https://artifacts.apis.io/ai-rudder/authentication/ai-rudder-authentication.yml
summary_line: 1 scheme
tags:
- AI
- ConversationalAI
- Enterprise
- Automation
- Platform
---
