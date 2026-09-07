---
anonymous_access: false
api_key_in: []
api_specs:
- filename: bp-fleet-authentication-openapi.json
  format: json
  label: bp Open Fleet Authentication API
  slug: bp-fleet-authentication
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bp/refs/heads/main/openapi/bp-fleet-authentication-openapi.json
- filename: bp-fleet-card-management-openapi.json
  format: json
  label: bp Open Fleet Card Management API
  slug: bp-fleet-card-management
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bp/refs/heads/main/openapi/bp-fleet-card-management-openapi.json
- filename: bp-fleet-invoice-management-openapi.json
  format: json
  label: bp Open Fleet Invoice Management API
  slug: bp-fleet-invoice-management
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bp/refs/heads/main/openapi/bp-fleet-invoice-management-openapi.json
- filename: bp-fleet-transaction-management-openapi.json
  format: json
  label: bp Open Fleet Transaction Management API
  slug: bp-fleet-transaction-management
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bp/refs/heads/main/openapi/bp-fleet-transaction-management-openapi.json
- filename: bp-fleet-retail-site-information-openapi.json
  format: json
  label: bp Open Fleet Retail Site Information API
  slug: bp-fleet-retail-site-information
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bp/refs/heads/main/openapi/bp-fleet-retail-site-information-openapi.json
- filename: bp-fleet-aral-appconnect-openapi.json
  format: json
  label: bp Open Fleet Aral AppConnect (Pay@Pump) API
  slug: bp-fleet-aral-appconnect
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bp/refs/heads/main/openapi/bp-fleet-aral-appconnect-openapi.json
auth_types: []
description: 'Authentication profile for the bp Open Fleet API platform. Two distinct surfaces exist: a machine-to-machine client-credentials exchange that issues the bearer token every Open Fleet API requires, and a browser OpenID Connect flow on BP''s B2B identity host used to sign in to the developer portal itself.'
kind: authentication
layout: security
mechanism_count: 0
method: searched
name: Bp Authentication
name_suffix: Authentication
oauth_flows: []
overview: BP declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: BP
provider_slug: bp
scheme_count: 0
schemes: []
slug: bp-authentication
source_filename: bp-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-04'\nmethod: searched\nsource: >-\n  https://b2bid.bp.com/.well-known/openid-configuration (fetched, HTTP 200) plus the\n  securitySchemes and /token operation of the six bp Open Fleet OpenAPI documents published on\n  https://developer.fleet.bp.com/DE/api-status, and the OAuth client code shipped by that portal.\nprovider: BP\nproviderId: bp\ndescription: >-\n  Authentication profile for the bp Open Fleet API platform. Two distinct surfaces exist: a\n  machine-to-machine client-credentials exchange that issues the bearer token every Open Fleet\n  API requires, and a browser OpenID Connect flow on BP's B2B identity host used to sign in to\n  the developer portal itself.\nsurfaces:\n  - name: bp Open Fleet API — bearer token\n    type: machine-to-machine\n    scheme: oauth2-client-credentials\n    token_endpoint: https://api.fleet.bp.com/authentication/v1.0/token\n    token_endpoint_note: >-\n      The Authentication API's OpenAPI declares POST /token. The\
  \ host and the\n      /authentication/v1.0/ prefix are read from the portal's own base-URL builder, which\n      composes https://api.fleet.bp.com/{apiPrefix}/v{version}/ and compares the path segments\n      against the literals \"authentication\" and \"v1.0\".\n    credentials:\n      - name: client_id\n        in: formData\n        required: true\n      - name: client_secret\n        in: formData\n        required: true\n    request_media_type: application/x-www-form-urlencoded\n    response:\n      access_token: string\n      token_type: string\n      expires_in: integer (int32)\n      ext_expires_in: integer (int32)\n    responses_documented: [200, 401, 403]\n    environment_scoping: >-\n      Credentials are bound to one environment. BP's getting-started page states sandbox\n      credentials can only reach sandbox authentication and API product endpoints, and\n      production credentials only production endpoints.\n  - name: bp Open Fleet API — resource requests\n    type: bearer\n\
  \    scheme: http-bearer\n    header: Authorization\n    format: \"Bearer <access_token>\"\n    declared_as: >-\n      Every resource spec declares securitySchemes.Bearer as type apiKey, in header, name\n      Authorization, described as \"JWT Authorization header using the Bearer scheme\". That is an\n      apiKey-typed declaration of what is functionally HTTP bearer auth — a common OpenAPI 3.0\n      idiom, recorded here as published rather than corrected.\n    applies_to:\n      - Card Management\n      - Invoice Management\n      - Transaction Management\n      - Retail Site Information\n      - Aral AppConnect (Pay@Pump)\n  - name: bp B2B identity (developer portal sign-in)\n    type: user\n    scheme: openid-connect\n    issuer: https://b2bid.bp.com/am/oauth2\n    discovery: https://b2bid.bp.com/.well-known/openid-configuration\n    platform: ForgeRock Access Management\n    client_id_observed: openfleet-global-web\n    endpoints:\n      authorization: https://b2bid.bp.com/am/oauth2/authorize\n\
  \      token: https://b2bid.bp.com/am/oauth2/access_token\n      userinfo: https://b2bid.bp.com/am/oauth2/userinfo\n      jwks: https://b2bid.bp.com/am/oauth2/connect/jwk_uri\n      registration: https://b2bid.bp.com/am/oauth2/register\n      introspection: https://b2bid.bp.com/am/oauth2/introspect\n      revocation: https://b2bid.bp.com/am/oauth2/token/revoke\n      end_session: https://b2bid.bp.com/am/oauth2/connect/endSession\n      pushed_authorization_request: https://b2bid.bp.com/am/oauth2/par\n    pkce:\n      supported: true\n      methods: [plain, S256]\n      observed_in_use: S256\n    grant_types_supported:\n      - authorization_code\n      - client_credentials\n      - refresh_token\n      - implicit\n      - password\n      - urn:ietf:params:oauth:grant-type:device_code\n      - urn:ietf:params:oauth:grant-type:jwt-bearer\n      - urn:ietf:params:oauth:grant-type:saml2-bearer\n      - urn:ietf:params:oauth:grant-type:uma-ticket\n      - urn:openid:params:grant-type:ciba\n\
  \    token_endpoint_auth_methods_supported:\n      - client_secret_basic\n      - client_secret_post\n      - private_key_jwt\n      - tls_client_auth\n      - self_signed_tls_client_auth\n      - none\n    mutual_tls_bound_access_tokens: true\n    dynamic_client_registration: true\n    pushed_authorization_requests: true\n    require_pushed_authorization_requests: false\nnotes:\n  - >-\n    No API key, basic-auth or mTLS option is documented for the Open Fleet resource APIs; a\n    bearer token from the Authentication API is the only published path.\n  - >-\n    The separate bp API Marketplace (api.developer.bp.com) documents Basic Auth and OAuth2, but\n    its catalogue is behind a login and no machine-readable contract was reachable anonymously.\nmaintainers:\n  - FN: Kin Lane\n    email: info@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bp/refs/heads/main/authentication/bp-authentication.yml
summary_line: 0 schemes
tags:
- Energy
- Oil
- Gas
- Renewables
- Developer Platform
- Fleet
- Fuel Cards
- Mobility
- Retail Fuel
- EV Charging
---
