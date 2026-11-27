---
anonymous_access: false
api_key_in: []
api_specs:
- filename: callchatsyn-com-answer-api-openapi.yml
  format: yaml
  label: CallChatSyn Answer API
  slug: callchatsyn-com-answer-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/callchatsyn-com/openapi/callchatsyn-com-answer-api-openapi.yml
- filename: callchatsyn-com-bookings-api-openapi.yml
  format: yaml
  label: CallChatSyn Bookings API
  slug: callchatsyn-com-bookings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/callchatsyn-com/openapi/callchatsyn-com-bookings-api-openapi.yml
- filename: callchatsyn-com-slots-api-openapi.yml
  format: yaml
  label: CallChatSyn Slots API
  slug: callchatsyn-com-slots-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/callchatsyn-com/openapi/callchatsyn-com-slots-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: CallChatSyn Authentication
name_suffix: Authentication
oauth_flows: []
overview: CallChatSyn secures its APIs with http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: CallChatSyn
provider_slug: callchatsyn-com
scheme_count: 2
schemes:
- description: ccs_live_… API key, or the public demo key ccs_demo_public
  format: 'Authorization: Bearer ccs_live_…'
  header: Authorization
  issuance: In Dashboard → Developers, create a key. It's shown once; keep it on your server, never in browser code.
  key_prefixes:
    demo: ccs_demo_public
    live: ccs_live_
  name: bearer
  scheme: bearer
  scope_note: One key acts for one business (WhatsApp guide).
  sources:
  - openapi/callchatsyn-com-openapi.yml
  - https://callchatsyn.com/developers
  - https://callchatsyn.com/developers/whatsapp
  type: http
- applies_to: https://callchatsyn.com/api/mcp
  description: 'With no key it uses the demo business; send Authorization: Bearer ccs_live_… to use your own.'
  name: mcp-bearer
  scheme: bearer
  sources:
  - https://callchatsyn.com/developers
  type: http
slug: callchatsyn-com-authentication
source_filename: callchatsyn-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: searched\nsource: https://callchatsyn.com/developers\ndocs: https://callchatsyn.com/developers\nsummary:\n  types:\n  - http\nschemes:\n- name: bearer\n  type: http\n  scheme: bearer\n  header: Authorization\n  format: 'Authorization: Bearer ccs_live_…'\n  description: ccs_live_… API key, or the public demo key ccs_demo_public\n  key_prefixes:\n    live: ccs_live_\n    demo: ccs_demo_public\n  issuance: \"In Dashboard → Developers, create a key. It's shown once; keep it on your server, never in browser code.\"\n  scope_note: One key acts for one business (WhatsApp guide).\n  sources:\n  - openapi/callchatsyn-com-openapi.yml\n  - https://callchatsyn.com/developers\n  - https://callchatsyn.com/developers/whatsapp\n- name: mcp-bearer\n  type: http\n  scheme: bearer\n  applies_to: https://callchatsyn.com/api/mcp\n  description: \"With no key it uses the demo business; send Authorization: Bearer ccs_live_… to use your own.\"\n  sources:\n  - https://callchatsyn.com/developers\n"
source_yaml_url: https://artifacts.apis.io/callchatsyn-com/authentication/callchatsyn-com-authentication.yml
summary_line: http · 2 schemes
tags:
- Company
- AI Receptionist
- Answering Service
- Voice AI
- Appointment Booking
- Chatbots
- WhatsApp
- Small Business
- MCP
---
