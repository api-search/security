---
api_key_in:
- header
api_specs:
- filename: webjet-tripninja-smartflights-get-searches-openapi.yml
  format: yaml
  label: Trip Ninja SmartFlights API
  slug: tripninja-smartflights-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/webjet/refs/heads/main/openapi/webjet-tripninja-smartflights-get-searches-openapi.yml
- filename: webjet-tripninja-adminpanel-refresh-token-openapi.yml
  format: yaml
  label: Trip Ninja Admin Panel API
  slug: tripninja-admin-panel-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/webjet/refs/heads/main/openapi/webjet-tripninja-adminpanel-refresh-token-openapi.yml
- filename: webjet-tripninja-farestructure-get-searches-openapi.yml
  format: yaml
  label: Trip Ninja FareStructure API (deprecated)
  slug: tripninja-farestructure-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/webjet/refs/heads/main/openapi/webjet-tripninja-farestructure-get-searches-openapi.yml
- filename: webjet-tripninja-virtual-interlining-get-searches-openapi.yml
  format: yaml
  label: Trip Ninja Virtual Interlining API (deprecated)
  slug: tripninja-virtual-interlining-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/webjet/refs/heads/main/openapi/webjet-tripninja-virtual-interlining-get-searches-openapi.yml
- filename: 20885222-5fccfe6e-479a-429f-a497-d42a0bb859c9
  format: yaml
  label: Trip Ninja DataStream API
  slug: tripninja-datastream-api
  spec_type: Postman
  url: https://www.postman.com/tripninjadevteam/workspace/trip-ninja-public/collection/20885222-5fccfe6e-479a-429f-a497-d42a0bb859c9
- filename: webjet-tripninja-flights-core-openapi.yml
  format: yaml
  label: Trip Ninja Flights Core API
  slug: tripninja-flights-core-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/webjet/refs/heads/main/openapi/webjet-tripninja-flights-core-openapi.yml
- filename: webjet-tripninja-pricing-booking-openapi.yml
  format: yaml
  label: Trip Ninja Pricing & Booking API
  slug: tripninja-pricing-booking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/webjet/refs/heads/main/openapi/webjet-tripninja-pricing-booking-openapi.yml
- filename: webjet-tripninja-hotels-openapi.yml
  format: yaml
  label: Trip Ninja Hotels API
  slug: tripninja-hotels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/webjet/refs/heads/main/openapi/webjet-tripninja-hotels-openapi.yml
- filename: webjet-tripninja-msdp-openapi.yml
  format: yaml
  label: Trip Ninja MSDP (Dynamic Packaging) API
  slug: tripninja-msdp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/webjet/refs/heads/main/openapi/webjet-tripninja-msdp-openapi.yml
- filename: webjet-tripninja-v2-core-openapi.yml
  format: yaml
  label: Trip Ninja v2 Legacy API
  slug: tripninja-v2-legacy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/webjet/refs/heads/main/openapi/webjet-tripninja-v2-core-openapi.yml
auth_types:
- http
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Webjet Authentication
name_suffix: Authentication
oauth_flows: []
overview: Webjet secures its APIs with http and apiKey across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Webjet
provider_slug: webjet
scheme_count: 3
schemes:
- applies_to:
  - SmartFlights (v3)
  - FareStructure (v2, deprecated)
  - Virtual Interlining (v2, deprecated)
  - DataStream
  docs: https://devhub.tripninja.io/smartflights/authentication/
  environment_flags:
    is_datastream_token: false = SmartFlights credentials (true = DataStream)
    is_production_token: false = sandbox-only credentials
  example: 'headers = {"Authorization": "Token " + api_key}'
  format: 'Authorization: Token <access_token>'
  header: Authorization
  in: header
  issuance: Minted by a human in the Trip Ninja Admin Panel (app.tripninja.io) under Developer Resources. There is no self-serve signup; an admin panel username and password is issued by Trip Ninja.
  name: TokenAuthentication
  refresh:
    operation: POST /adminpanel/refresh-token/
    refresh_token_lifetime: indefinite until regenerated; using one issues a new refresh_token
    request:
      access_token: required
      refresh_token: required
    response_fields:
    - access_token
    - refresh_token
    - expiry_date
    - created_date
    - is_production_token
    - is_datastream_token
    spec: openapi/webjet-tripninja-adminpanel-refresh-token-openapi.yml
  scheme: Token
  sources:
  - https://devhub.tripninja.io/smartflights/authentication/
  - openapi/webjet-tripninja-adminpanel-refresh-token-openapi.yml
  token_lifetime: 90 days from created_date
  type: http
