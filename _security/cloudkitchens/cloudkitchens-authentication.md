---
api_key_in: []
api_specs:
- filename: cloudkitchens-public-api-openapi.yml
  format: yaml
  label: CloudKitchens Public API
  slug: cloudkitchens-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudkitchens/refs/heads/main/openapi/cloudkitchens-public-api-openapi.yml
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
method: searched
name: Cloudkitchens Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
overview: CloudKitchens secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode and clientCredentials flow(s).
provider_name: CloudKitchens
provider_slug: cloudkitchens
scheme_count: 1
schemes:
- description: 'The **Authorization API** is based on the [OAuth2.0 protocol](https://tools.ietf.org/html/rfc6749), supporting the (Client Credentials)[https://datatracker.ietf.org/doc/html/rfc6749#section-4.4] and the (Authorization Code)[https://datatracker.ietf.org/doc/html/rfc6749#section-4.1] flows. Resources expect a valid token sent as a `Bearer` token in the HTTP `Authorization` header.

    ### Scopes

    Scopes '
  flows:
  - flow: clientCredentials
    scopes: 27
    tokenUrl: /v1/auth/token
  - authorizationUrl: /v1/auth/oauth2/authorize
    flow: authorizationCode
    scopes: 2
    tokenUrl: /v1/auth/token
  name: OAuth2.0
  sources:
  - openapi/cloudkitchens-public-api-openapi.yml
  type: oauth2
slug: cloudkitchens-authentication
source_filename: cloudkitchens-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-01'\nmethod: searched\nsource: https://developer-guides.cloudkitchens.com/api-reference/\ndocs: https://developer-guides.cloudkitchens.com/api-reference/\nspec_source: openapi/cloudkitchens-public-api-openapi.yml\nidentity_provider:\n  issuer: https://iam.cloudkitchens.com/\n  discovery_url: https://iam.cloudkitchens.com/.well-known/openid-configuration\n  discovery_file: well-known/cloudkitchens-openid-configuration.json\n  authorization_endpoint: https://iam.cloudkitchens.com/api/oauth2/v2/authorize\n  token_endpoint: https://iam.cloudkitchens.com/api/oauth2/v2/token\n  userinfo_endpoint: https://iam.cloudkitchens.com/api/oauth2/v2/userinfo\n  jwks_uri: https://iam.cloudkitchens.com/api/oauth2/v1/keys\n  id_token_signing_alg: RS256\n  response_types_supported:\n  - code\n  note: 'The OIDC provider fronts CloudKitchens user sign-in (including the Developer Portal). The Public API token\n    endpoints declared in the OpenAPI are relative to the partner API\
  \ base URL: /v1/auth/token and /v1/auth/oauth2/authorize.'\ntoken:\n  header: 'Authorization: Bearer <access_token>'\n  lifetime: 30 days\n  reuse: Tokens should be stored and re-used while still valid.\n  credential_delivery: client credentials in the request body or HTTP Basic Auth\n  content_type: application/x-www-form-urlencoded\nstore_context:\n  header: X-Store-Id\n  description: Partner-side identifier of the store the call acts on behalf of; CloudKitchens translates it to the\n    internal store id and validates the application is associated with that store.\ncredential_issuance: Manual, one-time application registration performed by a CloudKitchens Account Representative.\n  Separate Application ID (formerly Partner ID) and Client Secret per environment (production and staging). No self-serve\n  signup.\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - authorizationCode\n  - clientCredentials\nschemes:\n- name: OAuth2.0\n  type: oauth2\n  flows:\n  - flow: clientCredentials\n\
  \    tokenUrl: /v1/auth/token\n    scopes: 27\n  - flow: authorizationCode\n    authorizationUrl: /v1/auth/oauth2/authorize\n    tokenUrl: /v1/auth/token\n    scopes: 2\n  description: 'The **Authorization API** is based on the [OAuth2.0 protocol](https://tools.ietf.org/html/rfc6749),\n    supporting the (Client Credentials)[https://datatracker.ietf.org/doc/html/rfc6749#section-4.4] and the (Authorization\n    Code)[https://datatracker.ietf.org/doc/html/rfc6749#section-4.1] flows. Resources expect a valid token sent\n    as a `Bearer` token in the HTTP `Authorization` header.\n\n    ### Scopes\n\n    Scopes '\n  sources:\n  - openapi/cloudkitchens-public-api-openapi.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cloudkitchens/refs/heads/main/authentication/cloudkitchens-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Restaurant
- Ghost Kitchens
- Food Delivery
- Order Management
- Menu Management
- Storefront
- Delivery
- Reporting
- Loyalty
- Real-Estate
---
