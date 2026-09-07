---
anonymous_access: true
api_key_in: []
api_specs:
- filename: consol-energy-mines-content-api-openapi.yml
  format: yaml
  label: Core Natural Resources Mines Content API
  slug: mines-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/consol-energy/refs/heads/main/openapi/consol-energy-mines-content-api-openapi.yml
- filename: consol-energy-leadership-content-api-openapi.yml
  format: yaml
  label: Core Natural Resources Leadership Content API
  slug: leadership-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/consol-energy/refs/heads/main/openapi/consol-energy-leadership-content-api-openapi.yml
- filename: consol-energy-news-content-api-openapi.yml
  format: yaml
  label: Core Natural Resources News Content API
  slug: news-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/consol-energy/refs/heads/main/openapi/consol-energy-news-content-api-openapi.yml
- filename: consol-energy-site-content-api-openapi.yml
  format: yaml
  label: Core Natural Resources Site Content API
  slug: site-content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/consol-energy/refs/heads/main/openapi/consol-energy-site-content-api-openapi.yml
- filename: consol-energy-discovery-api-openapi.yml
  format: yaml
  label: Core Natural Resources Discovery API
  slug: discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/consol-energy/refs/heads/main/openapi/consol-energy-discovery-api-openapi.yml
auth_types:
- none
- cookie-nonce
- http-basic
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: probed
name: Consol Energy Authentication
name_suffix: Authentication
oauth_flows: []
overview: CONSOL Energy secures its APIs with none, cookie-nonce, and http-basic across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: CONSOL Energy
provider_slug: consol-energy
scheme_count: 3
schemes:
- applies_to: every GET operation in openapi/consol-energy-*-openapi.yml
  description: Public read access. No API key, no token, no account. The company publishes no developer portal, no sign-up and no key issuance of any kind.
  name: anonymous
  sources:
  - https://corenaturalresources.com/wp-json/
  type: none
- applies_to: write methods and administrative routes (not catalogued here)
  description: WordPress' first-party session auth for logged-in editors. Advertised by the host in its CORS preflight allow-list (Access-Control-Allow-Headers includes X-WP-Nonce, observed 2026-09-05). Applies to write methods and the administrative namespaces only.
  in: header
  name: wordpress-cookie-nonce
  parameter_name: X-WP-Nonce
  type: apiKey
- applies_to: write methods and administrative routes (not catalogued here)
  description: WordPress Application Passwords over HTTP Basic, the standard machine credential for the WordPress REST API. The route /wp/v2/users/{id}/application-passwords is registered on this host. Issued by site administrators; not available to the public.
  name: wordpress-application-passwords
  scheme: basic
  type: http
slug: consol-energy-authentication
source_filename: consol-energy-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-05'\nmethod: probed\nsource: https://corenaturalresources.com/wp-json/\ndocs: null\nsummary:\n  types: [none, cookie-nonce, http-basic]\n  api_key_in: []\n  oauth2_flows: []\n  public_read: true\n  note: >-\n    The read surface this profile catalogs requires NO authentication: every\n    endpoint in openapi/ returned HTTP 200 to an anonymous GET on 2026-09-05,\n    and the route discovery document reports an empty \"authentication\" array.\n    The write and administrative surface is authenticated by WordPress core\n    mechanisms, which the company documents nowhere; it was established by\n    probe, not by reading a docs page.\nschemes:\n  - name: anonymous\n    type: none\n    description: >-\n      Public read access. No API key, no token, no account. The company\n      publishes no developer portal, no sign-up and no key issuance of any kind.\n    applies_to: every GET operation in openapi/consol-energy-*-openapi.yml\n    sources: [https://corenaturalresources.com/wp-json/]\n\
  \  - name: wordpress-cookie-nonce\n    type: apiKey\n    in: header\n    parameter_name: X-WP-Nonce\n    description: >-\n      WordPress' first-party session auth for logged-in editors. Advertised by\n      the host in its CORS preflight allow-list (Access-Control-Allow-Headers\n      includes X-WP-Nonce, observed 2026-09-05). Applies to write methods and\n      the administrative namespaces only.\n    applies_to: write methods and administrative routes (not catalogued here)\n  - name: wordpress-application-passwords\n    type: http\n    scheme: basic\n    description: >-\n      WordPress Application Passwords over HTTP Basic, the standard machine\n      credential for the WordPress REST API. The route\n      /wp/v2/users/{id}/application-passwords is registered on this host.\n      Issued by site administrators; not available to the public.\n    applies_to: write methods and administrative routes (not catalogued here)\nevidence:\n  - url: https://corenaturalresources.com/wp-json/wp/v2/mine\n\
  \    status: 200\n    note: anonymous GET succeeded\n  - url: https://corenaturalresources.com/wp-json/wp/v2/users\n    status: 401\n    body: '{\"code\":\"rest_user_cannot_view\",\"message\":\"Sorry, you are not allowed to list users.\",\"data\":{\"status\":401}}'\n  - url: https://corenaturalresources.com/wp-json/wp/v2/settings\n    status: 401\n    body: '{\"code\":\"rest_forbidden\",\"message\":\"Sorry, you are not allowed to do that.\",\"data\":{\"status\":401}}'\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/consol-energy/refs/heads/main/authentication/consol-energy-authentication.yml
summary_line: none/cookie-nonce/http-basic · 3 schemes
tags:
- Bituminous Coal
- Coal Mining
- Core Natural Resources
- Energy
- Investor Relations
- Mining
- Suppliers
- Sustainability
- Fortune 1000
---
