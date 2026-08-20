---
api_key_in:
- header
auth_types:
- oauth2
- apiKey
description: ''
kind: authentication
layout: security
method: searched
name: Uship Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- implicit
- password
- clientCredentials
overview: uShip secures its APIs with oauth2 and apiKey across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, implicit, password, and clientCredentials flow(s).
provider_name: uShip
provider_slug: uship
scheme_count: 2
schemes:
- description: 'uShip APIs use OAuth 2.0 (RFC 6749) for authentication and authorization. All four grant types are supported; the grant granted to an integration depends on its use case. Access tokens are presented on every subsequent call as `Authorization: Bearer {access_token}` (the "Bearer" label is case sensitive).'
  flows:
  - description: For applications that access endpoints as an anonymous user (for example searching listings). POST content-type application/x-www-form-urlencoded with grant_type=client_credentials&client_id=...&client_secret=...
    documented_expires_in: 2592000
    flow: clientCredentials
    response_fields:
    - token_type
    - mapi
    - access_token
    - expires_in
    - refresh_token
    tokenUrl: https://api.uship.com/oauth/token
    tokenUrl_sandbox: https://apistaging.uship.com/oauth/token
  - description: For web-based scenarios where the source code runs on a private server. Documented as the most secure grant type and the recommended default for server-side integrations.
    flow: authorizationCode
    tokenUrl: https://api.uship.com/oauth/token
  - description: For single-page JavaScript and browser/mobile applications that require less security; uShip recommends the authorization code grant instead where a more secure method is available.
    flow: implicit
  - description: Resource Owner Password Credentials — for authorizing an app that needs access to a uShip user account where the user supplies their own credentials.
    flow: password
  name: OAuth2
  scopes: []
  scopes_note: uShip does not publish a named OAuth scope vocabulary. Access is granted per integration — "we grant access to the resources that make the most sense for your integration needs" — so authorization is resource-grant based rather than scope-string based. No scopes/ artifact is emitted.
  type: oauth2
- description: A self-service API key is available for the LTL products; keys are created and rotated in the developer portal at https://developer.uship.com/apps/mykeys. The archived first-party Node.js wrapper initializes with an API key, API secret, uShip username, and password.
  docs: https://developer.uship.com/about-our-apis/self-service-api-key--ltl-
  in: header
  name: APIKey
  type: apiKey
slug: uship-authentication
source_filename: uship-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-02'\nmethod: searched\nsource: >-\n  uShip developer portal authentication documentation — https://developer.uship.com/docs/Authentication_OAuth2,\n  /docs/Client_Credentials, /docs/Authorization_Code, /docs/Resource_Owner_Password_Credentials, and\n  /docs/read/Authorization_Code (referenced from https://www.uship.com/llms.txt)\ndocs: https://developer.uship.com/docs/read/Authorization_Code\naccess: >-\n  Partner-gated. The uShip developer portal is invitation-only (\"You must have been invited to get access\")\n  and OAuth 2.0 credentials are issued by the uShip API team after a uShip Account Manager or General\n  Manager approves API access. An API key can be self-served for the LTL products\n  (https://developer.uship.com/about-our-apis/self-service-api-key--ltl-); keys are managed at\n  https://developer.uship.com/apps/mykeys.\nsummary:\n  types: [oauth2, apiKey]\n  api_key_in: [header]\n  oauth2_flows: [authorizationCode, implicit, password, clientCredentials]\n\
  \  token_type: bearer\n  token_generator: Mashery\nschemes:\n- name: OAuth2\n  type: oauth2\n  description: >-\n    uShip APIs use OAuth 2.0 (RFC 6749) for authentication and authorization. All four grant types are\n    supported; the grant granted to an integration depends on its use case. Access tokens are presented on\n    every subsequent call as `Authorization: Bearer {access_token}` (the \"Bearer\" label is case sensitive).\n  flows:\n  - flow: clientCredentials\n    tokenUrl: https://api.uship.com/oauth/token\n    tokenUrl_sandbox: https://apistaging.uship.com/oauth/token\n    description: >-\n      For applications that access endpoints as an anonymous user (for example searching listings).\n      POST content-type application/x-www-form-urlencoded with\n      grant_type=client_credentials&client_id=...&client_secret=...\n    response_fields: [token_type, mapi, access_token, expires_in, refresh_token]\n    documented_expires_in: 2592000\n  - flow: authorizationCode\n    tokenUrl:\
  \ https://api.uship.com/oauth/token\n    description: >-\n      For web-based scenarios where the source code runs on a private server. Documented as the most secure\n      grant type and the recommended default for server-side integrations.\n  - flow: implicit\n    description: >-\n      For single-page JavaScript and browser/mobile applications that require less security; uShip\n      recommends the authorization code grant instead where a more secure method is available.\n  - flow: password\n    description: >-\n      Resource Owner Password Credentials — for authorizing an app that needs access to a uShip user\n      account where the user supplies their own credentials.\n  scopes: []\n  scopes_note: >-\n    uShip does not publish a named OAuth scope vocabulary. Access is granted per integration — \"we grant\n    access to the resources that make the most sense for your integration needs\" — so authorization is\n    resource-grant based rather than scope-string based. No scopes/ artifact\
  \ is emitted.\n- name: APIKey\n  type: apiKey\n  in: header\n  description: >-\n    A self-service API key is available for the LTL products; keys are created and rotated in the developer\n    portal at https://developer.uship.com/apps/mykeys. The archived first-party Node.js wrapper initializes\n    with an API key, API secret, uShip username, and password.\n  docs: https://developer.uship.com/about-our-apis/self-service-api-key--ltl-\nrequired_headers:\n- header: Authorization\n  value: Bearer {access_token}\n  description: Required for every call after initial authorization. Case-sensitive \"Bearer\" label plus a space.\n- header: Accept\n  value: application/json\n  description: Acceptable content types for the response.\n- header: Content-Type\n  value: application/json\n  description: Defines the request body MIME type for POST and PUT requests.\n- header: Content-Type\n  value: application/x-www-form-urlencoded\n  description: Required for POSTs to obtain codes or tokens from the\
  \ authorization/resource server.\nsupport: api-support@uship.com\npartner_contact: partners@uship.com\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/uship/refs/heads/main/authentication/uship-authentication.yml
summary_line: oauth2/apiKey · 2 schemes
tags:
- Shipping
- Logistics
- Freight
- Marketplace
- Transportation
- auto-transport
- ltl-freight
- Last Mile Delivery
- Shipment Tracking
- E-Commerce
- Supply Chain
- rate-quotes
---
