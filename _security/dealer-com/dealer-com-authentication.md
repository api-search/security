---
api_key_in: []
auth_types: []
description: Dealer.com runs two distinct, publicly documented authentication models, one per API family. The Dealer Developer Portal APIs (Accounts, Incentives, Inventory — the "Vehicle Consumer Display API") use a single API key issued on registration, passed either as an `api_key` query parameter or as a request header. The Website Integration API — the browser-side Integrated Partner Program surface — uses no key at call time; instead Dealer.com signs a JWT asserting that it rendered a given page, for a given account, on a given domain, with given vehicles, and publishes the rotating RSA public keys as a JWK Set the partner validates server-side before releasing paid content.
kind: authentication
layout: security
method: searched
name: Dealer Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: Dealer.com declares 5 security scheme(s) across its OpenAPI definitions.
provider_name: Dealer.com
provider_slug: dealer-com
scheme_count: 5
schemes:
- applies_to:
  - Dealer.com Accounts API
  - Dealer.com Incentives API
  - Dealer.com Inventory (Vehicle / Equipment / Price) API
  description: Authorized API key issued per consumer on registration at the Cox Automotive Developer Network. Documented form is {protocol}://api.dealer.com/{endpoint}?api_key={API key}. Required on every call.
  evidence: '"Requests to the API are authenticated using API key authentication. Simply provide the key in either a header or query string parameter and requests will be authenticated as the corresponding consumer." — Dealer Developer Portal, General Concepts.'
  id: api_key_query
  in: query
  name: api_key
  registration: https://coxautoinc.mashery.com/member/register
  required: true
  type: apiKey
- applies_to:
  - Dealer.com Accounts API
  - Dealer.com Incentives API
  - Dealer.com Inventory (Vehicle / Equipment / Price) API
  confidence: medium
  description: The Accounts API general-concepts page states the key "must be provided in either query string or request header". The exact header name is not published; the Swagger UI shipped with the portal wires the key as a query parameter named api_key.
  id: api_key_header
  in: header
  name: api_key
  required: false
  type: apiKey
- applies_to:
  - Dealer.com Website Integration API
  contact: IntegratedPartners@coxautoinc.com
  description: Integrated Partner Program integration key, issued after enrollment. It identifies the partner integration to the Dealer.com website platform; it is configured on the integration rather than sent on a public HTTP call.
  id: ipp_integration_key
  in: config
  name: integration key
  registration: https://forms.dealer.com/integrated-partner-program.htm
  required: true
  type: apiKey
- applies_to:
  - Dealer.com Website Integration API
  bearerFormat: JWT
  description: Loosely-coupled content-delivery authentication. API.utils.getJwtForSite() and API.utils.getJwtForVehicles() return JWTs asserting that Dealer.com rendered a page containing specific vehicles, on a specific domain, for a specific account. The partner validates the RS256 signature against Dealer.com's published JWK Set and decides whether to serve paid content. Dealer.com issues an `iat` claim but deliberately issues NO `exp` claim — the consumer must define its own freshness window. An implicit expiry is reached when the signing keypair's public key stops being published.
  id: ipp_jwt
  scheme: bearer
  standards:
  - RFC 7515 (JWS)
  - RFC 7517 (JWK)
  - RFC 7519 (JWT)
  type: http
- applies_to:
  - Dealer.com Leads API
  description: Platform-level Cox Automotive Integration Platform APIs (leads, inventory, deal, digital retail) at developer.coxautoinc.com authenticate with OAuth against an Okta tenant (rapi-storefront-prod.okta.com) and require an approved partner agreement. The OIDC discovery document is anonymous and readable; the API reference behind it is not.
  discovery: https://rapi-storefront-prod.okta.com/.well-known/openid-configuration
  grant_types_documented: false
  id: cox_platform_oauth
  note: Okta's discovery document advertises authorization_code, implicit, refresh_token, password and client_credentials, but Cox Automotive publishes no scope reference, so no scopes/ artifact is authored.
  required: true
  scopes_documented: false
  type: oauth2
