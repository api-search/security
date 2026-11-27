---
anonymous_access: false
api_key_in:
- cookie
- header
api_specs:
- filename: craftingeventfinder-com-account-api-openapi.yml
  format: yaml
  label: Crafting Event Finder Account API
  slug: craftingeventfinder-com-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/craftingeventfinder-com/openapi/craftingeventfinder-com-account-api-openapi.yml
- filename: craftingeventfinder-com-admin-api-openapi.yml
  format: yaml
  label: Crafting Event Finder Admin API
  slug: craftingeventfinder-com-admin-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/craftingeventfinder-com/openapi/craftingeventfinder-com-admin-api-openapi.yml
- filename: craftingeventfinder-com-auth-api-openapi.yml
  format: yaml
  label: Crafting Event Finder Auth API
  slug: craftingeventfinder-com-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/craftingeventfinder-com/openapi/craftingeventfinder-com-auth-api-openapi.yml
- filename: craftingeventfinder-com-events-api-openapi.yml
  format: yaml
  label: Crafting Event Finder Events API
  slug: craftingeventfinder-com-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/craftingeventfinder-com/openapi/craftingeventfinder-com-events-api-openapi.yml
- filename: craftingeventfinder-com-mcp-api-openapi.yml
  format: yaml
  label: Crafting Event Finder MCP API
  slug: craftingeventfinder-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/craftingeventfinder-com/openapi/craftingeventfinder-com-mcp-api-openapi.yml
- filename: craftingeventfinder-com-network-api-openapi.yml
  format: yaml
  label: Crafting Event Finder Network API
  slug: craftingeventfinder-com-network-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/craftingeventfinder-com/openapi/craftingeventfinder-com-network-api-openapi.yml
- filename: craftingeventfinder-com-organizers-api-openapi.yml
  format: yaml
  label: Crafting Event Finder Organizers API
  slug: craftingeventfinder-com-organizers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/craftingeventfinder-com/openapi/craftingeventfinder-com-organizers-api-openapi.yml
- filename: craftingeventfinder-com-platform-api-openapi.yml
  format: yaml
  label: Crafting Event Finder Platform API
  slug: craftingeventfinder-com-platform-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/craftingeventfinder-com/openapi/craftingeventfinder-com-platform-api-openapi.yml
- filename: craftingeventfinder-com-preferences-api-openapi.yml
  format: yaml
  label: Crafting Event Finder Preferences API
  slug: craftingeventfinder-com-preferences-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/craftingeventfinder-com/openapi/craftingeventfinder-com-preferences-api-openapi.yml
- filename: craftingeventfinder-com-submissions-api-openapi.yml
  format: yaml
  label: Crafting Event Finder Submissions API
  slug: craftingeventfinder-com-submissions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/craftingeventfinder-com/openapi/craftingeventfinder-com-submissions-api-openapi.yml
- filename: craftingeventfinder-com-taxonomy-api-openapi.yml
  format: yaml
  label: Crafting Event Finder Taxonomy API
  slug: craftingeventfinder-com-taxonomy-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/craftingeventfinder-com/openapi/craftingeventfinder-com-taxonomy-api-openapi.yml
auth_types:
- apiKey
- http
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Crafting Event Finder Authentication
name_suffix: Authentication
oauth_flows: []
overview: Crafting Event Finder secures its APIs with apiKey and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Crafting Event Finder
provider_slug: craftingeventfinder-com
scheme_count: 2
schemes:
- description: 'API key from /admin/api-keys: Authorization: Bearer cef_<scope>_...'
  example_header: 'Authorization: Bearer cef_user_YOUR_KEY'
  key_format: cef_<scope>_...
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/craftingeventfinder-com-openapi.yml
  - https://craftingeventfinder.com/docs/mcp
  type: http
- description: Browser session cookie set after email magic-link / 6-digit code sign-in (POST /api/auth/login, /api/auth/verify-code per the spec; not called).
  in: cookie
  name: cookieAuth
  parameter: cef_session
  sources:
  - openapi/craftingeventfinder-com-openapi.yml
  type: apiKey
slug: craftingeventfinder-com-authentication
source_filename: craftingeventfinder-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://craftingeventfinder.com/docs/mcp\ndocs: https://craftingeventfinder.com/docs/mcp\nsummary:\n  types:\n  - apiKey\n  - http\n  api_key_in:\n  - cookie\n  - header\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'API key from /admin/api-keys: Authorization: Bearer cef_<scope>_...'\n  key_format: cef_<scope>_...\n  example_header: 'Authorization: Bearer cef_user_YOUR_KEY'\n  sources:\n  - openapi/craftingeventfinder-com-openapi.yml\n  - https://craftingeventfinder.com/docs/mcp\n- name: cookieAuth\n  type: apiKey\n  in: cookie\n  parameter: cef_session\n  description: Browser session cookie set after email magic-link / 6-digit code sign-in (POST /api/auth/login, /api/auth/verify-code per the spec; not called).\n  sources:\n  - openapi/craftingeventfinder-com-openapi.yml\nanonymous_access: 'Browse and search (no key needed)'\nkey_issuance: 'Account tools need a personal key. Ask us for one;\
  \ self-serve keys arrive with organizer accounts.'\nnote: Quotes are verbatim from https://craftingeventfinder.com/docs/mcp. No OAuth is documented, so no scopes file; the cef_<scope>_ key prefix encodes a key scope (cef_user_ shown in the docs).\n"
source_yaml_url: https://artifacts.apis.io/craftingeventfinder-com/authentication/craftingeventfinder-com-authentication.yml
summary_line: apiKey/http · 2 schemes
tags:
- Company
- Crafting
- Event
- Event Discovery
- Directory
- Quilting
- Knitting
- MCP
---
