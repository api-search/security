---
api_key_in: []
api_specs:
- filename: target-inventory-api-openapi.yml
  format: yaml
  label: target Inventory API
  slug: target-inventory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/target/refs/heads/main/openapi/target-inventory-api-openapi.yml
- filename: target-orders-api-openapi.yml
  format: yaml
  label: target Orders API
  slug: target-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/target/refs/heads/main/openapi/target-orders-api-openapi.yml
- filename: target-products-api-openapi.yml
  format: yaml
  label: target Products API
  slug: target-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/target/refs/heads/main/openapi/target-products-api-openapi.yml
- filename: target-search-api-openapi.yml
  format: yaml
  label: target Search API
  slug: target-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/target/refs/heads/main/openapi/target-search-api-openapi.yml
- filename: target-status-api-openapi.yml
  format: yaml
  label: target Status API
  slug: target-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/target/refs/heads/main/openapi/target-status-api-openapi.yml
- filename: target-stores-api-openapi.yml
  format: yaml
  label: target Stores API
  slug: target-stores-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/target/refs/heads/main/openapi/target-stores-api-openapi.yml
auth_types:
- oauth2
- openIdConnect
description: Target runs two separate OpenID Connect issuers, both of which publish an anonymous discovery document. oauth.iam.target.com fronts the corporate identity domain used by developer.target.com (the internal/partner API developer portal). oauth.iam.partnersonline.com fronts Target Partners Online, the supplier and vendor portal. The two documents are identical in shape and differ only in issuer and endpoint host. Neither issuer serves an RFC 8414 oauth-authorization-server document; discovery is OIDC-only. Target publishes no anonymous API key or bearer-token program — every credential is issued through a Target relationship (employee, vendor, Target Plus partner).
kind: authentication
layout: security
method: searched
name: Target Authentication
name_suffix: Authentication
oauth_flows: []
overview: target secures its APIs with oauth2 and openIdConnect across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: target
provider_slug: target
scheme_count: 3
schemes:
- audience: Target team members and trusted third parties with an existing Target relationship
  authorization_endpoint: https://oauth.iam.target.com/auth/oauth/v2/authorize
  file: well-known/target-oauth-iam-target-openid-configuration.json
  grant_types_supported:
  - authorization_code
  - implicit
  id_token_signing_alg_values_supported:
  - RS256
  - HS256
  issuer: https://oauth.iam.target.com
  jwks_uri: https://oauth.iam.target.com/openid/connect/jwks.json
  method: searched
  name: targetIamOidc
  openIdConnectUrl: https://oauth.iam.target.com/.well-known/openid-configuration
  registration_endpoint: https://oauth.iam.target.com/openid/connect/register
  response_types_supported:
  - code
  - token id_token
  scopes_supported:
  - openid
  - email
  - profile
  - openid_client_registration
  subject_types_supported:
  - pairwise
  token_endpoint: https://oauth.iam.target.com/auth/oauth/v2/token
  token_endpoint_auth_methods_supported:
  - client_secret_basic
  - client_secret_post
  type: openIdConnect
  userinfo_endpoint: https://oauth.iam.target.com/openid/connect/v1/target/userinfo
  x-evidence:
    content_type: application/json
    fetched: '2026-08-27'
    http_status: 200
    jwks_http_status: 200
    url: https://oauth.iam.target.com/.well-known/openid-configuration
- audience: Target suppliers, vendors and Target Plus marketplace partners
  authorization_endpoint: https://oauth.iam.partnersonline.com/auth/oauth/v2/authorize
  file: well-known/target-oauth-iam-partnersonline-openid-configuration.json
  grant_types_supported:
  - authorization_code
  - implicit
  id_token_signing_alg_values_supported:
  - RS256
  - HS256
  issuer: https://oauth.iam.partnersonline.com
  jwks_uri: https://oauth.iam.partnersonline.com/openid/connect/jwks.json
  method: searched
  name: partnersOnlineOidc
  openIdConnectUrl: https://oauth.iam.partnersonline.com/.well-known/openid-configuration
  registration_endpoint: https://oauth.iam.partnersonline.com/openid/connect/register
  response_types_supported:
  - code
  - token id_token
  scopes_supported:
  - openid
  - email
  - profile
  - openid_client_registration
  subject_types_supported:
  - pairwise
  token_endpoint: https://oauth.iam.partnersonline.com/auth/oauth/v2/token
  token_endpoint_auth_methods_supported:
  - client_secret_basic
  - client_secret_post
  type: openIdConnect
  userinfo_endpoint: https://oauth.iam.partnersonline.com/openid/connect/v1/target/userinfo
  x-evidence:
    content_type: application/json
    fetched: '2026-08-27'
    http_status: 200
    url: https://oauth.iam.partnersonline.com/.well-known/openid-configuration
- description: The developer.target.com catalog backend rejects anonymous calls with HTTP 401 and the body {"message":"Invalid Key","errors":[{"resource":"Go-Proxy","reason":"no API key ..."}]}, so an API key issued through the portal is the credential for the catalog itself. The header name is not disclosed anonymously.
  in: header
  method: probed
  name: developerPortalApiKey
  type: apiKey
  x-evidence:
    body_signature: 'message: Invalid Key / resource: Go-Proxy'
    fetched: '2026-08-27'
    http_status: 401
    url: https://developer.target.com/api/docs/v1/docs/
