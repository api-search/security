---
anonymous_access: false
api_key_in: []
api_specs:
- filename: cleat-so-lines-api-openapi.yml
  format: yaml
  label: Cleat Lines API
  slug: cleat-so-lines-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cleat-so/openapi/cleat-so-lines-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Cleat Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cleat secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Cleat
provider_slug: cleat-so
scheme_count: 1
schemes:
- description: 'An API key created in workspace settings, sent as `Authorization: Bearer clt_...`. Keys begin with `clt_` and are shown once.


    A key belongs to one workspace and is limited to 120 requests per minute. It can be narrowed further when it is created: to named lines (up to 50), and to a date it stops working, up to a year out — which is what makes a key safe to hand to an agent or a contractor. A line'
  name: apiKey
  scheme: bearer
  sources:
  - openapi/cleat-so-openapi.yml
  type: http
slug: cleat-so-authentication
source_filename: cleat-so-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://cleat.so/for/developers\nsummary:\n  types:\n  - http\nschemes:\n- name: apiKey\n  type: http\n  scheme: bearer\n  description: 'An API key created in workspace settings, sent as `Authorization: Bearer clt_...`. Keys begin with `clt_`\n    and are shown once.\n\n\n    A key belongs to one workspace and is limited to 120 requests per minute. It can be narrowed further when it is created:\n    to named lines (up to 50), and to a date it stops working, up to a year out — which is what makes a key safe to hand to\n    an agent or a contractor. A line'\n  sources:\n  - openapi/cleat-so-openapi.yml\ndocs: https://cleat.so/for/developers\nkey_prefix: clt_\nnotes:\n- Create an API key in Settings. It starts with clt_ and is shown once.\n- Only the workspace owner can create API keys and webhook endpoints, and a revoked key stops working immediately.\n- 'A key can also be narrowed when you create it: to named lines, and to a\
  \ date it stops working'\n- 'Webhooks are signed: cleat-signature header t=<unix seconds>,v1=<hex HMAC-SHA256 of \"t.body\"> keyed with the endpoint signing\n  secret (whsec_).'\n"
source_yaml_url: https://artifacts.apis.io/cleat-so/authentication/cleat-so-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- SMS
- Phone Numbers
- Verification Codes
- Two-Factor Authentication
- Webhook
- Telephony
---
