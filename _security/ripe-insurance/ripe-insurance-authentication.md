---
api_key_in:
- header
api_specs:
- filename: ripe-insurance-umbraco-content-delivery-openapi.json
  format: json
  label: Ripe Insurance Umbraco Content Delivery API
  slug: ripe-insurance-umbraco-content-delivery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ripe-insurance/refs/heads/main/openapi/ripe-insurance-umbraco-content-delivery-openapi.json
- filename: ripe-insurance-cycleplan-content-delivery-openapi.json
  format: json
  label: Cycleplan Umbraco Content Delivery API
  slug: ripe-insurance-cycleplan-content-delivery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ripe-insurance/refs/heads/main/openapi/ripe-insurance-cycleplan-content-delivery-openapi.json
auth_types:
- none
- apiKey
- oauth2
- openIdConnect
description: ''
kind: authentication
layout: security
method: searched
name: Ripe Insurance Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
- refreshToken
overview: Ripe Insurance secures its APIs with none, apiKey, oauth2, and openIdConnect across 3 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, clientCredentials, and refreshToken flow(s).
provider_name: Ripe Insurance
provider_slug: ripe-insurance
scheme_count: 3
schemes:
- description: The Content Delivery API is served anonymously. All eight v2 operations on ripeinsurance.co.uk (and sixteen v1+v2 operations on cycleplan.co.uk) return 200 with no credential. Verified live 2026-07-25 against /umbraco/delivery/api/v2/content (345 content items returned).
  name: anonymous
  sources:
  - openapi/ripe-insurance-umbraco-content-delivery-openapi.json
  - openapi/ripe-insurance-cycleplan-content-delivery-openapi.json
  type: none
- declared_as_security_scheme: false
  description: Umbraco platform feature. Declared in the specification as an optional request header on every operation ("API key specified through configuration to authorize access to the API") rather than in components.securitySchemes. It gates configuration-level access to the Delivery API. Ripe publishes no way to obtain one.
  in: header
  name: Api-Key
  parameter_name: Api-Key
  sources:
  - openapi/ripe-insurance-umbraco-content-delivery-openapi.json
  - openapi/ripe-insurance-cycleplan-content-delivery-openapi.json
  type: apiKey
- client_registration:
    dynamic: false
    note: No RFC 7591 registration_endpoint is advertised. Clients are configured server-side.
  description: The Umbraco/OpenIddict member-authentication server behind the Ripe Insurance customer login (www.ripeinsurance.co.uk/login redirects to account.ripeinsurance.co.uk). It protects member-only website content, including member-protected items served by the Content Delivery API — the reason GetContentItemById2.0 and GetContentItemByPath2.0 declare 401 and 403 responses. It is a consumer login system, not a partner API authorization server.
  endpoints:
    authorization: https://www.ripeinsurance.co.uk/umbraco/delivery/api/v1/security/member/authorize
    end_session: https://www.ripeinsurance.co.uk/umbraco/delivery/api/v1/security/member/signout
    jwks: https://www.ripeinsurance.co.uk/.well-known/jwks
    revocation: https://www.ripeinsurance.co.uk/umbraco/delivery/api/v1/security/member/revoke
    token: https://www.ripeinsurance.co.uk/umbraco/delivery/api/v1/security/member/token
    userinfo: https://www.ripeinsurance.co.uk/umbraco/delivery/api/v1/security/member/userinfo
  grant_types:
  - authorization_code
  - refresh_token
  - client_credentials
  id_token_signing_alg_values:
  - RS256
  issuer: https://www.ripeinsurance.co.uk/
  mtls_bound_tokens: false
  name: umbraco-member-oidc
  openIdConnectUrl: https://www.ripeinsurance.co.uk/.well-known/openid-configuration
  par_required: false
  peer_issuers:
  - https://www.cycleplan.co.uk/
  - https://www.golfcare.co.uk/
  - https://www.insure4sport.co.uk/
  pkce:
    code_challenge_methods:
    - plain
    - S256
    supported: true
  response_types:
  - code
  scopes_supported:
  - openid
  - offline_access
  sources:
  - well-known/ripe-insurance-openid-configuration.json
  token_endpoint_auth_methods:
  - client_secret_post
  - private_key_jwt
  - client_secret_basic
  type: openIdConnect
