---
api_key_in:
- header
auth_types:
- http-bearer
- oauth2
- openIdConnect
- saml
- apiKey-signed
description: 'Spark Platform''s authentication profile. There is no OpenAPI to derive securitySchemes from, so this profile is read from the published authentication documentation plus the one machine-readable identity document Spark serves anonymously — its OpenID Connect discovery document. Four mechanisms are documented: an OAuth 2 / MLS-issued Bearer access token (the normal path for data access), OpenID Connect (member identity, MLS approval required), SAML (service-provider integration with flexmls Web), and a legacy signed-request API key. Every data endpoint returns HTTP 401 with Spark code 1000 when called anonymously.'
kind: authentication
layout: security
method: searched
name: Spark Platform Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: Spark Platform secures its APIs with http-bearer, oauth2, openIdConnect, saml, and apiKey-signed across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: Spark Platform
provider_slug: spark-platform
scheme_count: 4
schemes:
- applies_to:
  - Spark API
  - Spark RESO Web API
  docs: https://sparkplatform.com/docs/authentication/access_token
  format: 'Authorization: Bearer <your_access_token>'
  in: header
  issued_by: OAuth 2 authorization, or a non-expiring access token issued by the MLS alongside an OAuth key (API feed ID). The same token authorizes both the Spark API and the RESO Web API endpoints.
  name: Bearer access token
  parameter: Authorization
  required_with: Accept header; HTTPS required (code 1030 otherwise)
  scheme: bearer
  type: http
- authorizationUrl: https://sparkplatform.com/openid/authorize
  claims_parameter_supported: true
  docs: https://sparkplatform.com/docs/authentication/openid_connect_authentication
  gate: Requires separate MLS approval before OIDC keys are issued.
  harvested: authentication/spark-platform-openid-configuration.json
  id_token_signing_alg:
  - RS256
  issuer: https://sparkplatform.com
  jwks_uri: https://sparkplatform.com/openid/jwks.json
  name: OpenID Connect
  note: The claim set is real-estate specific and encodes the licensing substrate itself — MemberMlsId, MemberNrdsId, MemberStateLicense, MemberAOR/MemberAORkey, MemberPrimaryAorId, MemberType, MemberStatus, OfficeKey/OfficeMlsId, FlexmlsMemberType and mls_system_access. This is the only machine-readable contract Spark serves without credentials.
  openIdConnectUrl: https://sparkplatform.com/.well-known/openid-configuration
  response_types:
  - code
  - id_token
  - id_token token
  - code token
  - id_token code
  - id_token code token
  revocationUrl: https://sparkplatform.com/openid/revoke
  scope_detail: scopes/spark-platform-scopes.yml
  scopes:
  - openid
  - profile
  - email
  - address
  - phone
  - RESO
  - FBS
  subject_types:
  - public
  - pairwise
  tokenUrl: https://sparkplatform.com/openid/token
  token_endpoint_auth_methods:
  - client_secret_post
  - client_secret_basic
  type: openIdConnect
  userinfoUrl: https://sparkplatform.com/openid/userinfo
- docs: https://sparkplatform.com/docs/authentication/saml
  name: SAML
  note: SAML service-provider integration with flexmls Web for member single sign-on.
  type: saml
- documented: partial
  in: header
  name: Legacy API key with request signing
  note: Evidenced by the 401 body returned by both sparkapi.com/v1 and the OData endpoints — "Invalid API key and/or request signed improperly" (code 1000) — and by the Supplemental Authentication Services page in the docs navigation. Superseded by the Bearer token flow for new integrations.
  type: apiKey
