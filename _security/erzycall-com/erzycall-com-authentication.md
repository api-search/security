---
anonymous_access: false
api_key_in: []
api_specs:
- filename: erzycall-com-openapi-generated.yml
  format: yaml
  label: ErzyCall API
  slug: erzycall-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/erzycall-com/openapi/_ae-authored/erzycall-com-openapi-generated.yml
auth_types: []
description: Authentication schemes for ErzyCall API
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: ErzyCall Authentication
name_suffix: Authentication
oauth_flows: []
overview: ErzyCall declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: ErzyCall
provider_slug: erzycall-com
scheme_count: 1
schemes:
- evidence: Every request to the ErzyCall REST API must include a valid API key in the X-API-Key header.
  header: X-API-Key
  how_to_obtain: Navigate to Settings > API Keys in the ErzyCall dashboard, click Create API Key, give it a name and select the scopes your integration needs, then copy the key immediately.
  location: header
  name: API Key
  type: apiKey
slug: erzycall-com-authentication
source_filename: erzycall-com-authentication.yml
source_heading: Authentication Profile
source_url: https://app.erzycall.com/docs/authentication
source_yaml: "generated: '2026-11-07'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://app.erzycall.com/docs/authentication\nsources:\n- https://app.erzycall.com/docs/authentication\n- https://app.erzycall.com/docs/api-reference/organization\n- https://app.erzycall.com/docs\ndescription: Authentication schemes for ErzyCall API\nschemes:\n- type: apiKey\n  name: API Key\n  evidence: Every request to the ErzyCall REST API must include a valid API key in the X-API-Key header.\n  location: header\n  header: X-API-Key\n  how_to_obtain: Navigate to Settings > API Keys in the ErzyCall dashboard, click Create API Key, give it a name and select the scopes your integration\n    needs, then copy the key immediately.\nnote: No OAuth2 or other authentication schemes are documented.\ndocs: https://app.erzycall.com/docs/authentication\n"
source_yaml_url: https://artifacts.apis.io/erzycall-com/authentication/erzycall-com-authentication.yml
summary_line: 1 scheme
tags:
- AI Call
- Virtual Receptionist
- Inbound Calls
- Outbound Calls
- WhatsApp
- Appointment Scheduling
- CRM Integration
- Call Analytics
---
