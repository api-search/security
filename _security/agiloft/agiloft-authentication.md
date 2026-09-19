---
anonymous_access: false
api_key_in:
- query
- body
auth_types:
- oauth2
- http
- apiKey
description: ''
kind: authentication
layout: security
mechanism_count: 7
method: searched
name: Agiloft Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- authorizationCodePKCE
- clientCredentials
overview: Agiloft secures its APIs with oauth2, http, and apiKey across 7 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, authorizationCodePKCE, and clientCredentials flow(s).
provider_name: Agiloft
provider_slug: agiloft
scheme_count: 7
schemes:
- authorizationUrl: https://{hostname}/ewws/oauth
  authorization_code_lifetime: 5 minutes
  docs: https://help.agiloft.com/space/HELP/43716464/Use%20OAuth2%20to%20Access%20REST%20API
  flow: authorizationCode
  grant_types:
  - authorization_code
  name: OAuth2AuthorizationCode
  note: Client registration happens in the KB at Setup > Integration > OAuth2 Client Setup. Each OAuth client is bound to one native Agiloft service-user account and every call made with its tokens runs as that account. Reusing one account across clients invalidates the other clients' tokens on refresh.
  scope_form: permissions_for:{CONTACT_ID}
  tokenUrl: https://{hostname}/ewws/otoken
  token_expiry_minutes_default: 15
  token_expiry_minutes_range:
  - 1
  - 60
  type: oauth2
- authorizationUrl: https://{hostname}/ewws/oauth
  code_challenge_methods:
  - S256
  - plain
  code_verifier_length:
  - 43
  - 128
  docs: https://help.agiloft.com/space/HELP/43716464/Use%20OAuth2%20to%20Access%20REST%20API
  flow: authorizationCode
  grant_types:
  - authorization_code_pkce
  name: OAuth2AuthorizationCodePKCE
  pkce: true
  recommended_for: public clients
  spec: RFC 7636
  tokenUrl: https://{hostname}/ewws/otoken
  type: oauth2
- docs: https://help.agiloft.com/space/HELP/43716464/Use%20OAuth2%20to%20Access%20REST%20API
  flow: clientCredentials
  grant_types:
  - client_credentials
  name: OAuth2ClientCredentials
  tokenUrl: https://{hostname}/ewws/otoken
  type: oauth2
  use_case: machine-to-machine integration with no user interaction
- bearerFormat: JWT
  default_expiry_minutes: 15
  docs: https://help.agiloft.com/space/HELP/43714204/REST%20-%20Login
  expiry_global_variable: token_expires_in
  max_expiry_minutes: 60
  name: JWTBearer
  note: EWLogin returns an access token plus the authentication scheme to prefix it with; the docs say Bearer is the default. Using the token in an Authorization header is how Agiloft recommends keeping credentials out of REST URLs.
  refresh: POST /ewws/EWLogin?$KB={kb}&$lang={lang}&refresh_token={token}
  response_fields:
  - access_token
  - refresh_token
  - expiration_time_unit
  - expires_in
  - authentication_scheme
  revocation_endpoint: https://{hostname}/ewws/EWLogout
  scheme: bearer
  token_endpoint: https://{hostname}/ewws/EWLogin
  type: http
- also_accepted_in: request body (POST)
  applies_to:
  - EWRead
  - EWSelect
  - EWCreate
  - EWUpdate
  - EWDelete
  docs: https://help.agiloft.com/space/HELP/43714573/API%20Security
  in: query
  name: BasicCredentialParameters
  names:
  - $login
  - $password
  note: The legacy credential-in-parameter style. Agiloft documents passing the pair in a POST body rather than the query string so the credentials are not in the URL. Not recommended for new integrations.
  type: apiKey
- docs: https://help.agiloft.com/space/HELP/703889445
  name: ExtAuth
  note: Agiloft's pre-OAuth authorization mechanism, still supported for backward compatibility with existing integrations. Issues bearer access tokens like OAuth 2.0 but uses different endpoints, configuration and an different authorization model.
  scheme: bearer
  status: legacy
  type: http
- docs: https://help.agiloft.com/space/HELP/778928159/Set%20Up%20SCIM
  name: SCIMBearerToken
  note: Generated per SCIM profile in the KB; multiple tokens per profile are supported so credentials can be rotated without interrupting provisioning. Shown once at generation time.
  scheme: bearer
  surface: https://{hostname}/scim/v2
  type: http
