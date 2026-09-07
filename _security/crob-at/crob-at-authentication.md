---
anonymous_access: true
api_key_in:
- cookie
api_specs:
- filename: crob-at-openapi.json
  format: json
  label: crob.at REST API
  slug: crobat-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/crob-at/refs/heads/main/openapi/crob-at-openapi.json
auth_types:
- none
- apiKey
description: Public endpoints are anonymous and keyless — the OpenAPI declares top-level security [] and the docs state no account, API key, or payment method is required. Two same-origin helper endpoints (getCurrentUser, createShowdownAssertion) use the crob.at browser session cookie; the onboarding document is explicit that the session cookie is for same-origin browser flows and is not an API key, and the docs warn never to send it to another origin or embed it in client code.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Crob At Authentication
name_suffix: Authentication
oauth_flows: []
overview: crob.at secures its APIs with none and apiKey across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: crob.at
provider_slug: crob-at
scheme_count: 2
schemes:
- description: No authentication required for public team, generation, reference and feedback endpoints.
  name: public
  sources:
  - https://crob.at/.well-known/api-onboarding
  type: none
- description: Optional crob.at browser session cookie for account helpers (/api/me, /api/showdown/assertion). Bootstrap by signing in at https://crob.at/login; acts only on the signed-in account.
  in: cookie
  name: cookieSession
  parameter: session
  sources:
  - openapi/crob-at-openapi.json
  - https://crob.at/.well-known/api-onboarding
  type: apiKey
slug: crob-at-authentication
source_filename: crob-at-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-03'\nmethod: searched\nsource: openapi/crob-at-openapi.json + https://crob.at/api#security + https://crob.at/.well-known/api-onboarding\ndocs: https://crob.at/api#security\nsummary:\n  types:\n  - none\n  - apiKey\n  api_key_in:\n  - cookie\ndescription: >-\n  Public endpoints are anonymous and keyless — the OpenAPI declares top-level\n  security [] and the docs state no account, API key, or payment method is\n  required. Two same-origin helper endpoints (getCurrentUser,\n  createShowdownAssertion) use the crob.at browser session cookie; the\n  onboarding document is explicit that the session cookie is for same-origin\n  browser flows and is not an API key, and the docs warn never to send it to\n  another origin or embed it in client code.\nschemes:\n- name: public\n  type: none\n  description: No authentication required for public team, generation, reference and feedback endpoints.\n  sources:\n  - https://crob.at/.well-known/api-onboarding\n- name: cookieSession\n\
  \  type: apiKey\n  in: cookie\n  parameter: session\n  description: >-\n    Optional crob.at browser session cookie for account helpers (/api/me,\n    /api/showdown/assertion). Bootstrap by signing in at https://crob.at/login;\n    acts only on the signed-in account.\n  sources:\n  - openapi/crob-at-openapi.json\n  - https://crob.at/.well-known/api-onboarding\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/crob-at/refs/heads/main/authentication/crob-at-authentication.yml
summary_line: none/apiKey · 2 schemes
tags:
- Gaming
- Esports
- Pokemon
- Pokemon Showdown
- Team Building
- Content Rendering
- Developer Tools
- REST API
---
