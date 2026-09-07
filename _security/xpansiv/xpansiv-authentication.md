---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: xpansiv-connect-openapi.yml
  format: yaml
  label: Xpansiv Connect API
  slug: xpansiv-connect
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xpansiv/refs/heads/main/openapi/xpansiv-connect-openapi.yml
- filename: xpansiv-managed-solutions-openapi.yml
  format: yaml
  label: Xpansiv Managed Solutions API
  slug: xpansiv-managed-solutions
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xpansiv/refs/heads/main/openapi/xpansiv-managed-solutions-openapi.yml
- filename: xpansiv-nar-registry-client-openapi.yml
  format: yaml
  label: NAR Registry Client API
  slug: xpansiv-nar-registry
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xpansiv/refs/heads/main/openapi/xpansiv-nar-registry-client-openapi.yml
- filename: xpansiv-tigr-registry-client-openapi.yml
  format: yaml
  label: TIGRS Registry Client API
  slug: xpansiv-tigr-registry
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xpansiv/refs/heads/main/openapi/xpansiv-tigr-registry-client-openapi.yml
- filename: xpansiv-optimal-system-openapi.yml
  format: yaml
  label: Xpansiv Optimal Outcomes APIs
  slug: xpansiv-optimal-outcomes
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xpansiv/refs/heads/main/openapi/xpansiv-optimal-system-openapi.yml
- filename: xpansiv-apx-power-markets-file-registry-openapi.yml
  format: yaml
  label: APX Power Markets File Registry API
  slug: xpansiv-apx-power-markets
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/xpansiv/refs/heads/main/openapi/xpansiv-apx-power-markets-file-registry-openapi.yml
auth_types:
- http (bearer)
- http (basic)
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Xpansiv Authentication
name_suffix: Authentication
oauth_flows: []
overview: Xpansiv secures its APIs with http (bearer), http (basic), and apiKey across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Xpansiv
provider_slug: xpansiv
scheme_count: 3
schemes:
- bearerFormat: JWT
  name: bearerToken
  scheme: bearer
  sources:
  - openapi/xpansiv-connect-openapi.yml
  - openapi/xpansiv-managed-solutions-openapi.yml
  - openapi/xpansiv-nar-registry-client-openapi.yml
  - openapi/xpansiv-optimal-file-registry-openapi.yml
  - openapi/xpansiv-optimal-reporting-openapi.yml
  - openapi/xpansiv-optimal-resource-openapi.yml
  - openapi/xpansiv-optimal-system-openapi.yml
  - openapi/xpansiv-optimal-telemetry-openapi.yml
  type: http
- name: basicScheme
  note: The APX Power Markets description declares HTTP Basic as its scheme, but the authentication page documents Basic only on the TOKEN request; application endpoints take the resulting bearer JWT. The contract and the prose disagree; follow the prose.
  scheme: basic
  sources:
  - openapi/xpansiv-apx-power-markets-file-registry-openapi.yml
  type: http
- in: header
  name: JWT
  note: Modelled as an apiKey in the Authorization header rather than as http/bearer. Functionally the same bearer JWT as the NAR description declares.
  parameter: Authorization
  sources:
  - openapi/xpansiv-tigr-registry-client-openapi.yml
  type: apiKey
