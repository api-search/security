---
api_key_in: []
api_specs:
- filename: mercedes-me-components-api-openapi.yml
  format: yaml
  label: Mercedes-Benz Mercedes me Components API
  slug: mercedes-me-components-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mercedes-me/refs/heads/main/openapi/mercedes-me-components-api-openapi.yml
- filename: mercedes-me-configurations-api-openapi.yml
  format: yaml
  label: Mercedes-Benz Mercedes me Configurations API
  slug: mercedes-me-configurations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mercedes-me/refs/heads/main/openapi/mercedes-me-configurations-api-openapi.yml
- filename: mercedes-me-dealer-search-api-openapi.yml
  format: yaml
  label: Mercedes-Benz Mercedes me Dealer search API
  slug: mercedes-me-dealer-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mercedes-me/refs/heads/main/openapi/mercedes-me-dealer-search-api-openapi.yml
- filename: mercedes-me-diagnostic-trouble-code-dtc-snapshots-api-openapi.yml
  format: yaml
  label: Mercedes-Benz Mercedes me Diagnostic Trouble Code (DTC) Snapshots API
  slug: mercedes-me-diagnostic-trouble-code-dtc-snapshots-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mercedes-me/refs/heads/main/openapi/mercedes-me-diagnostic-trouble-code-dtc-snapshots-api-openapi.yml
