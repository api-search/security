---
anonymous_access: false
api_key_in: []
api_specs:
- filename: adplug-health-api-openapi.yml
  format: yaml
  label: AdPlug Health API
  slug: adplug-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adplug/refs/heads/main/openapi/adplug-health-api-openapi.yml
- filename: adplug-mcp-api-openapi.yml
  format: yaml
  label: AdPlug MCP API
  slug: adplug-mcp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adplug/refs/heads/main/openapi/adplug-mcp-api-openapi.yml
- filename: adplug-oauth-api-openapi.yml
  format: yaml
  label: AdPlug OAuth API
  slug: adplug-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adplug/refs/heads/main/openapi/adplug-oauth-api-openapi.yml
- filename: adplug-oauth-legacy-compat-api-openapi.yml
  format: yaml
  label: AdPlug OAUTH Legacy Compat API
  slug: adplug-oauth-legacy-compat-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adplug/refs/heads/main/openapi/adplug-oauth-legacy-compat-api-openapi.yml
- filename: adplug-users-api-openapi.yml
  format: yaml
  label: AdPlug Users API
  slug: adplug-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adplug/refs/heads/main/openapi/adplug-users-api-openapi.yml
- filename: adplug-webhooks-api-openapi.yml
  format: yaml
  label: AdPlug Webhooks API
  slug: adplug-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adplug/refs/heads/main/openapi/adplug-webhooks-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Adplug Authentication
name_suffix: Authentication
oauth_flows: []
overview: AdPlug secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: AdPlug
provider_slug: adplug
scheme_count: 1
schemes:
- name: HTTPBearer
  scheme: bearer
  sources:
  - openapi/adplug.json
  type: http
slug: adplug-authentication
source_filename: adplug-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-15'\nmethod: derived\nsource: openapi/adplug.json\nsummary:\n  types:\n  - http\nschemes:\n- name: HTTPBearer\n  type: http\n  scheme: bearer\n  sources:\n  - openapi/adplug.json\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/adplug/refs/heads/main/authentication/adplug-authentication.yml
summary_line: http · 1 scheme
tags:
- PPC
- AI Integration
- Agency Tools
- Search Console
---