slug: dealer-com-authentication
source_filename: dealer-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-12'\nmethod: searched\nsource: https://developer.inv.dealer.com/content/inventory/inventory-home.html\nprovider: Dealer.com\nproviderId: dealer-com\ndocs:\n  - https://developer.inv.dealer.com/content/accounts/accounts-home.html\n  - https://developer.inv.dealer.com/content/inventory/inventory-home.html\n  - https://dealerdotcom.github.io/web-integration-api-docs/\ndescription: >-\n  Dealer.com runs two distinct, publicly documented authentication models, one per API family.\n  The Dealer Developer Portal APIs (Accounts, Incentives, Inventory — the \"Vehicle Consumer\n  Display API\") use a single API key issued on registration, passed either as an `api_key`\n  query parameter or as a request header. The Website Integration API — the browser-side\n  Integrated Partner Program surface — uses no key at call time; instead Dealer.com signs a\n  JWT asserting that it rendered a given page, for a given account, on a given domain, with\n  given vehicles, and publishes\
  \ the rotating RSA public keys as a JWK Set the partner\n  validates server-side before releasing paid content.\nschemes:\n  - id: api_key_query\n    type: apiKey\n    in: query\n    name: api_key\n    description: >-\n      Authorized API key issued per consumer on registration at the Cox Automotive Developer\n      Network. Documented form is {protocol}://api.dealer.com/{endpoint}?api_key={API key}.\n      Required on every call.\n    required: true\n    applies_to:\n      - Dealer.com Accounts API\n      - Dealer.com Incentives API\n      - Dealer.com Inventory (Vehicle / Equipment / Price) API\n    registration: https://coxautoinc.mashery.com/member/register\n    evidence: >-\n      \"Requests to the API are authenticated using API key authentication. Simply provide the\n      key in either a header or query string parameter and requests will be authenticated as\n      the corresponding consumer.\" — Dealer Developer Portal, General Concepts.\n  - id: api_key_header\n    type: apiKey\n\
  \    in: header\n    name: api_key\n    description: >-\n      The Accounts API general-concepts page states the key \"must be provided in either query\n      string or request header\". The exact header name is not published; the Swagger UI shipped\n      with the portal wires the key as a query parameter named api_key.\n    required: false\n    confidence: medium\n    applies_to:\n      - Dealer.com Accounts API\n      - Dealer.com Incentives API\n      - Dealer.com Inventory (Vehicle / Equipment / Price) API\n  - id: ipp_integration_key\n    type: apiKey\n    in: config\n    name: integration key\n    description: >-\n      Integrated Partner Program integration key, issued after enrollment. It identifies the\n      partner integration to the Dealer.com website platform; it is configured on the\n      integration rather than sent on a public HTTP call.\n    required: true\n    applies_to:\n      - Dealer.com Website Integration API\n    registration: https://forms.dealer.com/integrated-partner-program.htm\n\
  \    contact: IntegratedPartners@coxautoinc.com\n  - id: ipp_jwt\n    type: http\n    scheme: bearer\n    bearerFormat: JWT\n    description: >-\n      Loosely-coupled content-delivery authentication. API.utils.getJwtForSite() and\n      API.utils.getJwtForVehicles() return JWTs asserting that Dealer.com rendered a page\n      containing specific vehicles, on a specific domain, for a specific account. The partner\n      validates the RS256 signature against Dealer.com's published JWK Set and decides whether\n      to serve paid content. Dealer.com issues an `iat` claim but deliberately issues NO `exp`\n      claim — the consumer must define its own freshness window. An implicit expiry is reached\n      when the signing keypair's public key stops being published.\n    applies_to:\n      - Dealer.com Website Integration API\n    standards:\n      - RFC 7515 (JWS)\n      - RFC 7517 (JWK)\n      - RFC 7519 (JWT)\n  - id: cox_platform_oauth\n    type: oauth2\n    description: >-\n      Platform-level\
  \ Cox Automotive Integration Platform APIs (leads, inventory, deal, digital\n      retail) at developer.coxautoinc.com authenticate with OAuth against an Okta tenant\n      (rapi-storefront-prod.okta.com) and require an approved partner agreement. The OIDC\n      discovery document is anonymous and readable; the API reference behind it is not.\n    required: true\n    applies_to:\n      - Dealer.com Leads API\n    discovery: https://rapi-storefront-prod.okta.com/.well-known/openid-configuration\n    grant_types_documented: false\n    scopes_documented: false\n    note: >-\n      Okta's discovery document advertises authorization_code, implicit, refresh_token,\n      password and client_credentials, but Cox Automotive publishes no scope reference, so no\n      scopes/ artifact is authored.\nkey_material:\n  - name: Integrated Partner Program JWK Set\n    url: https://api.web.dealer.com/ipp/keys/jwks.json\n    status: 200\n    file: dealer-com-ipp-jwks.json\n    fetched: '2026-08-12'\n \
  \   key_count: 31\n    kty: RSA\n    alg: RS256\n    use: sig\n    rotation: >-\n      Keys rotate. Dealer.com publishes each public key well before the matching private key\n      is used to sign, so a consumer polling the set can always validate a fresh token.\n      Consumers SHOULD poll and cache briefly and SHOULD NOT cache keys for long, so revoked\n      keys drop out promptly.\n    served_from: Dealer.com CDN over HTTPS on a *.dealer.com domain\ngaps:\n  - No OAuth 2.0 or OpenID Connect on the Dealer.com-branded developer APIs — a single\n    long-lived API key in a query string is the whole model.\n  - The header form of the API key is documented as supported but the header NAME is never\n    published, so an integrator cannot use it without asking support.\n  - No key rotation, expiry, or revocation policy is published for the api_key credential.\n  - No scopes or permission model; access is scoped by which dealer accounts the consumer has\n    been authorized for, out of band.\n\
  maintainers:\n  - FN: Kin Lane\n    email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dealer-com/refs/heads/main/authentication/dealer-com-authentication.yml
summary_line: 5 schemes
tags:
- Automotive
- Dealership
- Digital Marketing
- Website Platform
- Inventory
- Vehicle Data
- Incentives
- Leads
- Digital Advertising
- Cox Automotive
- Partner Program
---
