---
anonymous_access: true
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Callstay Authentication
name_suffix: Authentication
oauth_flows: []
overview: Callstay declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Callstay
provider_slug: callstay-com
scheme_count: 2
schemes:
- applies_to:
  - capabilities
  - search_stays
  - get_property
  - price_stay
  description: 'The docs say "Tools without a key: capabilities, search_stays (place, dates, party), get_property (full detail by slug), price_stay". The MCP GET description adds: "Search, property detail and pricing need no key."'
  name: none
  type: none
- description: 'The docs say "Agent keys for higher limits and for booking tools: partners@callstay.com". They do not say how a key is sent (header name or scheme), and no booking tools are on the public tools/list.'
  name: agent-key
  provisioning: email partners@callstay.com
  type: unspecified
slug: callstay-com-authentication
source_filename: callstay-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: searched\nsource: https://callstay.com/llms.txt\ndocs: https://callstay.com/llms.txt\nschemes:\n- name: none\n  type: none\n  applies_to: [capabilities, search_stays, get_property, price_stay]\n  description: 'The docs say \"Tools without a key: capabilities, search_stays (place, dates, party), get_property (full detail by slug), price_stay\". The MCP GET description adds: \"Search, property detail and pricing need no key.\"'\n- name: agent-key\n  type: unspecified\n  description: 'The docs say \"Agent keys for higher limits and for booking tools: partners@callstay.com\". They do not say how a key is sent (header name or scheme), and no booking tools are on the public tools/list.'\n  provisioning: email partners@callstay.com\nevidence:\n- url: https://callstay.com/api/mcp\n  http_status: 200\n  note: 'GET description field \"keys\": \"partners@callstay.com\"'\n"
source_yaml_url: https://artifacts.apis.io/callstay-com/authentication/callstay-com-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Travel
- Hotels
- Hotel Booking
- Accommodation
- Reservations
- MCP
- AI Agents
---
