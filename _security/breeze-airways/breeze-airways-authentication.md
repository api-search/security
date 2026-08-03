---
api_key_in:
- header
auth_types:
- apiKey
- http-basic
- http-bearer
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Breeze Airways Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: Breeze Airways secures its APIs with apiKey, http-basic, http-bearer, and oauth2 across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: Breeze Airways
provider_slug: breeze-airways
scheme_count: 4
schemes:
- applies_to: all routes
  description: Azure API Management subscription key, unique per partner and per environment (sandbox vs production). It does not rotate per session. A missing or incorrect value returns 401 Access Denied with a WWW-Authenticate AzureApiManagementKey response header.
  in: header
  name: SubscriptionKey
  parameter_name: Ocp-Apim-Subscription-Key
  required: true
  source: https://ndc.flybreeze.com/docs/ndc-for-developers/authentication
  type: apiKey
- applies_to:
  - POST /api/Selling/r3.x/Auth
  description: Base64 encoded agency credentials presented on the Authorization header of the token request only. Credentials are issued by Breeze and delivered over a secure Bitwarden Send link (https://send.bitwarden.com).
  name: BasicAuth
  scheme: basic
  source: https://ndc.flybreeze.com/docs/ndc-for-developers/authentication
  type: http
- applies_to: all Selling and Servicing routes, plus Shopping AirlineProfile
  bearerFormat: JWT
  description: Session bearer token returned by the Auth endpoint. Stateful — the token creates a unique session in the Breeze reservation system, so a new token must be obtained for each transaction flow. Concurrent use of one token across bookings causes failures.
  name: SessionBearerToken
  scheme: bearer
  source: https://ndc.flybreeze.com/docs/ndc-for-developers/authentication
  type: http
- description: The Auth endpoint implements an OAuth 2.0 client-credentials style exchange — a JSON body of {"grant_type":"client_credentials"} with HTTP Basic credentials returns an access_token (JWT), token_type Bearer, and expires_in 00:30:00. The JWT aud claim carries the four authorized service audiences. Declaring the optional role query parameter makes the token request roughly twice as fast because the gateway then avoids an extra reservation-system lookup.
  expires_in: 00:30:00
  flow: clientCredentials
  grant_type: client_credentials
  name: OAuth2ClientCredentials
  source: https://ndc.flybreeze.com/docs/ndc-for-developers/authentication
  token_audiences:
  - shopping
  - selling
  - servicing
  - orderchangenotification
  token_lifetime_seconds: 1800
  token_type: Bearer
  token_url: /api/Selling/r3.x/Auth
  token_url_optional_parameter: ?role={rolecode}
  type: oauth2
slug: breeze-airways-authentication
source_filename: breeze-airways-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-01'\nmethod: searched\nsource: https://ndc.flybreeze.com/docs/ndc-for-developers/authentication\ndocs: https://ndc.flybreeze.com/docs/ndc-for-developers/authentication\napi: Breeze Airways NDC Gateway\nsummary:\n  types:\n  - apiKey\n  - http-basic\n  - http-bearer\n  - oauth2\n  api_key_in:\n  - header\n  oauth2_flows:\n  - clientCredentials\n  network_controls:\n  - ip-allowlisting\nnotes: >-\n  Derived by reading the Breeze Airways NDC gateway authentication documentation.\n  Breeze publishes no OpenAPI or machine-readable security scheme document, so this\n  profile is transcribed from the published route/authorization table and the token\n  request/response samples on the authentication page. Every request to the gateway\n  carries a per-partner Azure API Management subscription key; most routes then\n  additionally require a short-lived session bearer token.\nschemes:\n- name: SubscriptionKey\n  type: apiKey\n  in: header\n  parameter_name: Ocp-Apim-Subscription-Key\n\
  \  required: true\n  applies_to: all routes\n  description: >-\n    Azure API Management subscription key, unique per partner and per environment\n    (sandbox vs production). It does not rotate per session. A missing or incorrect\n    value returns 401 Access Denied with a WWW-Authenticate AzureApiManagementKey\n    response header.\n  source: https://ndc.flybreeze.com/docs/ndc-for-developers/authentication\n- name: BasicAuth\n  type: http\n  scheme: basic\n  applies_to:\n  - POST /api/Selling/r3.x/Auth\n  description: >-\n    Base64 encoded agency credentials presented on the Authorization header of the\n    token request only. Credentials are issued by Breeze and delivered over a secure\n    Bitwarden Send link (https://send.bitwarden.com).\n  source: https://ndc.flybreeze.com/docs/ndc-for-developers/authentication\n- name: SessionBearerToken\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  applies_to: all Selling and Servicing routes, plus Shopping AirlineProfile\n  description:\
  \ >-\n    Session bearer token returned by the Auth endpoint. Stateful — the token creates\n    a unique session in the Breeze reservation system, so a new token must be\n    obtained for each transaction flow. Concurrent use of one token across bookings\n    causes failures.\n  source: https://ndc.flybreeze.com/docs/ndc-for-developers/authentication\n- name: OAuth2ClientCredentials\n  type: oauth2\n  flow: clientCredentials\n  token_url: /api/Selling/r3.x/Auth\n  token_url_optional_parameter: '?role={rolecode}'\n  grant_type: client_credentials\n  token_type: Bearer\n  expires_in: 00:30:00\n  token_lifetime_seconds: 1800\n  token_audiences:\n  - shopping\n  - selling\n  - servicing\n  - orderchangenotification\n  description: >-\n    The Auth endpoint implements an OAuth 2.0 client-credentials style exchange —\n    a JSON body of {\"grant_type\":\"client_credentials\"} with HTTP Basic credentials\n    returns an access_token (JWT), token_type Bearer, and expires_in 00:30:00. The\n   \
  \ JWT aud claim carries the four authorized service audiences. Declaring the\n    optional role query parameter makes the token request roughly twice as fast\n    because the gateway then avoids an extra reservation-system lookup.\n  source: https://ndc.flybreeze.com/docs/ndc-for-developers/authentication\nauthorization_by_route:\n- route: /api/Selling/r3.x/Auth\n  methods: [POST]\n  authorization: Basic\n  message: Authorization\n- route: /api/Shopping/r3.x/v21.3/AirlineProfile\n  methods: [GET, POST]\n  authorization: Bearer\n  message: IATA_AirlineProfileRQ / IATA_AirlineProfileRS\n- route: /api/Shopping/r3.x/v21.3/AirShopping\n  methods: [GET, POST]\n  authorization: none\n  message: IATA_AirShoppingRQ / IATA_AirShoppingRS\n- route: /api/Selling/r3.x/v21.3/SeatAvailability\n  methods: [POST]\n  authorization: Bearer\n  message: IATA_SeatAvailabilityRQ / IATA_SeatAvailabilityRS\n- route: /api/Servicing/r3.x/v21.3/SeatAvailability\n  methods: [POST]\n  authorization: Bearer\n  message:\
  \ IATA_SeatAvailabilityRQ / IATA_SeatAvailabilityRS\n- route: /api/Selling/r3.x/v21.3/ServiceList\n  methods: [POST]\n  authorization: Bearer\n  message: IATA_ServiceListRQ / IATA_ServiceListRS\n- route: /api/Servicing/r3.x/v21.3/ServiceList\n  methods: [POST]\n  authorization: Bearer\n  message: IATA_ServiceListRQ / IATA_ServiceListRS\n- route: /api/Selling/r3.x/v21.3/OfferPrice\n  methods: [POST]\n  authorization: Bearer\n  message: IATA_OfferPriceRQ / IATA_OfferPriceRS\n- route: /api/Selling/r3.x/v21.3/OrderCreate\n  methods: [POST]\n  authorization: Bearer\n  message: IATA_OrderCreateRQ / IATA_OrderViewRS\n- route: /api/Servicing/r3.x/v21.3/OrderRetrieve\n  methods: [POST]\n  authorization: Bearer\n  message: IATA_OrderRetrieveRQ / IATA_OrderViewRS\n- route: /api/Servicing/r3.x/v21.3/OrderChange\n  methods: [POST]\n  authorization: Bearer\n  message: IATA_OrderChangeRQ / IATA_OrderViewRS\n- route: /api/Servicing/r3.x/v21.3/OrderReshop\n  methods: [POST]\n  authorization: Bearer\n \
  \ message: IATA_OrderReshopRQ / IATA_OrderReshopRS\n- route: /api/Servicing/r3.x/v21.3/OrderQuote\n  methods: [POST]\n  authorization: Bearer\n  message: IATA_OrderQuoteRQ / IATA_OrderReshopRS\nonboarding:\n  prerequisites:\n  - IATA or ARC agency number\n  - Executed commercial agreement (agreement in principle accepted for sandbox access)\n  - Declared agency content type (leisure, business/corporate, or federal government)\n  - List of egress IP addresses for sandbox and production allowlisting\n  credential_delivery: https://send.bitwarden.com\n  ip_allowlist_sla: requests to allow additional IPs are typically fulfilled within one week\n  source: https://ndc.flybreeze.com/docs/ndc-for-developers/getting-started\nx-evidence:\n  fetched: '2026-08-01'\n  urls:\n  - url: https://ndc.flybreeze.com/docs/ndc-for-developers/authentication\n    http_status: 200\n  - url: https://ndc.flybreeze.com/docs/ndc-for-developers/getting-started\n    http_status: 200\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/breeze-airways/refs/heads/main/authentication/breeze-airways-authentication.yml
summary_line: apiKey/http-basic/http-bearer/oauth2 · 4 schemes
tags:
- Company
- Airlines
- Travel
- Aviation
- NDC
- Distribution
- Booking
- Reservations
- Travel Agencies
- IATA
---
