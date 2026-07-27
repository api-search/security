---
api_key_in: []
api_specs:
- filename: wahi-listing-search-openapi.yaml
  format: yaml
  label: Wahi Listing Search API
  slug: wahi-listing-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wahi/refs/heads/main/openapi/wahi-listing-search-openapi.yaml
auth_types:
- none
- http-basic
- cookie
description: ''
kind: authentication
layout: security
method: searched
name: Wahi Authentication
name_suffix: Authentication
oauth_flows: []
overview: Wahi secures its APIs with none, http-basic, and cookie across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Wahi
provider_slug: wahi
scheme_count: 3
schemes:
- api: openapi/wahi-listing-search-openapi.yaml
  applies_to:
  - searchListings
  evidence: 'The published OpenAPI 3.0.1 contains no components.securitySchemes and no security[] requirement on /search. https://wahi.com/.well-known/ai-plugin.json declares "auth": {"type": "none"} and "is_user_authenticated": false.'
  name: none
  type: none
- api: openapi/wahi-wp-json-discovery.json
  authorization_endpoint: https://wahi.com/wp-admin/authorize-application.php
  evidence: The wp-json discovery document declares authentication.application-passwords.endpoints.authorization. WordPress application passwords are HTTP Basic credentials minted per user inside wp-admin; anonymous reads on /wp-json/wp/v2/* need no credential, writes need one.
  name: application-passwords
  public: false
  scheme: basic
  type: http
- api: openapi/wahi-wp-json-discovery.json
  evidence: Standard WordPress REST behaviour for same-origin browser requests (cookie plus X-WP-Nonce). Not documented by Wahi; inherent to the WordPress core REST API it runs.
  name: wordpress-cookie-nonce
  public: false
  type: cookie
slug: wahi-authentication
source_filename: wahi-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-26'\nmethod: searched\nsource: >-\n  https://wahi.com/.well-known/ai-plugin.json, openapi/wahi-listing-search-openapi.yaml,\n  openapi/wahi-wp-json-discovery.json, and live probes of https://api.prod.wahi.com — 2026-07-26\ndocs: null\nsummary:\n  types: [none, http-basic, cookie]\n  api_key_in: []\n  oauth2_flows: []\n  developer_credential_programme: false\n  note: >-\n    Wahi issues no developer credential of any kind. There is no API key programme, no OAuth 2.0\n    or OpenID Connect developer flow, and no partner credential path. The Listing Search API that\n    Wahi publishes an OpenAPI for declares NO securitySchemes at all, and Wahi's own AI plugin\n    manifest states auth.type \"none\" with is_user_authenticated false — it was designed as an\n    anonymous read surface for a ChatGPT plugin. The only credential mechanism documented\n    anywhere on a Wahi host is WordPress application passwords on the marketing CMS, issued\n    through wp-admin\
  \ to authenticated CMS users, which is not a public developer path.\nschemes:\n- name: none\n  type: none\n  api: openapi/wahi-listing-search-openapi.yaml\n  applies_to: [searchListings]\n  evidence: >-\n    The published OpenAPI 3.0.1 contains no components.securitySchemes and no security[]\n    requirement on /search. https://wahi.com/.well-known/ai-plugin.json declares\n    \"auth\": {\"type\": \"none\"} and \"is_user_authenticated\": false.\n- name: application-passwords\n  type: http\n  scheme: basic\n  api: openapi/wahi-wp-json-discovery.json\n  authorization_endpoint: https://wahi.com/wp-admin/authorize-application.php\n  public: false\n  evidence: >-\n    The wp-json discovery document declares\n    authentication.application-passwords.endpoints.authorization. WordPress application passwords\n    are HTTP Basic credentials minted per user inside wp-admin; anonymous reads on\n    /wp-json/wp/v2/* need no credential, writes need one.\n- name: wordpress-cookie-nonce\n  type: cookie\n\
  \  api: openapi/wahi-wp-json-discovery.json\n  public: false\n  evidence: >-\n    Standard WordPress REST behaviour for same-origin browser requests (cookie plus X-WP-Nonce).\n    Not documented by Wahi; inherent to the WordPress core REST API it runs.\nconsumer_sign_in:\n  note: >-\n    Consumer sign-in on wahi.com is first-party session auth with a Google One Tap social login\n    wired to https://wahi.com/api/login/google/onetap/callback (HTTP 200, text/html). It is an\n    internal browser redirect route, not a documented API. https://wahi.com/ca/en/login redirects\n    to https://wahi.com/wp-login.php — the CMS admin login, not a consumer or developer sign-up.\ngraphql:\n  endpoint: https://api.prod.wahi.com/graphql\n  documented: false\n  introspection: disabled\n  evidence: >-\n    POST of the introspection query returns\n    {\"errors\":[{\"message\":\"introspection has been disabled\",\"extensions\":{\"code\":\"INTROSPECTION_DISABLED\"}}]}.\n    A GET without a query returns INVALID_GRAPHQL_REQUEST.\
  \ The endpoint is live but undocumented,\n    carries no published auth model, and wahi.com/robots.txt disallows */graphql. No schema was\n    harvested and none is fabricated here.\noauth: null\nscopes: null\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wahi/refs/heads/main/authentication/wahi-authentication.yml
summary_line: none/http-basic/cookie · 3 schemes
tags:
- Real Estate
- Canada
- Property Listings
- MLS
- Valuation
- AVM
- PropTech
- Rentals
- Brokerage
---