slug: target-authentication
source_filename: target-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-27'\nmethod: searched\nsource: https://oauth.iam.target.com/.well-known/openid-configuration\ndocs: https://logonservices.oauth.iam.partnersonline.com/guide/\ndescription: >-\n  Target runs two separate OpenID Connect issuers, both of which publish an anonymous discovery\n  document. oauth.iam.target.com fronts the corporate identity domain used by developer.target.com\n  (the internal/partner API developer portal). oauth.iam.partnersonline.com fronts Target Partners\n  Online, the supplier and vendor portal. The two documents are identical in shape and differ only\n  in issuer and endpoint host. Neither issuer serves an RFC 8414 oauth-authorization-server document;\n  discovery is OIDC-only. Target publishes no anonymous API key or bearer-token program — every\n  credential is issued through a Target relationship (employee, vendor, Target Plus partner).\nsummary:\n  types:\n  - oauth2\n  - openIdConnect\n  issuers: 2\n  anonymous_registration: false\nschemes:\n\
  - name: targetIamOidc\n  type: openIdConnect\n  method: searched\n  openIdConnectUrl: https://oauth.iam.target.com/.well-known/openid-configuration\n  issuer: https://oauth.iam.target.com\n  authorization_endpoint: https://oauth.iam.target.com/auth/oauth/v2/authorize\n  token_endpoint: https://oauth.iam.target.com/auth/oauth/v2/token\n  userinfo_endpoint: https://oauth.iam.target.com/openid/connect/v1/target/userinfo\n  jwks_uri: https://oauth.iam.target.com/openid/connect/jwks.json\n  registration_endpoint: https://oauth.iam.target.com/openid/connect/register\n  grant_types_supported:\n  - authorization_code\n  - implicit\n  response_types_supported:\n  - code\n  - token id_token\n  scopes_supported:\n  - openid\n  - email\n  - profile\n  - openid_client_registration\n  token_endpoint_auth_methods_supported:\n  - client_secret_basic\n  - client_secret_post\n  id_token_signing_alg_values_supported:\n  - RS256\n  - HS256\n  subject_types_supported:\n  - pairwise\n  audience: Target team\
  \ members and trusted third parties with an existing Target relationship\n  file: well-known/target-oauth-iam-target-openid-configuration.json\n  x-evidence:\n    fetched: '2026-08-27'\n    url: https://oauth.iam.target.com/.well-known/openid-configuration\n    http_status: 200\n    content_type: application/json\n    jwks_http_status: 200\n- name: partnersOnlineOidc\n  type: openIdConnect\n  method: searched\n  openIdConnectUrl: https://oauth.iam.partnersonline.com/.well-known/openid-configuration\n  issuer: https://oauth.iam.partnersonline.com\n  authorization_endpoint: https://oauth.iam.partnersonline.com/auth/oauth/v2/authorize\n  token_endpoint: https://oauth.iam.partnersonline.com/auth/oauth/v2/token\n  userinfo_endpoint: https://oauth.iam.partnersonline.com/openid/connect/v1/target/userinfo\n  jwks_uri: https://oauth.iam.partnersonline.com/openid/connect/jwks.json\n  registration_endpoint: https://oauth.iam.partnersonline.com/openid/connect/register\n  grant_types_supported:\n \
  \ - authorization_code\n  - implicit\n  response_types_supported:\n  - code\n  - token id_token\n  scopes_supported:\n  - openid\n  - email\n  - profile\n  - openid_client_registration\n  token_endpoint_auth_methods_supported:\n  - client_secret_basic\n  - client_secret_post\n  id_token_signing_alg_values_supported:\n  - RS256\n  - HS256\n  subject_types_supported:\n  - pairwise\n  audience: Target suppliers, vendors and Target Plus marketplace partners\n  file: well-known/target-oauth-iam-partnersonline-openid-configuration.json\n  x-evidence:\n    fetched: '2026-08-27'\n    url: https://oauth.iam.partnersonline.com/.well-known/openid-configuration\n    http_status: 200\n    content_type: application/json\n- name: developerPortalApiKey\n  type: apiKey\n  in: header\n  method: probed\n  description: >-\n    The developer.target.com catalog backend rejects anonymous calls with HTTP 401 and the body\n    {\"message\":\"Invalid Key\",\"errors\":[{\"resource\":\"Go-Proxy\",\"reason\":\"no\
  \ API key ...\"}]}, so an\n    API key issued through the portal is the credential for the catalog itself. The header name is\n    not disclosed anonymously.\n  x-evidence:\n    fetched: '2026-08-27'\n    url: https://developer.target.com/api/docs/v1/docs/\n    http_status: 401\n    body_signature: 'message: Invalid Key / resource: Go-Proxy'\ngaps:\n- id: service-documentation-404\n  detail: >-\n    Both discovery documents advertise service_documentation (a Swagger definition for the OAuth v2\n    service). Both URLs return 404. See well-known/target-well-known.yml findings[].\n- id: no-rfc8414\n  detail: Neither issuer serves /.well-known/oauth-authorization-server (both 404); discovery is OIDC-only.\nunverified_prior_claims:\n- scheme: bearerAuth\n  detail: >-\n    Earlier rounds derived an http/bearer JWT scheme from openapi/target-target-api-openapi.yml.\n    That spec is an API Evangelist scaffold, not a Target-published contract (see\n    openapi/PROVENANCE.md), so the bearer scheme\
  \ is NOT carried forward as evidenced.\nmaintainers:\n- FN: Kin Lane\n  email: kin@apievangelist.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/target/refs/heads/main/authentication/target-authentication.yml
summary_line: oauth2/openIdConnect · 3 schemes
tags:
- Fortune 100
- E-Commerce
- Retail
- Product
- Inventory
- Stores
- Order
---
