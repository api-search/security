---
anonymous_access: false
api_key_in: []
api_specs:
- filename: workwae-com-v1-openapi.json
  format: json
  label: Workwae API V1 API
  slug: workwae-api-v1-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/workwae-com/openapi/_original/workwae-com-v1-openapi.json
auth_types: []
description: Authentication methods as published on the Workwae API reference page.
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: workwae-com Authentication
name_suffix: Authentication
oauth_flows: []
overview: workwae-com declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: workwae-com
provider_slug: workwae-com
scheme_count: 2
schemes:
- evidence: 'Send Authorization: Bearer <credential> with one of:'
  header: Authorization
  how_to_obtain: Use an API key that starts with wk_… and has the read, write, send or admin scope.
  location: header
  name: API key
  type: http-bearer
- evidence: 'Send Authorization: Bearer <credential> with one of:'
  header: Authorization
  how_to_obtain: Use an account token that starts with wat_…; it is short‑lived and acts with every scope on one account.
  location: header
  name: Account token
  type: http-bearer
slug: workwae-com-authentication
source_filename: workwae-com-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.workwae.com/reference/oauth-apps
source_yaml: "generated: '2026-10-31'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.workwae.com/reference/oauth-apps\nsources:\n- https://docs.workwae.com/reference/oauth-apps\n- https://docs.workwae.com/reference\ndescription: Authentication methods as published on the Workwae API reference page.\nschemes:\n- type: http-bearer\n  name: API key\n  evidence: 'Send Authorization: Bearer <credential> with one of:'\n  location: header\n  header: Authorization\n  how_to_obtain: Use an API key that starts with wk_… and has the read, write, send or admin scope.\n- type: http-bearer\n  name: Account token\n  evidence: 'Send Authorization: Bearer <credential> with one of:'\n  location: header\n  header: Authorization\n  how_to_obtain: Use an account token that starts with wat_…; it is short‑lived and acts with every scope on one account.\nnote: No OAuth2 flows are described on the referenced pages.\ndocs: https://docs.workwae.com/reference/oauth-apps\n"
source_yaml_url: https://artifacts.apis.io/workwae-com/authentication/workwae-com-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Email
- Calendar
- Contacts
- Scheduling
- Artificial Intelligence
---