- applies_to:
  - SmartFlights
  - FareStructure
  - Virtual Interlining
  example: 'auth = base64.b64encode("USERNAME:PASSWORD"); headers = {"authorization": "Basic "+ auth}'
  format: 'Authorization: Basic base64(USERNAME:PASSWORD)'
  header: Authorization
  in: header
  name: BasicAuthentication
  note: Verbatim from the docs — "SmartFlights API uses both Basic Authentication and Token Authentication standards. Depending on how you signed up for your account, you will need to use one or the other. If you signed up through our admin panel please follow the Token Authentication steps. Otherwise, please follow the Basic Authentication steps." Not offered for DataStream.
  scheme: basic
  sources:
  - https://devhub.tripninja.io/smartflights/authentication/
  type: http
- base_urls:
    production: https://api.tripninja.io
    sandbox: https://sandbox.tripninja.io
  credential_cache: credentials.json on local disk (atomic write)
  env_vars:
  - TN_SDK_CLIENT_ID
  - TN_SDK_CLIENT_SECRET
  header_names:
  - X-Client-ID
  - X-Client-Secret
  in: header
  name: SDKClientCredentials
  returns: 'A credentials document keyed by token type — sandbox_token, prod_token, data_stream_token — which the SDK then presents as "Authorization: Token <token>" on every subsequent call. On a 401 the SDK re-fetches credentials and retries once.'
  sources:
  - https://github.com/trip-ninja-inc/tn-sdk-python/blob/master/src/tn_sdk/utils/constants.py
  - https://github.com/trip-ninja-inc/tn-sdk-python/blob/master/src/tn_sdk/core/tn_api.py
  status: Undocumented on the developer hub — discovered in the first-party SDK source. /sdk/auth/ appears in no published OpenAPI document.
  token_endpoint: POST /sdk/auth/
  type: apiKey
