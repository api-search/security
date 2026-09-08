---
anonymous_access: true
api_key_in: []
api_specs:
- filename: department-of-state-state-gov-content-openapi.yml
  format: yaml
  label: state.gov Content API
  slug: state-gov-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/department-of-state/refs/heads/main/openapi/department-of-state-state-gov-content-openapi.yml
auth_types:
- none
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Department Of State Authentication
name_suffix: Authentication
oauth_flows: []
overview: Department of State secures its APIs with none and http across 2 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Department of State
provider_slug: department-of-state
scheme_count: 2
schemes:
- applies_to: All 65 read operations on https://www.state.gov/wp-json, all four Office of the Historian OPDS catalog operations, and the travel advisory RSS feed.
  evidence: Live anonymous GETs returning 200 on 2026-09-07 against https://www.state.gov/wp-json/wp/v2/state_press_release, https://history.state.gov/api/v1/catalog and https://travel.state.gov/_res/rss/TAsTWs.xml.
  name: none
  type: none
- applies_to: The 93 write operations (create, update, delete) across every content type and taxonomy.
  availability: internal-only
  description: WordPress Application Passwords. Advertised by the Department at https://www.state.gov/wp-json/ under authentication.application-passwords, authorization endpoint https://www.state.gov/wp-admin/authorize-application.php.
  name: applicationPassword
  scheme: basic
  sources:
  - openapi/department-of-state-state-gov-content-openapi.yml
  - https://www.state.gov/wp-json/
  type: http
slug: department-of-state-authentication
source_filename: department-of-state-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-07'\nmethod: searched\nsource: openapi/department-of-state-state-gov-content-openapi.yml\ndocs: https://www.state.gov/wp-json/\nsummary:\n  types:\n    - none\n    - http\n  public_read_auth: none\n  api_key_required: false\n  registration_required: false\n  oauth2_flows: []\n  api_key_in: []\nnote: >-\n  The defining fact about authentication at the Department of State is that there is none to obtain.\n  Every public surface found in this repo — the 65 read operations of the state.gov Content API, the\n  Office of the Historian OPDS Ebook Catalog API, the Travel Advisories RSS feed and the DCAT-US open\n  data catalog — is served anonymously over HTTPS with no key, no token, no registration and no\n  quota. There is no developer portal to sign up at and no credential to issue.\n  The one credential the contract names is internal: HTTP Basic with a WordPress Application\n  Password, which gates the 93 write operations. The Department advertises it itself\
  \ in the route\n  index, so it is recorded here for completeness, but it is issued to Department editorial accounts\n  and is not obtainable by the public at any price.\nschemes:\n  - name: none\n    type: none\n    applies_to: >-\n      All 65 read operations on https://www.state.gov/wp-json, all four Office of the Historian OPDS\n      catalog operations, and the travel advisory RSS feed.\n    evidence: >-\n      Live anonymous GETs returning 200 on 2026-09-07 against\n      https://www.state.gov/wp-json/wp/v2/state_press_release,\n      https://history.state.gov/api/v1/catalog and\n      https://travel.state.gov/_res/rss/TAsTWs.xml.\n  - name: applicationPassword\n    type: http\n    scheme: basic\n    description: >-\n      WordPress Application Passwords. Advertised by the Department at https://www.state.gov/wp-json/\n      under authentication.application-passwords, authorization endpoint\n      https://www.state.gov/wp-admin/authorize-application.php.\n    applies_to: The 93 write\
  \ operations (create, update, delete) across every content type and taxonomy.\n    availability: internal-only\n    sources:\n      - openapi/department-of-state-state-gov-content-openapi.yml\n      - https://www.state.gov/wp-json/\ndiscovery_documents_absent:\n  - path: /.well-known/openid-configuration\n    result: 404 or unreachable on all nine State hosts probed\n  - path: /.well-known/oauth-authorization-server\n    result: 404 or unreachable on all nine State hosts probed\n  - path: /.well-known/oauth-protected-resource\n    result: 404 or unreachable on all nine State hosts probed\ndiscovery_probe_record: well-known/department-of-state-well-known.yml\nedge_controls:\n  note: >-\n    Authorization is not the only thing standing between a client and the data. travel.state.gov,\n    step.state.gov and cadatacatalog.state.gov answer non-browser clients with a Cloudflare 403\n    challenge, and https://www.state.gov/wp-json/wp/v2/users is blocked at the edge. These are bot\n    policies,\
  \ not authentication — no credential exists that would clear them.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/department-of-state/refs/heads/main/authentication/department-of-state-authentication.yml
summary_line: none/http · 2 schemes
tags:
- Federal-Government
- Foreign Affairs
- Travel
- Consular
- Visas
- Passports
---
