---
api_key_in: []
api_specs:
- filename: emulate-content-api-openapi.yml
  format: yaml
  label: Emulate Content REST API
  slug: content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/emulate/refs/heads/main/openapi/emulate-content-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
method: probed
name: Emulate Authentication
name_suffix: Authentication
oauth_flows: []
overview: Emulate declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Emulate
provider_slug: emulate
scheme_count: 0
schemes: []
slug: emulate-authentication
source_filename: emulate-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-01'\nmethod: probed\nsource: openapi/emulate-content-api-openapi.yml\nsummary:\n  types: []\n  api_key_in: []\n  oauth2_flows: []\n  note: >-\n    No authentication is required and none is offered. Every emulate-* namespace under\n    https://emulatebio.com/wp-json returned HTTP 200 with real JSON on an anonymous GET\n    with no credentials, no API key and no session cookie. The route index declares no\n    security requirement for these routes, and Emulate publishes no API key issuance,\n    OAuth client registration or developer account of any kind.\nschemes: []\nobserved:\n  anonymous_read: true\n  credentials_required: false\n  probes:\n  - url: https://emulatebio.com/wp-json/emulate-posts/v2/posts\n    headers_sent: none\n    http_status: 200\n  - url: https://emulatebio.com/wp-json/emulate-resources/v2/resources\n    headers_sent: none\n    http_status: 200\n  - url: https://emulatebio.com/wp-json/emulate-support/v2/support\n    headers_sent: none\n\
  \    http_status: 200\n  discovery:\n  - path: /.well-known/openid-configuration\n    status: 404\n  - path: /.well-known/oauth-authorization-server\n    status: 404\nwrite_surface:\n  present: false\n  note: >-\n    Only GET is registered on the emulate-* routes. WordPress core write routes under\n    /wp-json/wp/v2/ exist but require an authenticated WordPress user; the site's\n    /login/ page is the WordPress administrative login, not a customer or developer\n    sign-up, so no SignUp/Login pointer is claimed in apis.yml.\nx-evidence:\n  fetched: '2026-08-01'\n  url: https://emulatebio.com/wp-json/\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/emulate/refs/heads/main/authentication/emulate-authentication.yml
summary_line: 0 schemes
tags:
- Company
- Biotechnology
- Life Sciences
- Organ-on-a-Chip
- Drug Discovery
- Preclinical Research
- Toxicology
- Laboratory Instruments
- In Vitro Models
- Scientific Software
---
