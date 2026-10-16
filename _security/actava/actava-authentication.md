---
anonymous_access: false
api_key_in: []
api_specs:
- filename: actava-models-api-openapi.yml
  format: yaml
  label: Actava.ai Models API
  slug: actava-models-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/actava/refs/heads/main/openapi/actava-models-api-openapi.yml
- filename: actava-chat-completions-api-openapi.yml
  format: yaml
  label: Actava.ai Chat Completions API
  slug: actava-chat-completions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/actava/refs/heads/main/openapi/actava-chat-completions-api-openapi.yml
auth_types: []
description: Authentication methods as published on Actava.ai documentation.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Actava Authentication
name_suffix: Authentication
oauth_flows: []
overview: Actava.ai declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Actava.ai
provider_slug: actava
scheme_count: 1
schemes:
- evidence: All requests go to the base URL below with a bearer token.
  header: Authorization
  how_to_obtain: API keys are issued by Actava.ai. Join the waitlist and we'll set you up.
  location: header
  name: Bearer
  type: http-bearer
slug: actava-authentication
source_filename: actava-authentication.yml
source_heading: Authentication Profile
source_url: https://www.actava.ai/cura/docs#get-a-key
source_yaml: "generated: '2026-10-15'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://www.actava.ai/cura/docs#get-a-key\nsources:\n- https://www.actava.ai/cura/docs#get-a-key\n- https://www.actava.ai/cura/docs\n- https://www.actava.ai/benchmarks/docs/quickstart\ndescription: Authentication methods as published on Actava.ai documentation.\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: All requests go to the base URL below with a bearer token.\n  location: header\n  header: Authorization\n  how_to_obtain: API keys are issued by Actava.ai. Join the waitlist and we'll set you up.\ndocs: https://www.actava.ai/cura/docs#get-a-key\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/actava/refs/heads/main/authentication/actava-authentication.yml
summary_line: 1 scheme
tags:
- Company
- AI
- Healthcare
- MachineLearning
- Platform
---
