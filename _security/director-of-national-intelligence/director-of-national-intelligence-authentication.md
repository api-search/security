---
anonymous_access: false
api_key_in: []
api_specs:
- filename: director-of-national-intelligence-wp-content-openapi.yml
  format: yaml
  label: ODNI Public Content API
  slug: odni-public-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/director-of-national-intelligence/refs/heads/main/openapi/director-of-national-intelligence-wp-content-openapi.yml
auth_types:
- none
description: ''
kind: authentication
layout: security
mechanism_count: 0
method: probed
name: Director Of National Intelligence Authentication
name_suffix: Authentication
oauth_flows: []
overview: Director of National Intelligence secures its APIs with none across 0 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Director of National Intelligence
provider_slug: director-of-national-intelligence
scheme_count: 0
schemes: []
slug: director-of-national-intelligence-authentication
source_filename: director-of-national-intelligence-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-06'\nmethod: probed\nsource: openapi/director-of-national-intelligence-wp-content-openapi.yml + live anonymous probes of https://www.odni.gov/?rest_route=/\nsummary:\n  types: [none]\n  api_key_in: []\n  oauth2_flows: []\n  public_read: true\n  note: >-\n    The catalogued surface requires no authentication at all. Every operation in the derived OpenAPI was\n    called with no credential and returned HTTP 200 on 2026-09-06. ODNI issues no API keys, runs no\n    developer signup, and publishes no authentication documentation, because it publishes no developer\n    program.\nschemes: []\npublic_surface:\n  scheme: none\n  evidence:\n    - {url: 'https://www.odni.gov/?rest_route=/wp/v2/posts&per_page=3', status: 200, note: 'JSON returned with no Authorization header'}\n    - {url: 'https://www.odni.gov/?rest_route=/wp/v2/dlm_download&per_page=3', status: 200}\n    - {url: 'https://www.odni.gov/?rest_route=/', status: 200, note: 'route discovery document, 205\
  \ routes'}\ngated_surface:\n  note: >-\n    The same host advertises an authenticated write/administrative surface that is NOT part of the public\n    API and is not modelled in the OpenAPI. WordPress core supports Application Passwords (HTTP Basic over\n    TLS) and cookie authentication with an X-WP-Nonce header; the route index exposes\n    /wp/v2/users/{id}/application-passwords. Anonymous callers are refused.\n  schemes_advertised_by_platform:\n    - {name: WordPress Application Passwords, type: http, scheme: basic, note: 'WordPress core mechanism; not documented or offered to the public by ODNI'}\n    - {name: Cookie + X-WP-Nonce, type: apiKey, in: header, parameter: X-WP-Nonce, note: 'Advertised in Access-Control-Allow-Headers on every response'}\n  evidence:\n    - {url: 'https://www.odni.gov/?rest_route=/wp/v2/settings', status: 401, body: '{\"code\":\"rest_forbidden\",\"message\":\"Sorry, you are not allowed to do that.\",\"data\":{\"status\":401}}'}\n    - {header: 'Allow: GET',\
  \ note: 'Collection responses advertise GET only for an anonymous caller'}\n    - {header: 'Access-Control-Allow-Headers: Authorization, X-WP-Nonce, Content-Disposition, Content-MD5, Content-Type'}\ndocs: null\ndocs_note: >-\n  ODNI publishes no authentication documentation. The upstream platform reference is\n  https://developer.wordpress.org/rest-api/using-the-rest-api/authentication/ — WordPress's, not ODNI's.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/director-of-national-intelligence/refs/heads/main/authentication/director-of-national-intelligence-authentication.yml
summary_line: none · 0 schemes
tags:
- Federal-Government
- Intelligence
- National-Security
- Government
- Public-Sector
- Transparency
- News
- Publications
---