slug: xpansiv-authentication
source_filename: xpansiv-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-04'\nmethod: searched\nsource: >-\n  Derived from all 11 harvested OpenAPI descriptions, then upgraded from the four\n  authentication pages Xpansiv publishes and the OIDC discovery documents that were\n  fetched live.\ndocs:\n- https://developer.xpansiv.com/developer-portal/xpansiv-connect/getting-started\n- https://developer.xpansiv.com/developer-portal/xpansiv-data/authorization\n- https://developer.xpansiv.com/developer-portal/xpansiv-managed-solutions/authorization\n- https://developer.xpansiv.com/developer-portal/nar-registry/authentication\n- https://developer.xpansiv.com/developer-portal/tigr-registry/authentication\n- https://developer.xpansiv.com/developer-portal/xpansiv-power/rest_api/authentication\nprovider: Xpansiv\nheadline: >-\n  Every Xpansiv REST surface authenticates with `Authorization: Bearer {token}`, but there\n  are FOUR separate credential systems behind that one header and none of their tokens is\n  accepted by another. This is\
  \ the single most important integration fact about Xpansiv\n  and it is a direct consequence of the platform being assembled by acquisition (APX,\n  2022). A client integrating two Xpansiv products needs two sets of credentials from two\n  issuers.\nsummary:\n  types:\n  - http (bearer)\n  - http (basic)\n  - apiKey\n  api_key_in:\n  - header\n  oauth2_declared_in_spec: false\n  note: >-\n    No description declares an oauth2 securityScheme, even though three of the four\n    credential systems ARE OAuth2 flows documented in prose. The specs model the result\n    (a bearer token) rather than the grant, so a code generator reading only the contracts\n    will not produce a working token exchange. That gap is why the prose below matters.\ncredential_systems:\n- id: xpansiv-auth0\n  name: Xpansiv authorization server (Auth0)\n  serves:\n  - Xpansiv Connect API\n  - Xpansiv Data API (SSO accounts)\n  token_endpoint: https://auth.xpansiv.com/oauth/token\n  preprod_token_endpoint: https://auth.preprod.xpansiv.com/oauth/token\n\
  \  discovery: https://auth.xpansiv.com/.well-known/openid-configuration\n  discovery_status: 200\n  jwks_uri: https://auth.xpansiv.com/.well-known/jwks.json\n  grant_type: http://auth0.com/oauth/grant-type/password-realm\n  grant_note: >-\n    An Auth0 vendor extension grant, not a registered IETF grant type. A generic OAuth2\n    client library will not have it built in.\n  parameters:\n    realm: Username-Password-Authentication\n    audience: https://xpansiv/platform\n    scope: 'documented only as the placeholder SCOPE; the successful response the docs\n      show returns \"scope\": \"\"'\n    client_id: issued by Xpansiv\n    client_secret: issued by Xpansiv\n    username: issued by Xpansiv\n    password: issued by Xpansiv\n  token_lifetime: expires_in 86400 (24 hours)\n  credential_issuance: 'Request from Xpansiv — \"To generate bearer token one has request\n    credentials from Xpansiv\"'\n  source: https://developer.xpansiv.com/developer-portal/xpansiv-connect/getting-started\n\
  - id: apx-jwt\n  name: APX OAuth2 authorization server\n  serves:\n  - NAR Registry Client API\n  - TIGRS Registry Client API\n  - APX Power Markets File Registry API\n  token_endpoint: https://apxjwtauthprod.apx.com/oauth/token\n  uat_token_endpoint: https://apxjwtauthuat.apx.com/oauth/token\n  discovery: none published (host returns 403 on every /.well-known/ path)\n  grant_type: password (RFC 6749 section 4.3.2)\n  client_authentication: 'Authorization: Basic {base64(clientId:clientSecret)}'\n  content_type: application/x-www-form-urlencoded\n  form_parameters: [Username, Password, grant_type]\n  returns: [access_token, token_type, grant_type, expires_in, scope]\n  scope_returned: access\n  scope_note: A single fixed value; not requestable and not subdividable. See\n    scopes/xpansiv-scopes.yml.\n  token_lifetime: 'documented as \"short-lived\"; expires_in returned but not documented'\n  auth_failure: 401 with status message \"Bad Request - Invalid Login ID or Password\"\n  credential_issuance:\n\
  \  - NAR — create an API login per the account-holder article at\n    https://nar.zendesk.com/hc/en-us/articles/25002082817175-Account-Holder-API (linked\n    from info.description of the published NAR description)\n  - TIGR — contact the TIGR administrator\n  source: https://developer.xpansiv.com/developer-portal/nar-registry/authentication and\n    https://developer.xpansiv.com/developer-portal/xpansiv-power/rest_api/authentication\n- id: xpansiv-data-native\n  name: Xpansiv Data native login\n  serves:\n  - Xpansiv Data API\n  login: 'GET https://api.data.xpansiv.com/auth/login with HTTP Basic (username:password)'\n  returns: '{ \"token\": ..., \"refreshToken\": ... }'\n  refresh: 'POST https://api.data.xpansiv.com/auth/refresh with {\"refreshToken\": ...}'\n  logout: 'POST https://api.data.xpansiv.com/auth/logout with {\"refreshToken\": ...}'\n  change_password: POST https://api.data.xpansiv.com/auth/changePassword\n  alternative: >-\n    An NG_API_KEY generated in the Xpansiv platform\
  \ may be used instead of\n    username/password (see the Python SDK environment variables). SSO-only accounts must\n    additionally obtain an Auth0 token via https://auth.xpansiv.com/oauth/token with\n    CLIENT_ID and CLIENT_SECRET.\n  refresh_note: >-\n    The only Xpansiv family that publishes a refresh-token flow and an explicit logout.\n    Everywhere else, clients simply re-run the grant.\n  source: https://developer.xpansiv.com/developer-portal/xpansiv-data/authorization\n- id: managed-solutions-key\n  name: Xpansiv Managed Solutions account API key\n  serves:\n  - Xpansiv Managed Solutions API\n  model: long-lived bearer API key, no token endpoint\n  issuance: >-\n    Self-service from inside the account — log in to Xpansiv Managed Solutions, open the\n    API Access page (https://www.ms.xpansiv.com/app/api_access/manage), and under\n    \"Xpansiv Managed Solutions Internal API\" click \"Generate Key\".\n  header: 'Authorization: Bearer {apiKey}'\n  privilege_model: >-\n    The\
  \ provider states the key \"is linked to a user and an account, and has the same\n    rights as\" that user. There is no scoping, no per-endpoint restriction, no read-only\n    variant and no documented rotation or expiry policy. The description does declare\n    ApiKeyCreate/Deactivate/Rotate schemas, so key management exists in the product; the\n    developer docs do not describe a rotation policy.\n  risk_note: >-\n    This is the widest-blast-radius credential in the Xpansiv catalog and the only one an\n    integrator can mint without contacting Xpansiv. Treat it as a full account credential.\n  source: https://developer.xpansiv.com/developer-portal/xpansiv-managed-solutions/authorization\nschemes:\n- name: bearerToken\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/xpansiv-connect-openapi.yml\n  - openapi/xpansiv-managed-solutions-openapi.yml\n  - openapi/xpansiv-nar-registry-client-openapi.yml\n  - openapi/xpansiv-optimal-file-registry-openapi.yml\n\
  \  - openapi/xpansiv-optimal-reporting-openapi.yml\n  - openapi/xpansiv-optimal-resource-openapi.yml\n  - openapi/xpansiv-optimal-system-openapi.yml\n  - openapi/xpansiv-optimal-telemetry-openapi.yml\n- name: basicScheme\n  type: http\n  scheme: basic\n  sources:\n  - openapi/xpansiv-apx-power-markets-file-registry-openapi.yml\n  note: >-\n    The APX Power Markets description declares HTTP Basic as its scheme, but the\n    authentication page documents Basic only on the TOKEN request; application endpoints\n    take the resulting bearer JWT. The contract and the prose disagree; follow the prose.\n- name: JWT\n  type: apiKey\n  in: header\n  parameter: Authorization\n  sources:\n  - openapi/xpansiv-tigr-registry-client-openapi.yml\n  note: Modelled as an apiKey in the Authorization header rather than as http/bearer.\n    Functionally the same bearer JWT as the NAR description declares.\ngaps:\n- api: Transfer Position External API\n  file: openapi/xpansiv-optimal-transfer-position-openapi.yml\n\
  \  issue: >-\n    components.securitySchemes is EMPTY and no security requirement is declared, on the\n    Optimal description with the largest and most sensitive write surface (14 operations\n    including initiateRetirements, initiateAccountTransfers and initiateSubaccountTransfers).\n    The five sibling Optimal descriptions all declare the JWT bearer scheme. A reader of\n    this contract alone would conclude the API is unauthenticated. It is not — the Optimal\n    Outcomes docs state \"Use API credentials to view and manage instruments.\"\n  impact: Code generated from this contract will omit the Authorization header entirely.\nmtls: not declared\nopenid_connect_scheme: not declared in any spec (OIDC discovery is published at\n  https://auth.xpansiv.com/.well-known/openid-configuration)\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/xpansiv/refs/heads/main/authentication/xpansiv-authentication.yml
summary_line: http (bearer)/http (basic)/apiKey · 3 schemes
tags:
- Company
- Environmental Commodities
- Carbon Markets
- Renewable Energy Certificates
- Registries
- Market Data
- Trading
- Energy
- Sustainability
- Climate
---
