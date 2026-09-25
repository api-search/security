---
anonymous_access: false
api_key_in: []
auth_types:
- oauth2
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: East West Bancorp Authentication
name_suffix: Authentication
oauth_flows:
- clientCredentials
overview: East West Bancorp secures its APIs with oauth2 across 1 declared security scheme, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the clientCredentials flow(s).
provider_name: East West Bancorp
provider_slug: east-west-bancorp
scheme_count: 1
schemes:
- credentials:
    application_model: An "application" is a collection of one or more API resources reachable with a single authentication credential. A developer must create one before calling the sandbox.
    client_id: issued per application created in the developer portal
    client_secret: issued per application created in the developer portal
    encoding: Base-64 encode ClientID and ClientSecret; the FAQ recommends encoding in application logic rather than storing a static encoded string, and requires the "Basic" prefix on the token call.
  flows:
  - expires_in_seconds: 86400
    flow: clientCredentials
    grant_type: client_credentials
    note: Identity provider is Okta. The Authorization API page shows the token call with client_id and client_secret in the form body; the portal FAQ additionally documents base-64 encoding the ClientID and ClientSecret and prefixing "Basic " on the token call, so both credential presentations appear in the provider's own documentation.
    parameters:
    - client_id
    - client_secret
    - grant_type
    request_content_type: application/x-www-form-urlencoded
    response_fields:
    - access_token
    - token_type
    - expires_in
    token_type: Bearer
    token_url: https://ewbpoc.okta.com/oauth2/ausdaetdg9zY8EZuI2p6/v1/token
    token_url_status: 'Published verbatim by the provider. Probed 2026-09-14: the Okta authorization-server metadata for this server id returns 404 (Okta "Page Not Found"), and the org slug "ewbpoc" reads as a proof-of-concept tenant, so the documented endpoint may be stale. Recorded as the provider states it; not corrected, not guessed.'
  name: OAuth2 client credentials (Authorization API)
  request_authorization:
    applies_to: every protected API endpoint
    format: Bearer <access_token>
    header: Authorization
  scheme: OAuth 2.0 Authorization Framework, two-legged / machine-to-machine
  sources:
  - https://apiportal.eastwestbank.com/AuthorizationAPI
  - https://apiportal.eastwestbank.com/faqs
  transport_security:
    client_certificate_required: true
    scope: A client certificate is required for connectivity to the sandbox and production environments; no certificate is needed to browse the Bridge Open Banking portal. Certificates and access credentials are issued by East West Bank GTS during onboarding.
    source: https://apiportal.eastwestbank.com/faqs
  type: oauth2
slug: east-west-bancorp-authentication
source_filename: east-west-bancorp-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-14'\nmethod: searched\nsource: https://apiportal.eastwestbank.com/AuthorizationAPI\ndocs: https://apiportal.eastwestbank.com/AuthorizationAPI\nnote: >-\n  East West Bancorp publishes no API of its own; the group's API surface is the Bridge Open\n  Banking program operated by its banking subsidiary, East West Bank, at\n  apiportal.eastwestbank.com. No OpenAPI or Swagger document is publicly downloadable — the\n  API list, product library and reference render only after portal sign-in — so this profile\n  is transcribed from the two pages the provider serves anonymously: the Authorization API\n  page (which carries the full token exchange, including the literal token endpoint) and the\n  portal FAQ. Nothing here is derived from a securityScheme, because there is no public spec.\nsummary:\n  types:\n  - oauth2\n  oauth2_flows:\n  - clientCredentials\n  api_key_in: []\n  bearer: true\nschemes:\n- name: OAuth2 client credentials (Authorization API)\n  type: oauth2\n\
  \  scheme: OAuth 2.0 Authorization Framework, two-legged / machine-to-machine\n  sources:\n  - https://apiportal.eastwestbank.com/AuthorizationAPI\n  - https://apiportal.eastwestbank.com/faqs\n  flows:\n  - flow: clientCredentials\n    token_url: https://ewbpoc.okta.com/oauth2/ausdaetdg9zY8EZuI2p6/v1/token\n    token_url_status: >-\n      Published verbatim by the provider. Probed 2026-09-14: the Okta authorization-server\n      metadata for this server id returns 404 (Okta \"Page Not Found\"), and the org slug\n      \"ewbpoc\" reads as a proof-of-concept tenant, so the documented endpoint may be stale.\n      Recorded as the provider states it; not corrected, not guessed.\n    grant_type: client_credentials\n    request_content_type: application/x-www-form-urlencoded\n    parameters:\n    - client_id\n    - client_secret\n    - grant_type\n    response_fields:\n    - access_token\n    - token_type\n    - expires_in\n    token_type: Bearer\n    expires_in_seconds: 86400\n    note: >-\n\
  \      Identity provider is Okta. The Authorization API page shows the token call with\n      client_id and client_secret in the form body; the portal FAQ additionally documents\n      base-64 encoding the ClientID and ClientSecret and prefixing \"Basic \" on the token\n      call, so both credential presentations appear in the provider's own documentation.\n  credentials:\n    client_id: issued per application created in the developer portal\n    client_secret: issued per application created in the developer portal\n    encoding: >-\n      Base-64 encode ClientID and ClientSecret; the FAQ recommends encoding in application\n      logic rather than storing a static encoded string, and requires the \"Basic\" prefix on\n      the token call.\n    application_model: >-\n      An \"application\" is a collection of one or more API resources reachable with a single\n      authentication credential. A developer must create one before calling the sandbox.\n  request_authorization:\n    header:\
  \ Authorization\n    format: 'Bearer <access_token>'\n    applies_to: every protected API endpoint\n  transport_security:\n    client_certificate_required: true\n    scope: >-\n      A client certificate is required for connectivity to the sandbox and production\n      environments; no certificate is needed to browse the Bridge Open Banking portal.\n      Certificates and access credentials are issued by East West Bank GTS during onboarding.\n    source: https://apiportal.eastwestbank.com/faqs\ntroubleshooting:\n- status: 401\n  title: Unauthorized\n  causes:\n  - client-id and secret not correctly matched against the application that was created\n  - base-64 encoding not formatted per the authorization documentation\n  - '\"Basic\" not prefixed to the encoded ClientID and ClientSecret on the token call'\n  - access token invalidated or expired\n  source: https://apiportal.eastwestbank.com/faqs\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/east-west-bancorp/refs/heads/main/authentication/east-west-bancorp-authentication.yml
summary_line: oauth2 · 1 scheme
tags:
- Banking
- Financial Services
- Commercial Banking
- Treasury Management
- Open Banking
- Payments
- Cross-Border
- United States
---