slug: ripe-insurance-authentication
source_filename: ripe-insurance-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-25'\nmethod: searched\nsource: >-\n  https://www.ripeinsurance.co.uk/.well-known/openid-configuration (fetched 2026-07-25),\n  openapi/ripe-insurance-umbraco-content-delivery-openapi.json,\n  openapi/ripe-insurance-cycleplan-content-delivery-openapi.json,\n  https://docs.umbraco.com/umbraco-cms/reference/content-delivery-api\ndocs: https://docs.umbraco.com/umbraco-cms/reference/content-delivery-api#protected-content\nsummary:\n  types: [none, apiKey, oauth2, openIdConnect]\n  api_key_in: [header]\n  oauth2_flows: [authorizationCode, clientCredentials, refreshToken]\n  developer_credentials_available: false\n  note: >-\n    Ripe Insurance issues NO developer or partner credentials. There is no sign-up for\n    API access, no key-management console and no client-registration endpoint. What\n    exists is (a) an anonymous, unauthenticated read surface on the Umbraco Content\n    Delivery API and (b) an OpenID Connect server for website customer login. The\n\
  \    apiKey scheme below is an optional Umbraco platform feature declared as a header\n    parameter in the specification — it is NOT declared as an OpenAPI securityScheme\n    and no key is obtainable by an outside developer.\nschemes:\n- name: anonymous\n  type: none\n  description: >-\n    The Content Delivery API is served anonymously. All eight v2 operations on\n    ripeinsurance.co.uk (and sixteen v1+v2 operations on cycleplan.co.uk) return 200\n    with no credential. Verified live 2026-07-25 against\n    /umbraco/delivery/api/v2/content (345 content items returned).\n  sources:\n  - openapi/ripe-insurance-umbraco-content-delivery-openapi.json\n  - openapi/ripe-insurance-cycleplan-content-delivery-openapi.json\n- name: Api-Key\n  type: apiKey\n  in: header\n  parameter_name: Api-Key\n  declared_as_security_scheme: false\n  description: >-\n    Umbraco platform feature. Declared in the specification as an optional request\n    header on every operation (\"API key specified through\
  \ configuration to authorize\n    access to the API\") rather than in components.securitySchemes. It gates\n    configuration-level access to the Delivery API. Ripe publishes no way to obtain\n    one.\n  sources:\n  - openapi/ripe-insurance-umbraco-content-delivery-openapi.json\n  - openapi/ripe-insurance-cycleplan-content-delivery-openapi.json\n- name: umbraco-member-oidc\n  type: openIdConnect\n  openIdConnectUrl: https://www.ripeinsurance.co.uk/.well-known/openid-configuration\n  description: >-\n    The Umbraco/OpenIddict member-authentication server behind the Ripe Insurance\n    customer login (www.ripeinsurance.co.uk/login redirects to\n    account.ripeinsurance.co.uk). It protects member-only website content, including\n    member-protected items served by the Content Delivery API — the reason\n    GetContentItemById2.0 and GetContentItemByPath2.0 declare 401 and 403 responses.\n    It is a consumer login system, not a partner API authorization server.\n  issuer: https://www.ripeinsurance.co.uk/\n\
  \  endpoints:\n    authorization: https://www.ripeinsurance.co.uk/umbraco/delivery/api/v1/security/member/authorize\n    token: https://www.ripeinsurance.co.uk/umbraco/delivery/api/v1/security/member/token\n    userinfo: https://www.ripeinsurance.co.uk/umbraco/delivery/api/v1/security/member/userinfo\n    end_session: https://www.ripeinsurance.co.uk/umbraco/delivery/api/v1/security/member/signout\n    revocation: https://www.ripeinsurance.co.uk/umbraco/delivery/api/v1/security/member/revoke\n    jwks: https://www.ripeinsurance.co.uk/.well-known/jwks\n  grant_types: [authorization_code, refresh_token, client_credentials]\n  response_types: [code]\n  scopes_supported: [openid, offline_access]\n  pkce:\n    supported: true\n    code_challenge_methods: [plain, S256]\n  token_endpoint_auth_methods: [client_secret_post, private_key_jwt, client_secret_basic]\n  id_token_signing_alg_values: [RS256]\n  par_required: false\n  mtls_bound_tokens: false\n  client_registration:\n    dynamic: false\n\
  \    note: No RFC 7591 registration_endpoint is advertised. Clients are configured server-side.\n  sources:\n  - well-known/ripe-insurance-openid-configuration.json\n  peer_issuers:\n  - https://www.cycleplan.co.uk/\n  - https://www.golfcare.co.uk/\n  - https://www.insure4sport.co.uk/\ninsurance_api_auth:\n  present: false\n  note: >-\n    No quote, bind, issue, policy, billing or FNOL API is published, so no\n    authentication model exists for one. Partnering runs through a business-development\n    enquiry form at https://www.ripethinking.co.uk/partner-with-us/.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ripe-insurance/refs/heads/main/authentication/ripe-insurance-authentication.yml
summary_line: none/apiKey/oauth2/openIdConnect · 3 schemes
tags:
- Insurance
- United Kingdom
- Insurtech
- Managing General Agent
- Specialist Insurance
- Personal Lines
- Small Business Insurance
- Underwriting
- Direct to Consumer
- Brokers
---
