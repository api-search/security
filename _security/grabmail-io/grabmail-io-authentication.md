---
anonymous_access: false
api_key_in: []
api_specs:
- filename: grabmail-io-account-api-openapi.yml
  format: yaml
  label: grabmail-io Account API
  slug: grabmail-io-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/grabmail-io/openapi/grabmail-io-account-api-openapi.yml
- filename: grabmail-io-mailbox-api-openapi.yml
  format: yaml
  label: grabmail-io Mailbox API
  slug: grabmail-io-mailbox-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/grabmail-io/openapi/grabmail-io-mailbox-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Grabmail Io Authentication
name_suffix: Authentication
oauth_flows: []
overview: grabmail-io secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: grabmail-io
provider_slug: grabmail-io
scheme_count: 1
schemes:
- description: 'An API key (gm_live_…), created at /account/keys — one on a free account, more on paid plans. A key has no tier of its own: each call is judged on its account''s current plan, and the same key moves with it. On the free plan it counts the free allowance per account instead of per IP address; on a paid plan it removes the per-minute and daily caps and opens the premium pool and the pool names in /ap'
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/grabmail-io.json
  type: http
slug: grabmail-io-authentication
source_filename: grabmail-io-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: derived\nsource: openapi/grabmail-io.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  description: 'An API key (gm_live_…), created at /account/keys — one on a free account, more\n    on paid plans. A key has no tier of its own: each call is judged on its account''s current\n    plan, and the same key moves with it. On the free plan it counts the free allowance per\n    account instead of per IP address; on a paid plan it removes the per-minute and daily caps\n    and opens the premium pool and the pool names in /ap'\n  sources:\n  - openapi/grabmail-io.json\n"
source_yaml_url: https://artifacts.apis.io/grabmail-io/authentication/grabmail-io-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Email
- Temporary
- API
- DeveloperTools
---
