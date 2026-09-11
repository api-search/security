---
anonymous_access: false
api_key_in: []
api_specs:
- filename: federal-mediation-and-conciliation-service-wp-content-openapi.yml
  format: yaml
  label: FMCS Public Content API
  slug: fmcs-public-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/federal-mediation-and-conciliation-service/refs/heads/main/openapi/federal-mediation-and-conciliation-service-wp-content-openapi.yml
auth_types:
- none
description: ''
kind: authentication
layout: security
mechanism_count: 0
method: probed
name: Federal Mediation And Conciliation Service Authentication
name_suffix: Authentication
oauth_flows: []
overview: Federal Mediation and Conciliation Service secures its APIs with none across 0 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Federal Mediation and Conciliation Service
provider_slug: federal-mediation-and-conciliation-service
scheme_count: 0
schemes: []
slug: federal-mediation-and-conciliation-service-authentication
source_filename: federal-mediation-and-conciliation-service-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-09'\nmethod: probed\nsource: >-\n  openapi/federal-mediation-and-conciliation-service-wp-content-openapi.yml plus live anonymous probes of\n  https://www.fmcs.gov/wp-json/ (2026-09-09)\nsummary:\n  types: [none]\n  api_key_in: []\n  oauth2_flows: []\n  public_read: true\n  note: >-\n    The catalogued surface requires no authentication at all. All 31 operations in the derived OpenAPI were\n    called with no credential and returned HTTP 200 on 2026-09-09. FMCS issues no API keys, runs no developer\n    signup and publishes no authentication documentation, because it publishes no developer programme.\nschemes: []\npublic_surface:\n  scheme: none\n  evidence:\n    - {url: 'https://www.fmcs.gov/wp-json/', status: 200, note: 'route discovery document, 1,020 routes, no credential'}\n    - {url: 'https://www.fmcs.gov/wp-json/wp/v2/posts?per_page=1', status: 200, note: 'JSON returned with no Authorization header'}\n    - {url: 'https://www.fmcs.gov/wp-json/wp/v2/media?per_page=1',\
  \ status: 200}\n    - {url: 'https://www.fmcs.gov/wp-json/wp/v2/wpbdp_listing?per_page=1', status: 200}\ngated_surface:\n  note: >-\n    The same host advertises an authenticated write and administrative surface that is NOT part of the public\n    API and is not modelled in the OpenAPI. The route index declares WordPress Application Passwords as the\n    site's authentication mechanism, and anonymous callers are refused on every administrative route.\n  schemes_advertised_by_platform:\n    - name: WordPress Application Passwords\n      type: http\n      scheme: basic\n      authorization_endpoint: https://www.fmcs.gov/wp-admin/authorize-application.php\n      note: >-\n        Declared verbatim in the route discovery document under `authentication`. This is a WordPress\n        site-administrator mechanism, not a developer credential FMCS issues to the public.\n    - name: Cookie + X-WP-Nonce\n      type: apiKey\n      in: header\n      parameter: X-WP-Nonce\n      note: Advertised in\
  \ Access-Control-Allow-Headers on every response.\n  evidence:\n    - {url: 'https://www.fmcs.gov/wp-json/wp/v2/settings', status: 401, body: '{\"code\":\"rest_forbidden\",\"message\":\"Sorry, you are not allowed to do that.\",\"data\":{\"status\":401}}'}\n    - {url: 'https://www.fmcs.gov/wp-json/wp/v2/block-types', status: 401, note: 'rest_forbidden'}\n    - {url: 'https://www.fmcs.gov/wp-json/wp/v2/comments', status: 403, body: '{\"code\":\"rest_comment_disabled\",\"message\":\"Comments are disabled.\",\"data\":{\"status\":403}}'}\n    - {header: 'Allow: GET', note: 'Collection responses advertise GET only for an anonymous caller'}\n    - {header: 'Access-Control-Allow-Headers: Authorization, X-WP-Nonce, Content-Disposition, Content-MD5, Content-Type'}\nseparate_gated_systems:\n  note: >-\n    FMCS operates two login-gated case systems on separate hosts. Neither publishes a machine-readable\n    contract, neither is part of the API catalogued here, and no credential is issued to developers.\n\
  \  systems:\n    - {name: FMCS Arbitration System, url: 'https://arbitration.fmcs.gov/', status: 200, landing: 'https://arbitration.fmcs.gov/login.aspx', note: 'ASP.NET WebForms login; arbitration panel requests and case management'}\n    - {name: F-7 notice online filing, url: 'https://www.fmcs.gov/resources/documents-and-data/filing_an_f-7_online/', status: 200, note: 'Since 5 April 2022 F-7 notices may only be filed through the online portal; the portal itself is account-gated'}\ndocs: null\ndocs_note: >-\n  FMCS publishes no authentication documentation. The upstream platform reference is\n  https://developer.wordpress.org/rest-api/using-the-rest-api/authentication/ — WordPress's, not FMCS's.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/federal-mediation-and-conciliation-service/refs/heads/main/authentication/federal-mediation-and-conciliation-service-authentication.yml
summary_line: none · 0 schemes
tags:
- Federal-Government
- Labor
- Mediation
- Arbitration
- Dispute-Resolution
- Government
- Public-Sector
- Content
---
