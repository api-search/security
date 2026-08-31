---
api_key_in: []
api_specs:
- filename: electra.aero-news-api-openapi.yml
  format: yaml
  label: Electra.aero News API
  slug: electra.aero-news-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/electra.aero/refs/heads/main/openapi/electra.aero-news-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: Electra.Aero Authentication
name_suffix: Authentication
oauth_flows: []
overview: Electra.aero declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Electra.aero
provider_slug: electra.aero
scheme_count: 0
schemes: []
slug: electra.aero-authentication
source_filename: electra.aero-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: probed\nsource: openapi/electra.aero-content-openapi.yml\ndocs: null\nsummary:\n  types: []\n  api_key_in: []\n  oauth2_flows: []\n  model: none-required\n  public_read: true\nnote: >-\n  The Electra.aero content API is fully anonymous. Verified by probe on 2026-08-12 - GET\n  https://electra.aero/api/collections/news/entries returns HTTP 200 application/json with\n  no Authorization header, no API key, no cookie and no CORS restriction\n  (access-control-allow-origin: *). The OpenAPI derived from those probes therefore declares\n  components.securitySchemes as empty and security as [] at both document and operation level.\n  There is no credential to obtain because Electra publishes no developer program, no\n  sign-up, and no key issuance. /.well-known/openid-configuration and\n  /.well-known/oauth-authorization-server both 404.\nschemes: []\nwrite_surface:\n  authenticated: unknown\n  note: >-\n    Only GET operations were probed. Statamic's\
  \ control panel at /cp is the write surface\n    and is provider-internal; no anonymous write was attempted and none is documented.\nx-evidence:\n  - url: https://electra.aero/api/collections/news/entries?limit=1\n    http_status: 200\n    auth_sent: none\n    fetched: '2026-08-12'\n  - url: https://electra.aero/.well-known/openid-configuration\n    http_status: 404\n    fetched: '2026-08-12'\n  - url: https://electra.aero/.well-known/oauth-authorization-server\n    http_status: 404\n    fetched: '2026-08-12'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/electra.aero/refs/heads/main/authentication/electra.aero-authentication.yml
summary_line: 0 schemes
tags:
- Aerospace
- Aviation
- Aircraft Manufacturing
- Advanced Air Mobility
- Electric Aviation
- Hybrid-Electric Propulsion
- Regional Air Mobility
- Defense
- Transportation
- Content
- Company
---