- filename: mercedes-me-diagnostic-trouble-codes-dtc-s-api-openapi.yml
  format: yaml
  label: Mercedes-Benz Mercedes me Diagnostic Trouble Codes (DTC's) API
  slug: mercedes-me-diagnostic-trouble-codes-dtc-s-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mercedes-me/refs/heads/main/openapi/mercedes-me-diagnostic-trouble-codes-dtc-s-api-openapi.yml
- filename: mercedes-me-electronical-control-units-ecu-s-api-openapi.yml
  format: yaml
  label: Mercedes-Benz Mercedes me Electronical Control Units (ECU's) API
  slug: mercedes-me-electronical-control-units-ecu-s-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mercedes-me/refs/heads/main/openapi/mercedes-me-electronical-control-units-ecu-s-api-openapi.yml
- filename: mercedes-me-images-api-openapi.yml
  format: yaml
  label: Mercedes-Benz Mercedes me Images API
  slug: mercedes-me-images-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mercedes-me/refs/heads/main/openapi/mercedes-me-images-api-openapi.yml
- filename: mercedes-me-perspectives-api-openapi.yml
  format: yaml
  label: Mercedes-Benz Mercedes me Perspectives API
  slug: mercedes-me-perspectives-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mercedes-me/refs/heads/main/openapi/mercedes-me-perspectives-api-openapi.yml
- filename: mercedes-me-references-api-openapi.yml
  format: yaml
  label: Mercedes-Benz Mercedes me References API
  slug: mercedes-me-references-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mercedes-me/refs/heads/main/openapi/mercedes-me-references-api-openapi.yml
- filename: mercedes-me-resources-api-openapi.yml
  format: yaml
  label: Mercedes-Benz Mercedes me Resources API
  slug: mercedes-me-resources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mercedes-me/refs/heads/main/openapi/mercedes-me-resources-api-openapi.yml
- filename: mercedes-me-saved-configurations-api-openapi.yml
  format: yaml
  label: Mercedes-Benz Mercedes me Saved configurations API
  slug: mercedes-me-saved-configurations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mercedes-me/refs/heads/main/openapi/mercedes-me-saved-configurations-api-openapi.yml
auth_types: []
description: Mercedes-Benz runs two distinct authentication models across one API gateway, and which one applies depends on whether the API touches a customer's vehicle.
kind: authentication
layout: security
method: probed
name: Mercedes Me Authentication
name_suffix: Authentication
oauth_flows: []
overview: Mercedes-Benz Mercedes me declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: Mercedes-Benz Mercedes me
provider_slug: mercedes-me
scheme_count: 3
schemes:
- applies_to:
  - Car Configurator API (Components, Configurations, Images, References, Saved configurations)
  - Dealer API (Dealer search)
  - Vehicle Images API (Components, Perspectives)
  - Remote Diagnostic Support API (DTCs, DTC Snapshots, ECUs, Resources)
  evidence: 'Every operation in all four published Swagger 2.0 documents declares a 401 whose description is "Unauthorized: * Failed to resolve API Key query parameter * Invalid API Key". The key is issued per subscribed product on the developer portal. NOTE: the specs declare this in prose only — they carry no securityDefinitions object at all, so no machine can discover the parameter name from the contract.'
  gap: The contract does not name the query parameter that carries the key. An agent reading the OpenAPI cannot construct an authenticated request without a human reading the portal.
  id: mercedes-benz-api-key
  in: query
  type: apiKey
- applies_to:
  - Vehicle Status API
  - Vehicle Lock Status API
  - Fuel Status API
  - Electric Vehicle Status API
  - Pay As You Drive 2.0 API
  - Mercedes-Benz Fleet API (Kafka Push consumers authenticate with OAuth 2.0)
  consent_model: 'Authorization-code flow in which the VEHICLE OWNER — not the developer — grants per-resource consent. Scope selection is the consent surface: an application requesting mb:vehicle:mbdata:fuelstatus receives tank level and nothing else. See scopes/mercedes-me-scopes.yml for all 38 published product scopes.'
  flows:
    authorizationCode:
      authorizationUrl: https://id.mercedes-benz.com/as/authorization.oauth2
      pkce: S256
      refreshUrl: https://id.mercedes-benz.com/as/token.oauth2
      tokenUrl: https://id.mercedes-benz.com/as/token.oauth2
    clientCredentials:
      tokenUrl: https://id.mercedes-benz.com/as/token.oauth2
    deviceCode:
      deviceAuthorizationUrl: present in discovery document
  id: mercedes-benz-oauth2
  scopes_reference: scopes/mercedes-me-scopes.yml
  type: oauth2
- claims_supported:
  - acr
  - ciam-uid
  - company-id
  - country
  - email
  - email_verified
  - family_name
  - given_name
  - identityProviders
  - known_user
  - locale
  - name
  - phone_number
  - phone_number_verified
  - reg-track-id
  - sub
  - third-party-ids
  id: mercedes-benz-openid-connect
  id_token_signing_alg_values_supported:
  - RS256
  - RS384
  - RS512
  - ES256
  - ES384
  - ES512
  - PS256
  - PS384
  - PS512
  - HS256
  - HS384
  - HS512
  - none
  issuer: https://id.mercedes-benz.com
  jwks_uri: https://id.mercedes-benz.com/pf/JWKS
  openIdConnectUrl: https://id.mercedes-benz.com/.well-known/openid-configuration
  subject_types_supported:
  - public
  - pairwise
  type: openIdConnect
  userinfo_endpoint: https://id.mercedes-benz.com/idp/userinfo.openid
slug: mercedes-me-authentication
source_filename: mercedes-me-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-26'\nmethod: probed\nsource: >-\n  https://id.mercedes-benz.com/.well-known/openid-configuration (probed 200, saved verbatim) plus the\n  401 response descriptions declared in the four provider-published Swagger 2.0 documents in\n  openapi/_original/.\ndocs: https://developer.mercedes-benz.com/content-page/oauth-documentation\nevidence:\n  - url: https://id.mercedes-benz.com/.well-known/openid-configuration\n    status: 200\n  - url: https://id.mercedes-benz.com/.well-known/oauth-authorization-server\n    status: 200\n  - url: https://api.mercedes-benz.com/configurator/v1/markets\n    status: 401\n    body: '{\"errorMessage\":\"Unauthorized\",\"statusCode\":\"401\",\"message\":\"No credentials provided\"}'\n  - url: https://developer.mercedes-benz.com/content-page/oauth-documentation\n    status: 200\n    note: >-\n      HTTP 200 but the body is the portal's client-rendered SPA shell — identical to the shell served\n      for a path that does not exist —\
  \ so the OAuth reference text itself could not be read by a\n      non-browser client.\ndescription: >-\n  Mercedes-Benz runs two distinct authentication models across one API gateway, and which one applies\n  depends on whether the API touches a customer's vehicle.\nsummary:\n  models: 2\n  oauth2: true\n  openid_connect: true\n  api_key: true\n  mutual_tls: true            # tls_client_auth is advertised in token_endpoint_auth_methods_supported\n  pkce: true                  # S256\n  par: true                   # pushed_authorization_request_endpoint present\n  ciba: true                  # urn:openid:params:grant-type:ciba\n  token_exchange: true        # urn:ietf:params:oauth:grant-type:token-exchange\n  dynamic_client_registration: true   # registration_endpoint present\n  token_revocation: true\n  token_introspection: true\nschemes:\n  - id: mercedes-benz-api-key\n    type: apiKey\n    in: query\n    applies_to:\n      - Car Configurator API (Components, Configurations, Images,\
  \ References, Saved configurations)\n      - Dealer API (Dealer search)\n      - Vehicle Images API (Components, Perspectives)\n      - Remote Diagnostic Support API (DTCs, DTC Snapshots, ECUs, Resources)\n    evidence: >-\n      Every operation in all four published Swagger 2.0 documents declares a 401 whose description is\n      \"Unauthorized: * Failed to resolve API Key query parameter * Invalid API Key\". The key is issued\n      per subscribed product on the developer portal. NOTE: the specs declare this in prose only —\n      they carry no securityDefinitions object at all, so no machine can discover the parameter name\n      from the contract.\n    gap: >-\n      The contract does not name the query parameter that carries the key. An agent reading the\n      OpenAPI cannot construct an authenticated request without a human reading the portal.\n  - id: mercedes-benz-oauth2\n    type: oauth2\n    flows:\n      authorizationCode:\n        authorizationUrl: https://id.mercedes-benz.com/as/authorization.oauth2\n\
  \        tokenUrl: https://id.mercedes-benz.com/as/token.oauth2\n        refreshUrl: https://id.mercedes-benz.com/as/token.oauth2\n        pkce: S256\n      clientCredentials:\n        tokenUrl: https://id.mercedes-benz.com/as/token.oauth2\n      deviceCode:\n        deviceAuthorizationUrl: present in discovery document\n    applies_to:\n      - Vehicle Status API\n      - Vehicle Lock Status API\n      - Fuel Status API\n      - Electric Vehicle Status API\n      - Pay As You Drive 2.0 API\n      - Mercedes-Benz Fleet API (Kafka Push consumers authenticate with OAuth 2.0)\n    consent_model: >-\n      Authorization-code flow in which the VEHICLE OWNER — not the developer — grants per-resource\n      consent. Scope selection is the consent surface: an application requesting\n      mb:vehicle:mbdata:fuelstatus receives tank level and nothing else. See\n      scopes/mercedes-me-scopes.yml for all 38 published product scopes.\n    scopes_reference: scopes/mercedes-me-scopes.yml\n  - id: mercedes-benz-openid-connect\n\
  \    type: openIdConnect\n    openIdConnectUrl: https://id.mercedes-benz.com/.well-known/openid-configuration\n    issuer: https://id.mercedes-benz.com\n    userinfo_endpoint: https://id.mercedes-benz.com/idp/userinfo.openid\n    jwks_uri: https://id.mercedes-benz.com/pf/JWKS\n    claims_supported:\n      - acr\n      - ciam-uid\n      - company-id\n      - country\n      - email\n      - email_verified\n      - family_name\n      - given_name\n      - identityProviders\n      - known_user\n      - locale\n      - name\n      - phone_number\n      - phone_number_verified\n      - reg-track-id\n      - sub\n      - third-party-ids\n    subject_types_supported: [public, pairwise]\n    id_token_signing_alg_values_supported: [RS256, RS384, RS512, ES256, ES384, ES512, PS256, PS384, PS512, HS256, HS384, HS512, none]\ntoken_endpoint_auth_methods:\n  - client_secret_basic\n  - client_secret_post\n  - client_secret_jwt\n  - private_key_jwt\n  - tls_client_auth\n  - none\nobservations:\n  - >-\n\
  \    STRONG: the authorization server advertises PKCE S256, pushed authorization requests, private_key_jwt\n    and mutual-TLS client authentication, and dynamic client registration — a modern, FAPI-adjacent\n    posture for an OEM identity provider.\n  - >-\n    WEAK: implicit, password and the \"none\" token-endpoint auth method are still advertised as supported.\n    A public OAuth discovery document that still lists the resource-owner password grant is a legacy\n    surface an integrator should be told not to use; Mercedes-Benz publishes no statement deprecating it\n    that we could read.\n  - >-\n    WEAK: no securityDefinitions in ANY published OpenAPI. The four Swagger 2.0 documents describe\n    authentication only in a 401 response description string. That is not machine-readable auth: an\n    agent cannot construct a request from the contract alone.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mercedes-me/refs/heads/main/authentication/mercedes-me-authentication.yml
summary_line: 3 schemes
tags:
- Automotive
- Connected Car
- Connected Vehicle
- Daimler
- Fleet Management
- Mercedes me
- Mercedes-Benz
- OEM
- Telematics
- Vehicle Data
---
