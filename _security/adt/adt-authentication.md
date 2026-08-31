---
api_key_in: []
api_specs:
- filename: adt-access-codes-api-openapi.yml
  format: yaml
  label: ADT Access Codes API
  slug: adt-access-codes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adt/refs/heads/main/openapi/adt-access-codes-api-openapi.yml
- filename: adt-access-control-api-openapi.yml
  format: yaml
  label: ADT Access Control API
  slug: adt-access-control-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adt/refs/heads/main/openapi/adt-access-control-api-openapi.yml
- filename: adt-automation-api-openapi.yml
  format: yaml
  label: ADT Automation API
  slug: adt-automation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adt/refs/heads/main/openapi/adt-automation-api-openapi.yml
- filename: adt-devices-api-openapi.yml
  format: yaml
  label: ADT Devices API
  slug: adt-devices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adt/refs/heads/main/openapi/adt-devices-api-openapi.yml
- filename: adt-events-api-openapi.yml
  format: yaml
  label: ADT Events API
  slug: adt-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adt/refs/heads/main/openapi/adt-events-api-openapi.yml
- filename: adt-reports-api-openapi.yml
  format: yaml
  label: ADT Reports API
  slug: adt-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adt/refs/heads/main/openapi/adt-reports-api-openapi.yml
- filename: adt-security-systems-api-openapi.yml
  format: yaml
  label: ADT Security Systems API
  slug: adt-security-systems-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adt/refs/heads/main/openapi/adt-security-systems-api-openapi.yml
- filename: adt-sites-api-openapi.yml
  format: yaml
  label: ADT Sites API
  slug: adt-sites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adt/refs/heads/main/openapi/adt-sites-api-openapi.yml
- filename: adt-users-api-openapi.yml
  format: yaml
  label: ADT Users API
  slug: adt-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adt/refs/heads/main/openapi/adt-users-api-openapi.yml
- filename: adt-video-api-openapi.yml
  format: yaml
  label: ADT Video API
  slug: adt-video-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/adt/refs/heads/main/openapi/adt-video-api-openapi.yml
auth_types:
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: probed
name: Adt Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- implicit
- refresh_token
overview: ADT secures its APIs with oauth2 and openIdConnect across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, implicit, and refresh_token flow(s).
provider_name: ADT
provider_slug: adt
scheme_count: 1
schemes:
- authorizationUrl: https://auth.adt.com/services/oauth2/authorize
  dpop_signing_algs:
  - RS256
  - RS384
  - RS512
  - ES256
  - ES384
  - ES512
  - EdDSA
  endSessionUrl: https://auth.adt.com/services/auth/idp/oidc/logout
  id_token_signing_algs:
  - RS256
  introspectionUrl: https://auth.adt.com/services/oauth2/introspect
  issuer: https://auth.adt.com
  jwksUri: https://auth.adt.com/id/keys
  name: openIdConnect
  openIdConnectUrl: https://auth.adt.com/.well-known/openid-configuration
  registrationUrl: https://auth.adt.com/services/oauth2/register
  response_types:
  - code
  - token
  - token id_token
  revocationUrl: https://auth.adt.com/services/oauth2/revoke
  scopes_supported: 36
  sources:
  - well-known/adt-openid-configuration.json
  tokenUrl: https://auth.adt.com/services/oauth2/token
  token_endpoint_auth_methods:
  - client_secret_post
  - client_secret_basic
  - private_key_jwt
  type: openIdConnect
  userinfoUrl: https://auth.adt.com/services/oauth2/userinfo
slug: adt-authentication
source_filename: adt-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-30'\nmethod: probed\nsource: >-\n  https://auth.adt.com/.well-known/openid-configuration (HTTP 200, fetched 2026-08-30,\n  saved verbatim to well-known/adt-openid-configuration.json). Supersedes the 2026-07-11\n  profile, which was derived from OpenAPI documents API Evangelist authored (now in\n  openapi/_ae-authored/) rather than from anything ADT published.\nprovider: ADT\nproviderId: adt\nsummary:\n  types:\n  - oauth2\n  - openIdConnect\n  oauth2_flows:\n  - authorizationCode\n  - implicit\n  - refresh_token\n  discovery: https://auth.adt.com/.well-known/openid-configuration\n  note: >-\n    The only authentication surface ADT serves anonymously is the OpenID Connect provider\n    behind its CUSTOMER portal (auth.adt.com, Salesforce Experience Cloud, issuer\n    \"https://auth.adt.com\"). It authenticates ADT customers into ADT's own web\n    application. It is not a developer-API authorization server, and no ADT developer\n    program exists to issue\
  \ client credentials against it.\nschemes:\n- name: openIdConnect\n  type: openIdConnect\n  openIdConnectUrl: https://auth.adt.com/.well-known/openid-configuration\n  issuer: https://auth.adt.com\n  authorizationUrl: https://auth.adt.com/services/oauth2/authorize\n  tokenUrl: https://auth.adt.com/services/oauth2/token\n  userinfoUrl: https://auth.adt.com/services/oauth2/userinfo\n  revocationUrl: https://auth.adt.com/services/oauth2/revoke\n  introspectionUrl: https://auth.adt.com/services/oauth2/introspect\n  registrationUrl: https://auth.adt.com/services/oauth2/register\n  jwksUri: https://auth.adt.com/id/keys\n  endSessionUrl: https://auth.adt.com/services/auth/idp/oidc/logout\n  response_types:\n  - code\n  - token\n  - token id_token\n  token_endpoint_auth_methods:\n  - client_secret_post\n  - client_secret_basic\n  - private_key_jwt\n  id_token_signing_algs:\n  - RS256\n  dpop_signing_algs:\n  - RS256\n  - RS384\n  - RS512\n  - ES256\n  - ES384\n  - ES512\n  - EdDSA\n  scopes_supported:\
  \ 36\n  sources:\n  - well-known/adt-openid-configuration.json\ncorrections:\n  - claim: >-\n      The 2026-07-11 profile recorded tokenUrl https://auth.adt.com/oauth/token and\n      authorizationUrl https://auth.adt.com/oauth/authorize, with clientCredentials and\n      authorizationCode flows.\n    finding: >-\n      Those URLs do not exist. They came from OpenAPI documents API Evangelist wrote, not\n      from ADT. ADT's real, published discovery document names\n      /services/oauth2/authorize and /services/oauth2/token, and advertises no\n      client_credentials grant. Corrected here.\nunverified:\n  - surface: https://api.adt.com/\n    finding: >-\n      api.adt.com is a live ADT host — TLS completes against a Sectigo OV certificate whose\n      subject is CN=api.adt.com, O=ADT LLC, valid 2026-06-25 to 2027-01-09, so ADT LLC\n      actively maintains it — but the origin returns zero bytes to any anonymous HTTP\n      request. Its authentication scheme is therefore unknown and is\
  \ NOT asserted here.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/adt/refs/heads/main/authentication/adt-authentication.yml
summary_line: oauth2/openIdConnect · 1 scheme
tags:
- Access Control
- Automation
- Home Security
- IoT
- Monitoring
- Security
- Smart Home
- Fortune 1000
---