slug: spark-platform-authentication
source_filename: spark-platform-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-26'\nmethod: searched\nsource: >-\n  https://sparkplatform.com/docs/authentication/access_token,\n  https://sparkplatform.com/docs/authentication/openid_connect_authentication,\n  https://sparkplatform.com/docs/authentication/saml,\n  https://sparkplatform.com/.well-known/openid-configuration (HTTP 200, harvested verbatim to\n  authentication/spark-platform-openid-configuration.json).\ndocs: https://sparkplatform.com/docs/authentication/authentication\ndescription: >-\n  Spark Platform's authentication profile. There is no OpenAPI to derive securitySchemes from,\n  so this profile is read from the published authentication documentation plus the one\n  machine-readable identity document Spark serves anonymously — its OpenID Connect discovery\n  document. Four mechanisms are documented: an OAuth 2 / MLS-issued Bearer access token (the\n  normal path for data access), OpenID Connect (member identity, MLS approval required), SAML\n  (service-provider integration\
  \ with flexmls Web), and a legacy signed-request API key. Every\n  data endpoint returns HTTP 401 with Spark code 1000 when called anonymously.\nsummary:\n  types: [http-bearer, oauth2, openIdConnect, saml, apiKey-signed]\n  api_key_in: [header]\n  oauth2_flows: [authorizationCode]\n\nschemes:\n  - name: Bearer access token\n    type: http\n    scheme: bearer\n    in: header\n    parameter: Authorization\n    format: \"Authorization: Bearer <your_access_token>\"\n    issued_by: >-\n      OAuth 2 authorization, or a non-expiring access token issued by the MLS alongside an\n      OAuth key (API feed ID). The same token authorizes both the Spark API and the RESO Web\n      API endpoints.\n    required_with: Accept header; HTTPS required (code 1030 otherwise)\n    docs: https://sparkplatform.com/docs/authentication/access_token\n    applies_to: [Spark API, Spark RESO Web API]\n\n  - name: OpenID Connect\n    type: openIdConnect\n    openIdConnectUrl: https://sparkplatform.com/.well-known/openid-configuration\n\
  \    issuer: https://sparkplatform.com\n    authorizationUrl: https://sparkplatform.com/openid/authorize\n    tokenUrl: https://sparkplatform.com/openid/token\n    userinfoUrl: https://sparkplatform.com/openid/userinfo\n    revocationUrl: https://sparkplatform.com/openid/revoke\n    jwks_uri: https://sparkplatform.com/openid/jwks.json\n    id_token_signing_alg: [RS256]\n    token_endpoint_auth_methods: [client_secret_post, client_secret_basic]\n    response_types: [code, id_token, \"id_token token\", \"code token\", \"id_token code\", \"id_token code token\"]\n    subject_types: [public, pairwise]\n    claims_parameter_supported: true\n    scopes: [openid, profile, email, address, phone, RESO, FBS]\n    scope_detail: scopes/spark-platform-scopes.yml\n    gate: Requires separate MLS approval before OIDC keys are issued.\n    docs: https://sparkplatform.com/docs/authentication/openid_connect_authentication\n    note: >-\n      The claim set is real-estate specific and encodes the licensing\
  \ substrate itself —\n      MemberMlsId, MemberNrdsId, MemberStateLicense, MemberAOR/MemberAORkey,\n      MemberPrimaryAorId, MemberType, MemberStatus, OfficeKey/OfficeMlsId, FlexmlsMemberType\n      and mls_system_access. This is the only machine-readable contract Spark serves without\n      credentials.\n    harvested: authentication/spark-platform-openid-configuration.json\n\n  - name: SAML\n    type: saml\n    docs: https://sparkplatform.com/docs/authentication/saml\n    note: SAML service-provider integration with flexmls Web for member single sign-on.\n\n  - name: Legacy API key with request signing\n    type: apiKey\n    in: header\n    documented: partial\n    note: >-\n      Evidenced by the 401 body returned by both sparkapi.com/v1 and the OData endpoints —\n      \"Invalid API key and/or request signed improperly\" (code 1000) — and by the\n      Supplemental Authentication Services page in the docs navigation. Superseded by the\n      Bearer token flow for new integrations.\n\
  \nsession_semantics:\n  session_token_expiry: Code 1020 \"Session token has expired\" on expired session tokens.\n  key_restrictions:\n    - Keys can be restricted to specific IP addresses and/or User-Agent values (code 1019).\n    - Keys can be read-only; POST/PUT/DELETE then return code 1017.\n    - Keys can be restricted to replication.sparkapi.com (code 1021).\n    - Auth mechanism itself can be restricted per key (code 1013).\n\nauthorization_model:\n  mechanism: role-scoped keys\n  roles: [IDX, VOW, Private, Broker/Agent own data, Public, Portal]\n  note: >-\n    Authorization is not scope-based on the data API. What a valid token can see is determined\n    by the role assigned to its key and by which MLS data plans the developer has been approved\n    for. OAuth scopes exist only on the OpenID Connect identity surface.\n  docs: https://sparkplatform.com/docs/supporting_documentation/roles\n\naccess_gate:\n  classification: licence-agreement\n  note: >-\n    Credentials are not self-serve.\
  \ Free public developer registration yields demo credentials\n    only; production MLS data requires a signed FBS Developer Agreement, a role assignment and\n    an MLS-approved data plan purchased through the Spark Datamart at USD 50/month per MLS.\n  docs: https://sparkplatform.com/docs/overview/set_up_access\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/spark-platform/refs/heads/main/authentication/spark-platform-authentication.yml
summary_line: http-bearer/oauth2/openIdConnect/saml/apiKey-signed · 4 schemes
tags:
- Real Estate
- United States
- MLS
- RESO
- Property Listings
- IDX
- PropTech
- Listing Data Infrastructure
- OData
---