slug: webjet-authentication
source_filename: webjet-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-28'\nmethod: searched\nsource: >-\n  https://devhub.tripninja.io/smartflights/authentication/ (rendered from\n  devhub.tripninja.io/assets/index-8odYpnZf.js),\n  openapi/webjet-tripninja-adminpanel-refresh-token-openapi.yml,\n  https://github.com/trip-ninja-inc/tn-sdk-python (src/tn_sdk/core/tn_api.py, utils/constants.py)\ndocs: https://devhub.tripninja.io/smartflights/authentication/\nsummary:\n  types: [http, apiKey]\n  api_key_in: [header]\n  oauth2_flows: []\n  openid_connect: false\n  mutual_tls: false\n  note: >-\n    Trip Ninja publishes NO OAuth 2.0 and NO OpenID Connect. Nothing in the seventeen harvested\n    OpenAPI documents declares a components.securitySchemes block at all — the auth contract lives\n    only in the prose docs and in the first-party SDK source. There are consequently no OAuth scopes\n    and no scopes/ artifact for this provider.\nschemes:\n- name: TokenAuthentication\n  type: http\n  scheme: Token\n  in: header\n  header: Authorization\n\
  \  format: 'Authorization: Token <access_token>'\n  example: 'headers = {\"Authorization\": \"Token \" + api_key}'\n  applies_to:\n  - SmartFlights (v3)\n  - FareStructure (v2, deprecated)\n  - Virtual Interlining (v2, deprecated)\n  - DataStream\n  token_lifetime: 90 days from created_date\n  issuance: >-\n    Minted by a human in the Trip Ninja Admin Panel (app.tripninja.io) under Developer Resources.\n    There is no self-serve signup; an admin panel username and password is issued by Trip Ninja.\n  refresh:\n    operation: POST /adminpanel/refresh-token/\n    spec: openapi/webjet-tripninja-adminpanel-refresh-token-openapi.yml\n    request: {access_token: required, refresh_token: required}\n    response_fields: [access_token, refresh_token, expiry_date, created_date, is_production_token, is_datastream_token]\n    refresh_token_lifetime: indefinite until regenerated; using one issues a new refresh_token\n  environment_flags:\n    is_production_token: false = sandbox-only credentials\n\
  \    is_datastream_token: false = SmartFlights credentials (true = DataStream)\n  docs: https://devhub.tripninja.io/smartflights/authentication/\n  sources: [https://devhub.tripninja.io/smartflights/authentication/, openapi/webjet-tripninja-adminpanel-refresh-token-openapi.yml]\n- name: BasicAuthentication\n  type: http\n  scheme: basic\n  in: header\n  header: Authorization\n  format: 'Authorization: Basic base64(USERNAME:PASSWORD)'\n  example: 'auth = base64.b64encode(\"USERNAME:PASSWORD\"); headers = {\"authorization\": \"Basic \"+ auth}'\n  applies_to: [SmartFlights, FareStructure, Virtual Interlining]\n  note: >-\n    Verbatim from the docs — \"SmartFlights API uses both Basic Authentication and Token Authentication\n    standards. Depending on how you signed up for your account, you will need to use one or the other.\n    If you signed up through our admin panel please follow the Token Authentication steps. Otherwise,\n    please follow the Basic Authentication steps.\" Not offered\
  \ for DataStream.\n  sources: [https://devhub.tripninja.io/smartflights/authentication/]\n- name: SDKClientCredentials\n  type: apiKey\n  in: header\n  header_names: [X-Client-ID, X-Client-Secret]\n  token_endpoint: POST /sdk/auth/\n  base_urls:\n    production: https://api.tripninja.io\n    sandbox: https://sandbox.tripninja.io\n  returns: >-\n    A credentials document keyed by token type — sandbox_token, prod_token, data_stream_token — which\n    the SDK then presents as \"Authorization: Token <token>\" on every subsequent call. On a 401 the SDK\n    re-fetches credentials and retries once.\n  env_vars: [TN_SDK_CLIENT_ID, TN_SDK_CLIENT_SECRET]\n  credential_cache: credentials.json on local disk (atomic write)\n  status: >-\n    Undocumented on the developer hub — discovered in the first-party SDK source. /sdk/auth/ appears in\n    no published OpenAPI document.\n  sources:\n  - https://github.com/trip-ninja-inc/tn-sdk-python/blob/master/src/tn_sdk/utils/constants.py\n  - https://github.com/trip-ninja-inc/tn-sdk-python/blob/master/src/tn_sdk/core/tn_api.py\n\
  network_gate:\n  ip_allowlisting: true\n  quote: >-\n    \"For security, Trip Ninja's servers are only accessible from whitelisted IPs. Please contact your\n    account manager to whitelist the IPs you will be using.\"\n  effect: >-\n    A valid token is not sufficient. Every API host (sandbox.tripninja.io, preprodapi.tripninja.io,\n    api.tripninja.io) returns 403 to any source IP that has not been allow-listed by Trip Ninja.\nconsumer_brands:\n  webjet_ota: No public API and no published authentication surface.\n  gosee_airport_rentals: No public API.\n  gosee_motorhome_republic: No public API.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/webjet/refs/heads/main/authentication/webjet-authentication.yml
summary_line: http/apiKey · 3 schemes
tags:
- Travel
- Australia
- OTA
- Aviation
- Booking
- Distribution
- Flight Search
- Car Rental
- New Zealand
- Travel Technology
---
