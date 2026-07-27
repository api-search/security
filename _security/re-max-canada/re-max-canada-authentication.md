---
api_key_in: []
api_specs:
- filename: re-max-canada-blog-wp-json-index.json
  format: json
  label: RE/MAX Canada Blog WordPress REST API
  slug: re-max-canada-blog-wordpress-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/re-max-canada/refs/heads/main/openapi/re-max-canada-blog-wp-json-index.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: Re Max Canada Authentication
name_suffix: Authentication
oauth_flows: []
overview: RE/MAX Canada secures its APIs with http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: RE/MAX Canada
provider_slug: re-max-canada
scheme_count: 3
schemes:
- applies_to: The wp/v2 content namespace on blog.remax.ca, join.remax.ca, franchise.remax.ca and agentbrokerhub.remax.ca. Confirmed live with GET /wp-json/wp/v2/posts?per_page=1 (HTTP 200) and GET /wp-json/wp/v2/users (HTTP 200) with no credential of any kind.
  name: anonymous
  sources:
  - openapi/re-max-canada-blog-wp-json-index.json
  type: none
- authorization_endpoint: https://blog.remax.ca/wp-admin/authorize-application.php
  description: 'WordPress Application Passwords. Declared verbatim by the harvested discovery index as {"application-passwords":{"endpoints":{"authorization":"https://blog.remax.ca/wp-admin/authorize-application.php"}}}. A credential is minted inside wp-admin by an already-authenticated WordPress user and then sent as HTTP Basic (username + application password) on subsequent REST calls. This is a CMS staff-login mechanism supplied by the hosting platform, NOT a developer onboarding path: there is no self-serve signup, no key-request form, no application review and no published terms governing it.'
  name: application-passwords
  scheme: basic
  self_serve: false
  sources:
  - openapi/re-max-canada-blog-wp-json-index.json
  standard: RFC 7617 HTTP Basic over TLS
  type: http
- description: The WordPress core first-party scheme for logged-in browser sessions. Listed for completeness because it is inherent to every WordPress REST install; it is not usable by a third-party integrator and it is not advertised in the discovery index's authentication block.
  in: header
  name: cookie-plus-nonce
  parameter_name: X-WP-Nonce
  self_serve: false
  sources:
  - WordPress core behaviour (not asserted by the provider)
  type: apiKey
slug: re-max-canada-authentication
source_filename: re-max-canada-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-26'\nmethod: searched\nsource: >-\n  openapi/re-max-canada-blog-wp-json-index.json (harvested WordPress REST\n  discovery index, HTTP 200, 2026-07-26) plus live anonymous probes of\n  https://blog.remax.ca/wp-json/\ndocs: https://blog.remax.ca/wp-admin/authorize-application.php\nsummary:\n  types:\n  - http\n  api_key_in: []\n  oauth2_flows: []\n  anonymous_read: true\n  developer_onboarding: none-published\nproduct_api_auth: >-\n  None. RE/MAX Canada operates no product API, so there is no authentication\n  model for listings, agents, offices, valuations or transactions. Nothing was\n  invented to fill this section.\nschemes:\n- name: anonymous\n  type: none\n  applies_to: >-\n    The wp/v2 content namespace on blog.remax.ca, join.remax.ca,\n    franchise.remax.ca and agentbrokerhub.remax.ca. Confirmed live with GET\n    /wp-json/wp/v2/posts?per_page=1 (HTTP 200) and GET /wp-json/wp/v2/users\n    (HTTP 200) with no credential of any kind.\n  sources:\n\
  \  - openapi/re-max-canada-blog-wp-json-index.json\n- name: application-passwords\n  type: http\n  scheme: basic\n  standard: RFC 7617 HTTP Basic over TLS\n  description: >-\n    WordPress Application Passwords. Declared verbatim by the harvested\n    discovery index as\n    {\"application-passwords\":{\"endpoints\":{\"authorization\":\"https://blog.remax.ca/wp-admin/authorize-application.php\"}}}.\n    A credential is minted inside wp-admin by an already-authenticated WordPress\n    user and then sent as HTTP Basic (username + application password) on\n    subsequent REST calls. This is a CMS staff-login mechanism supplied by the\n    hosting platform, NOT a developer onboarding path: there is no self-serve\n    signup, no key-request form, no application review and no published terms\n    governing it.\n  authorization_endpoint: https://blog.remax.ca/wp-admin/authorize-application.php\n  self_serve: false\n  sources:\n  - openapi/re-max-canada-blog-wp-json-index.json\n- name: cookie-plus-nonce\n\
  \  type: apiKey\n  in: header\n  parameter_name: X-WP-Nonce\n  description: >-\n    The WordPress core first-party scheme for logged-in browser sessions. Listed\n    for completeness because it is inherent to every WordPress REST install; it\n    is not usable by a third-party integrator and it is not advertised in the\n    discovery index's authentication block.\n  self_serve: false\n  sources:\n  - WordPress core behaviour (not asserted by the provider)\nobserved_behaviour:\n- probe: GET https://blog.remax.ca/wp-json/wp/v2/settings\n  status: 401\n  body: '{\"code\":\"rest_forbidden\",\"message\":\"Sorry, you are not allowed to do that.\",\"data\":{\"status\":401}}'\n  note: >-\n    Authenticated-only routes reject anonymous callers with the WordPress\n    rest_forbidden envelope carrying HTTP 401 — no WWW-Authenticate challenge is\n    returned, so there is no discoverable auth negotiation.\n- probe: GET https://blog.remax.ca/wp-json/wp/v2/posts?per_page=1\n  status: 200\n  note: Content\
  \ routes read anonymously; CORS is Access-Control-Allow-Origin *.\nnegative_findings:\n  oauth2: >-\n    None documented and none discoverable.\n    /.well-known/oauth-authorization-server returns 404 on every host.\n  openid_connect: >-\n    None. /.well-known/openid-configuration returns 404 on blog.remax.ca,\n    join.remax.ca, franchise.remax.ca and www.remax.ca.\n  api_keys: None issued or documented by RE/MAX Canada.\n  mutual_tls: None documented.\n  scopes: >-\n    No scope vocabulary exists. WordPress authorizes by user capability, not by\n    OAuth scope, so scopes/ is deliberately NOT emitted for this provider.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/re-max-canada/refs/heads/main/authentication/re-max-canada-authentication.yml
summary_line: http · 3 schemes
tags:
- Real Estate
- Canada
- Brokerage
- Property Listings
- MLS
- RESO
- IDX
- PropTech
- Land Registry
- Valuation
- Rentals
- Franchising
---
