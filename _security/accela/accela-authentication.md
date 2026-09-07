---
anonymous_access: false
api_key_in: []
api_specs:
- filename: accela-records-openapi.yml
  format: yaml
  label: Accela Construct API (V4)
  slug: accela-construct-api-v4
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/accela/refs/heads/main/openapi/accela-records-openapi.yml
- filename: accela-authentication-openapi.yml
  format: yaml
  label: Accela Authentication API (OAuth 2.0)
  slug: accela-authentication-api-oauth-20
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/accela/refs/heads/main/openapi/accela-authentication-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Accela Authentication
name_suffix: Authentication
oauth_flows: []
overview: Accela declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: Accela
provider_slug: accela
scheme_count: 3
schemes:
- description: An Accela API access token. Applies to every endpoint that reads or writes Civic user data — 371 of 417 published operations.
  flows:
  - authorization_code
  - implicit
  - password
  header: Authorization
  id: access_token
  location: header
  scoped: true
  scopes_ref: scopes/accela-scopes.yml
  type: oauth2
- description: Application ID and secret issued when an app is registered on the Accela Developer Portal (My Apps). Applies to endpoints that read app settings.
  header:
  - x-accela-appid
  - x-accela-appsecret
  id: app_credentials
  location: header
  type: apiKey
- description: Anonymous public access for citizen apps. The app id, agency name and environment identify the tenant instead of a user. Only citizen apps support this type; the surfaced data is whatever the agency has granted the Civic Platform anonymous user. 34 published operations use it.
  header:
  - x-accela-appid
  - x-accela-agency
  - x-accela-environment
  id: anonymous
  location: header
  type: apiKey
slug: accela-authentication
source_filename: accela-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-06'\nmethod: searched\nsource: https://developer.accela.com/docs/construct-apiAuth.html\ndocs:\n  - https://developer.accela.com/docs/construct-apiAuth.html\n  - https://developer.accela.com/docs/construct-authenticationTypes.html\n  - https://developer.accela.com/docs/construct-httpHeaders.html\n  - https://developer.accela.com/docs/construct-permissionScopes.html\n  - https://developer.accela.com/docs/api_reference/api-auth.html\nsummary: >-\n  Accela Construct authenticates on three levels, and which one applies is declared per operation inside the\n  published Swagger documents rather than in a securityDefinitions block. 371 of the 417 published operations\n  require an OAuth 2.0 access token, 34 require no authorization (anonymous citizen access), and 1 requires app\n  credentials. NOTE FOR FUTURE ROUNDS: none of the fifteen Swagger 2.0 documents declares a securityDefinitions\n  object, so derive-authentication.py finds nothing; this profile was read\
  \ from the provider's own auth\n  documentation and from the per-operation \"**Authorization Type**\" line each operation carries in its\n  description.\nauthorization_server: https://auth.accela.com\nendpoints:\n  - name: Get Authorization Code\n    method: POST\n    url: https://auth.accela.com/oauth2/authorize\n    operationId: oauth2.authorize\n  - name: Get Access Token\n    method: POST\n    url: https://auth.accela.com/oauth2/token\n    operationId: oauth2.token\n    note: Requires Content-Type application/x-www-form-urlencoded and an x-accela-appid header.\n  - name: Get Token Info\n    method: GET\n    url: https://auth.accela.com/oauth2/tokeninfo\n    operationId: oauth2.tokeninfo\n    note: Validates an access token supplied in the Authorization header.\ndiscovery:\n  rfc8414_metadata: false\n  openid_configuration: false\n  note: >-\n    auth.accela.com publishes neither /.well-known/oauth-authorization-server nor\n    /.well-known/openid-configuration (both 404, empty body,\
  \ probed 2026-09-06). A client cannot discover\n    these endpoints programmatically; they are only documented in prose.\nschemes:\n  - id: access_token\n    type: oauth2\n    location: header\n    header: Authorization\n    description: >-\n      An Accela API access token. Applies to every endpoint that reads or writes Civic user data — 371 of 417\n      published operations.\n    flows:\n      - authorization_code\n      - implicit\n      - password\n    scoped: true\n    scopes_ref: scopes/accela-scopes.yml\n  - id: app_credentials\n    type: apiKey\n    location: header\n    header:\n      - x-accela-appid\n      - x-accela-appsecret\n    description: >-\n      Application ID and secret issued when an app is registered on the Accela Developer Portal (My Apps).\n      Applies to endpoints that read app settings.\n  - id: anonymous\n    type: apiKey\n    location: header\n    header:\n      - x-accela-appid\n      - x-accela-agency\n      - x-accela-environment\n    description: >-\n\
  \      Anonymous public access for citizen apps. The app id, agency name and environment identify the tenant\n      instead of a user. Only citizen apps support this type; the surfaced data is whatever the agency has\n      granted the Civic Platform anonymous user. 34 published operations use it.\ntenancy:\n  required_headers:\n    - name: x-accela-agency\n      description: The government agency (tenant) the request is executed against.\n    - name: x-accela-environment\n      description: The agency environment (for example a production or test instance) the request targets.\n    - name: x-accela-agencies\n      description: >-\n        \"all\" or a comma-delimited agency list, for cross-agency GET reads across the accounts linked to a\n        logged-in CivicID. Overrides x-accela-agency when both are sent.\n  note: >-\n    Agency and environment are also embedded inside the access token. When both a token and the headers are\n    sent, the values must match or the request is rejected.\
  \ This is the defining shape of the API: there is no\n    single Accela tenant, and every call is executed inside one named government agency.\napp_types:\n  types:\n    - id: agency\n      description: An app acting for agency staff. 151 operations are Agency-only.\n    - id: citizen\n      description: An app acting for a member of the public. 20 operations are Citizen-only.\n    - id: all\n      description: Available to both agency and citizen apps. 240 operations.\n  note: The client id/secret pair issued at registration determines whether a token is an agency or a citizen token.\nregistration:\n  url: https://developer.accela.com/Register/Register\n  app_registration: https://developer.accela.com/ApplicationList/Index\n  note: >-\n    Since the 4.6.5.4 release (August 2026) developer-portal registration is an approval request: the account\n    is created disabled and a human enables it in the admin portal before credentials work.\n  agency_credentials: >-\n    Agency and environment\
  \ names are not self-serve. Accela-hosted agencies get them from Accela Customer\n    Support; on-premise agencies from their own Construct administrator.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/accela/refs/heads/main/authentication/accela-authentication.yml
summary_line: 3 schemes
tags:
- GovTech
- Government
- Permitting
- Licensing
- Code Enforcement
- Inspections
- Asset Management
- Citizen Engagement
- Land Management
- Civic Platform
- Public Sector
- SaaS
---
