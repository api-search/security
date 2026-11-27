---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Coordínalo Authentication
name_suffix: Authentication
oauth_flows: []
overview: Coordínalo declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: Coordínalo
provider_slug: coordinalo-com
scheme_count: 3
schemes:
- description: An organization API key, sent in the X-Org-Api-Key header. 103 of the 112 MCP tools also accept an `apiKey` input property. The developer page says keys are free, issued in minutes after you request one and verify your email, and that "Tu key aparece una sola vez — guárdala" (the key is shown only once, so save it).
  header: X-Org-Api-Key
  in: header
  name: org-api-key
  source: https://coordinalo.com/developers
  type: apiKey
- description: The public booking tools (public_*) need no API key. public_booking_create returns a confirmationToken, which expires after 30 minutes and is used by public_booking_confirm, and a bookingToken that "scopes access to a single booking" for cancel/reschedule.
  name: public-booking-tokens
  source: json-schema/coordinalo-com-mcp-tools-list.json
  type: token
- bearerFormat: JWT
  description: The docs security section says the web app uses "Supabase Auth con contraseñas hasheadas (bcrypt) y tokens JWT con expiración", with Administrador and Profesional roles. This covers the end-user app, not the documented API surface.
  name: app-user-auth
  scheme: bearer
  source: https://coordinalo.com/docs
  type: http
slug: coordinalo-com-authentication
source_filename: coordinalo-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://coordinalo.com/developers\ndocs: https://coordinalo.com/developers\nnote: There is no OpenAPI. The auth profile is read from the developer page and from the MCP tools/list the provider serves at https://coordinalo.com/api/mcp (saved as json-schema/coordinalo-com-mcp-tools-list.json). Authentication endpoints were not called.\nschemes:\n- name: org-api-key\n  type: apiKey\n  in: header\n  header: X-Org-Api-Key\n  description: An organization API key, sent in the X-Org-Api-Key header. 103 of the 112 MCP tools also accept an `apiKey` input property. The developer page says keys are free, issued in minutes after you request one and verify your email, and that \"Tu key aparece una sola vez — guárdala\" (the key is shown only once, so save it).\n  source: https://coordinalo.com/developers\n- name: public-booking-tokens\n  type: token\n  description: The public booking tools (public_*) need no API key. public_booking_create\
  \ returns a confirmationToken, which expires after 30 minutes and is used by public_booking_confirm, and a bookingToken that \"scopes access to a single booking\" for cancel/reschedule.\n  source: json-schema/coordinalo-com-mcp-tools-list.json\n- name: app-user-auth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  description: The docs security section says the web app uses \"Supabase Auth con contraseñas hasheadas (bcrypt) y tokens JWT con expiración\", with Administrador and Profesional roles. This covers the end-user app, not the documented API surface.\n  source: https://coordinalo.com/docs\n"
source_yaml_url: https://artifacts.apis.io/coordinalo-com/authentication/coordinalo-com-authentication.yml
summary_line: 3 schemes
tags:
- Company
- Practice Management
- Healthcare
- Scheduling
- Booking
- Payments
- MCP
- Chile
---
