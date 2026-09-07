---
anonymous_access: true
api_key_in: []
auth_types:
- none
- application-password
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Clorox Authentication
name_suffix: Authentication
oauth_flows: []
overview: The Clorox Company secures its APIs with none and application-password across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: The Clorox Company
provider_slug: clorox
scheme_count: 2
schemes:
- applies_to: every first-party read route in tcc/v1 and clorox-security/v1
  evidence: GET /tcc/v1/sds-xml (200, 113549 bytes), /tcc/v1/cleaning_labels (200, 13410 bytes) and /tcc/v1/job-search/job-query (200, 41159 bytes) all returned real data with no credential of any kind on 2026-09-05.
  name: anonymous
  type: none
- audience: cms-editors
  authorization_endpoint: https://www.thecloroxcompany.com/wp-admin/authorize-application.php
  name: wordpress-application-passwords
  note: This is the only mechanism the discovery document advertises. It authenticates WordPress users for editorial writes; it is not an API-consumer credential and there is no public route to obtain one.
  scheme: basic
  source: contracts/clorox-wp-json-root.json
  type: http
slug: clorox-authentication
source_filename: clorox-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: derived\nsource: contracts/clorox-wp-json-root.json (authentication block) + anonymous live calls\nsummary:\n  types: [none, application-password]\n  api_key_in: []\n  oauth2_flows: []\n  public_read: true\n  self_service_credentials: false\nschemes:\n  - name: anonymous\n    type: none\n    applies_to: \"every first-party read route in tcc/v1 and clorox-security/v1\"\n    evidence: >-\n      GET /tcc/v1/sds-xml (200, 113549 bytes), /tcc/v1/cleaning_labels (200, 13410 bytes) and\n      /tcc/v1/job-search/job-query (200, 41159 bytes) all returned real data with no\n      credential of any kind on 2026-09-05.\n  - name: wordpress-application-passwords\n    type: http\n    scheme: basic\n    authorization_endpoint: https://www.thecloroxcompany.com/wp-admin/authorize-application.php\n    source: contracts/clorox-wp-json-root.json\n    audience: cms-editors\n    note: >-\n      This is the only mechanism the discovery document advertises. It authenticates\
  \ WordPress\n      users for editorial writes; it is not an API-consumer credential and there is no public\n      route to obtain one.\ngated_surfaces:\n  - host: api.clorox.com\n    mechanism: unknown\n    evidence: \"HTTP 403 at the gateway root; no /.well-known/oauth-authorization-server, no /.well-known/openid-configuration (both 404).\"\n    note: >-\n      MuleSoft Anypoint gateway. Clorox has an ENABLED Anypoint Exchange public portal at\n      https://anypoint.mulesoft.com/exchange/portals/clorox/ but it publishes zero assets, so\n      the gateway's auth model is not discoverable anonymously.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/clorox/refs/heads/main/authentication/clorox-authentication.yml
summary_line: none/application-password · 2 schemes
tags:
- Cleaning Products
- Consumer Goods
- CPG
- Disinfectants
- Household Products
- Manufacturer
- Fortune 500
- Safety Data Sheets
- Product Transparency
- MuleSoft
---