slug: agiloft-authentication
source_filename: agiloft-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-12'\nmethod: searched\nsource: https://help.agiloft.com/space/HELP/43716464/Use%20OAuth2%20to%20Access%20REST%20API\ndocs: https://help.agiloft.com/space/HELP/43714573/API%20Security\nnote: >-\n  Derived from the published documentation rather than from an OpenAPI securitySchemes block:\n  Agiloft's OpenAPI document is generated per knowledgebase and is only reachable from inside an\n  authenticated KB (Setup > System > View REST documentation), so there is no public spec to\n  parse. Every scheme below is stated in Agiloft's own public docs.\nsummary:\n  types: [oauth2, http, apiKey]\n  api_key_in: [query, body]\n  oauth2_flows: [authorizationCode, authorizationCodePKCE, clientCredentials]\n  bearer_formats: [JWT, OAuth2 access token, SCIM bearer token]\nschemes:\n- name: OAuth2AuthorizationCode\n  type: oauth2\n  flow: authorizationCode\n  authorizationUrl: https://{hostname}/ewws/oauth\n  tokenUrl: https://{hostname}/ewws/otoken\n  grant_types: [authorization_code]\n\
  \  scope_form: 'permissions_for:{CONTACT_ID}'\n  token_expiry_minutes_default: 15\n  token_expiry_minutes_range: [1, 60]\n  authorization_code_lifetime: 5 minutes\n  docs: https://help.agiloft.com/space/HELP/43716464/Use%20OAuth2%20to%20Access%20REST%20API\n  note: >-\n    Client registration happens in the KB at Setup > Integration > OAuth2 Client Setup. Each OAuth\n    client is bound to one native Agiloft service-user account and every call made with its tokens\n    runs as that account. Reusing one account across clients invalidates the other clients' tokens\n    on refresh.\n- name: OAuth2AuthorizationCodePKCE\n  type: oauth2\n  flow: authorizationCode\n  pkce: true\n  code_challenge_methods: [S256, plain]\n  code_verifier_length: [43, 128]\n  grant_types: [authorization_code_pkce]\n  authorizationUrl: https://{hostname}/ewws/oauth\n  tokenUrl: https://{hostname}/ewws/otoken\n  recommended_for: public clients\n  spec: RFC 7636\n  docs: https://help.agiloft.com/space/HELP/43716464/Use%20OAuth2%20to%20Access%20REST%20API\n\
  - name: OAuth2ClientCredentials\n  type: oauth2\n  flow: clientCredentials\n  tokenUrl: https://{hostname}/ewws/otoken\n  grant_types: [client_credentials]\n  use_case: machine-to-machine integration with no user interaction\n  docs: https://help.agiloft.com/space/HELP/43716464/Use%20OAuth2%20to%20Access%20REST%20API\n- name: JWTBearer\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  token_endpoint: https://{hostname}/ewws/EWLogin\n  revocation_endpoint: https://{hostname}/ewws/EWLogout\n  refresh: 'POST /ewws/EWLogin?$KB={kb}&$lang={lang}&refresh_token={token}'\n  default_expiry_minutes: 15\n  max_expiry_minutes: 60\n  expiry_global_variable: token_expires_in\n  response_fields: [access_token, refresh_token, expiration_time_unit, expires_in, authentication_scheme]\n  docs: https://help.agiloft.com/space/HELP/43714204/REST%20-%20Login\n  note: >-\n    EWLogin returns an access token plus the authentication scheme to prefix it with; the docs say\n    Bearer is the default. Using\
  \ the token in an Authorization header is how Agiloft recommends\n    keeping credentials out of REST URLs.\n- name: BasicCredentialParameters\n  type: apiKey\n  in: query\n  names: ['$login', '$password']\n  also_accepted_in: request body (POST)\n  applies_to: [EWRead, EWSelect, EWCreate, EWUpdate, EWDelete]\n  docs: https://help.agiloft.com/space/HELP/43714573/API%20Security\n  note: >-\n    The legacy credential-in-parameter style. Agiloft documents passing the pair in a POST body\n    rather than the query string so the credentials are not in the URL. Not recommended for new\n    integrations.\n- name: ExtAuth\n  type: http\n  scheme: bearer\n  status: legacy\n  docs: https://help.agiloft.com/space/HELP/703889445\n  note: >-\n    Agiloft's pre-OAuth authorization mechanism, still supported for backward compatibility with\n    existing integrations. Issues bearer access tokens like OAuth 2.0 but uses different endpoints,\n    configuration and an different authorization model.\n- name:\
  \ SCIMBearerToken\n  type: http\n  scheme: bearer\n  surface: https://{hostname}/scim/v2\n  docs: https://help.agiloft.com/space/HELP/778928159/Set%20Up%20SCIM\n  note: >-\n    Generated per SCIM profile in the KB; multiple tokens per profile are supported so credentials\n    can be rotated without interrupting provisioning. Shown once at generation time.\nsso:\n  saml2: https://help.agiloft.com/space/HELP/43718160\n  oauth2: https://help.agiloft.com/space/HELP/43716464/Use%20OAuth2%20to%20Access%20REST%20API\n  note: SCIM provisioning is supported alongside either SSO method.\nauthorization_controls:\n- control: group permissions\n  note: >-\n    API calls return only data the authenticated user's group permissions allow, at table, record\n    and field level. The API respects the same ownership model as the GUI.\n  docs: https://help.agiloft.com/space/HELP/43714573/API%20Security\n- control: interface allow-list\n  note: >-\n    Groups must be explicitly listed under Setup > System >\
  \ Manage Web Services > Groups allowed\n    for REST (and the SOAP equivalent). A user outside those groups gets 403 even with full record\n    permissions.\n- control: operation scopes\n  note: >-\n    A Scope parameter on the access-token configuration restricts which REST operations a token may\n    call. A blank Scope grants every operation.\n  see: scopes/agiloft-scopes.yml\n- control: IP allow/deny lists\n  global_variables: ['Security: REST IP Blacklist', 'Security: REST IP Whitelist', 'Security: SOAP IP Blacklist', 'Security: SOAP IP Whitelist']\n  docs: https://help.agiloft.com/space/HELP/43714573/API%20Security\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/agiloft/refs/heads/main/authentication/agiloft-authentication.yml
summary_line: oauth2/http/apiKey · 7 schemes
tags:
- Contract Lifecycle Management
- Contract Management
- Legal
- Procurement
- Enterprise Software
- No-Code
- Workflow-Automation
- Document Automation
- Webhook
- SCIM
- Company
---
