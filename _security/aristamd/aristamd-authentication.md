---
api_key_in: []
api_specs:
- filename: aristamd-comments-api-openapi.yml
  format: yaml
  label: AristaMD Comments API
  slug: aristamd-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aristamd/refs/heads/main/openapi/aristamd-comments-api-openapi.yml
- filename: aristamd-diagnostic-api-openapi.yml
  format: yaml
  label: AristaMD Diagnostic API
  slug: aristamd-diagnostic-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aristamd/refs/heads/main/openapi/aristamd-diagnostic-api-openapi.yml
- filename: aristamd-econsults-api-openapi.yml
  format: yaml
  label: AristaMD E Consults API
  slug: aristamd-econsults-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aristamd/refs/heads/main/openapi/aristamd-econsults-api-openapi.yml
- filename: aristamd-intergy-patients-api-openapi.yml
  format: yaml
  label: AristaMD Intergy/Patients API
  slug: aristamd-intergy-patients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aristamd/refs/heads/main/openapi/aristamd-intergy-patients-api-openapi.yml
- filename: aristamd-panelists-api-openapi.yml
  format: yaml
  label: AristaMD Panelists API
  slug: aristamd-panelists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aristamd/refs/heads/main/openapi/aristamd-panelists-api-openapi.yml
- filename: aristamd-patients-api-openapi.yml
  format: yaml
  label: AristaMD Patients API
  slug: aristamd-patients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aristamd/refs/heads/main/openapi/aristamd-patients-api-openapi.yml
- filename: aristamd-requests-api-openapi.yml
  format: yaml
  label: AristaMD Requests API
  slug: aristamd-requests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aristamd/refs/heads/main/openapi/aristamd-requests-api-openapi.yml
- filename: aristamd-reviews-api-openapi.yml
  format: yaml
  label: AristaMD Reviews API
  slug: aristamd-reviews-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aristamd/refs/heads/main/openapi/aristamd-reviews-api-openapi.yml
- filename: aristamd-specialties-api-openapi.yml
  format: yaml
  label: AristaMD Specialties API
  slug: aristamd-specialties-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aristamd/refs/heads/main/openapi/aristamd-specialties-api-openapi.yml
- filename: aristamd-specialty-api-openapi.yml
  format: yaml
  label: AristaMD Specialty API
  slug: aristamd-specialty-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aristamd/refs/heads/main/openapi/aristamd-specialty-api-openapi.yml
- filename: aristamd-users-api-openapi.yml
  format: yaml
  label: AristaMD Users API
  slug: aristamd-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aristamd/refs/heads/main/openapi/aristamd-users-api-openapi.yml
- filename: aristamd-workup-checklists-api-openapi.yml
  format: yaml
  label: AristaMD Workup Checklists API
  slug: aristamd-workup-checklists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aristamd/refs/heads/main/openapi/aristamd-workup-checklists-api-openapi.yml
auth_types:
- oauth2
- saml2
description: ''
kind: authentication
layout: security
method: probed
name: Aristamd Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
- clientCredentials
- password
- refreshToken
overview: AristaMD secures its APIs with oauth2 and saml2 across 2 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode, clientCredentials, password, and refreshToken flow(s).
provider_name: AristaMD
provider_slug: aristamd
scheme_count: 2
schemes:
- authorization_url: https://api.aristamd.com/oauth/authorize
  discovery:
    note: No RFC 8414 / RFC 9728 / OIDC discovery document is published. The endpoints below were found by direct probe, not by discovery.
    oauth_authorization_server: 404
    oauth_protected_resource: 404
    openid_configuration: 404
  grant_types_supported:
  - evidence: POST /oauth/token grant_type=authorization_code -> 400 invalid_request
    grant: authorization_code
    supported: true
  - evidence: POST /oauth/token grant_type=client_credentials -> 400 invalid_request
    grant: client_credentials
    supported: true
  - evidence: POST /oauth/token grant_type=password -> 400 invalid_request
    grant: password
    supported: true
  - evidence: POST /oauth/token grant_type=refresh_token -> 400 invalid_request
    grant: refresh_token
    supported: true
  - evidence: POST /oauth/token grant_type=implicit -> 400 unsupported_grant_type
    grant: implicit
    supported: false
  - evidence: POST /oauth/token grant_type=urn:ietf:params:oauth:grant-type:jwt-bearer -> 400 unsupported_grant_type
    grant: urn:ietf:params:oauth:grant-type:jwt-bearer
    supported: false
  method: probed
  name: oauth2
  scopes:
    note: No scope reference is published and the Swagger document carries no scope map, so no scopes/ artifact is emitted. Whether this deployment uses Passport scopes at all cannot be determined anonymously.
    published: false
  server: Laravel Passport (league/oauth2-server) — inferred from the RFC 6749 error envelope, which carries the league/oauth2-server `hint` and `message` fields alongside the standard `error`/`error_description` pair.
  token_url: https://api.aristamd.com/oauth/token
  type: oauth2
- assertion_consumer_service:
    binding: urn:oasis:names:tc:SAML:2.0:bindings:HTTP-POST
    index: 1
    location: https://api.aristamd.com/saml2/acs
  authn_requests_signed: false
  entity_id: https://api.aristamd.com/saml2/metadata
  evidence: GET /saml2/metadata -> 200 text/xml, 1622 bytes, valid SAML 2.0 EntityDescriptor
  metadata_file: aristamd-saml2-metadata.xml
  metadata_url: https://api.aristamd.com/saml2/metadata
  method: probed
  name: saml2
  name_id_format: urn:oasis:names:tc:SAML:2.0:nameid-format:persistent
  note: A real, machine-readable federation artifact — this is how an identity provider at a health plan or health system would federate clinicians into AristaMD. Worth flagging that the SP advertises AuthnRequestsSigned="false" and WantAssertionsSigned="false"; for a HIPAA-regulated workload most identity teams would expect signed assertions to be required.
  role: service-provider
  single_logout_service:
    binding: urn:oasis:names:tc:SAML:2.0:bindings:HTTP-Redirect
    location: https://api.aristamd.com/saml2/sls
  technical_contact: support@aristamd.com
  type: saml2
  want_assertions_signed: false
slug: aristamd-authentication
source_filename: aristamd-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-06'\nmethod: probed\nsource: >-\n  Anonymous live probes of https://api.aristamd.com — the published Swagger 2.0\n  definition at /api-docs declares NO securityDefinitions and NO security\n  requirements, so nothing here is derived from the spec. Every fact below is an\n  observed HTTP response recorded on 2026-08-06.\n\nsummary:\n  types: [oauth2, saml2]\n  api_key_in: []\n  oauth2_flows: [authorizationCode, clientCredentials, password, refreshToken]\n  spec_declares_auth: false\n  note: >-\n    This is a documentation gap, not an absence of authentication. The Swagger\n    document ships zero securityDefinitions, so a machine reading only the spec\n    would conclude the API is open. It is not: all 32 documented paths return\n    401 without credentials. The real auth model had to be recovered by probing.\n\n# ---------------------------------------------------------------------------\n# What the spec says\n# ---------------------------------------------------------------------------\n\
  spec:\n  file: openapi/aristamd-openapi-original.json\n  swagger: '2.0'\n  securityDefinitions: null\n  security: null\n  header_parameters_declared: 0\n  gap: >-\n    No securityDefinitions object, no global `security`, and not one operation\n    declares an Authorization header parameter. Adding a single\n    securityDefinitions entry plus a global security requirement would make the\n    contract self-describing for SDK generators and agents.\n\n# ---------------------------------------------------------------------------\n# What the running service actually does\n# ---------------------------------------------------------------------------\nschemes:\n- name: oauth2\n  type: oauth2\n  method: probed\n  server: Laravel Passport (league/oauth2-server) — inferred from the RFC 6749\n    error envelope, which carries the league/oauth2-server `hint` and `message`\n    fields alongside the standard `error`/`error_description` pair.\n  token_url: https://api.aristamd.com/oauth/token\n  authorization_url:\
  \ https://api.aristamd.com/oauth/authorize\n  discovery:\n    oauth_authorization_server: 404\n    oauth_protected_resource: 404\n    openid_configuration: 404\n    note: >-\n      No RFC 8414 / RFC 9728 / OIDC discovery document is published. The\n      endpoints below were found by direct probe, not by discovery.\n  grant_types_supported:\n  # Determined by POSTing each grant_type with no other parameters and reading\n  # which RFC 6749 error came back. `invalid_request` means the server knows the\n  # grant and is asking for the missing parameters; `unsupported_grant_type`\n  # means it does not implement it. No credentials were used or guessed.\n  - grant: authorization_code\n    supported: true\n    evidence: 'POST /oauth/token grant_type=authorization_code -> 400 invalid_request'\n  - grant: client_credentials\n    supported: true\n    evidence: 'POST /oauth/token grant_type=client_credentials -> 400 invalid_request'\n  - grant: password\n    supported: true\n    evidence: 'POST\
  \ /oauth/token grant_type=password -> 400 invalid_request'\n  - grant: refresh_token\n    supported: true\n    evidence: 'POST /oauth/token grant_type=refresh_token -> 400 invalid_request'\n  - grant: implicit\n    supported: false\n    evidence: 'POST /oauth/token grant_type=implicit -> 400 unsupported_grant_type'\n  - grant: urn:ietf:params:oauth:grant-type:jwt-bearer\n    supported: false\n    evidence: 'POST /oauth/token grant_type=urn:ietf:params:oauth:grant-type:jwt-bearer\n      -> 400 unsupported_grant_type'\n  scopes:\n    published: false\n    note: >-\n      No scope reference is published and the Swagger document carries no scope\n      map, so no scopes/ artifact is emitted. Whether this deployment uses\n      Passport scopes at all cannot be determined anonymously.\n\n- name: saml2\n  type: saml2\n  method: probed\n  role: service-provider\n  metadata_url: https://api.aristamd.com/saml2/metadata\n  metadata_file: aristamd-saml2-metadata.xml\n  entity_id: https://api.aristamd.com/saml2/metadata\n\
  \  assertion_consumer_service:\n    binding: urn:oasis:names:tc:SAML:2.0:bindings:HTTP-POST\n    location: https://api.aristamd.com/saml2/acs\n    index: 1\n  single_logout_service:\n    binding: urn:oasis:names:tc:SAML:2.0:bindings:HTTP-Redirect\n    location: https://api.aristamd.com/saml2/sls\n  name_id_format: urn:oasis:names:tc:SAML:2.0:nameid-format:persistent\n  authn_requests_signed: false\n  want_assertions_signed: false\n  technical_contact: support@aristamd.com\n  evidence: 'GET /saml2/metadata -> 200 text/xml, 1622 bytes, valid SAML 2.0\n    EntityDescriptor'\n  note: >-\n    A real, machine-readable federation artifact — this is how an identity\n    provider at a health plan or health system would federate clinicians into\n    AristaMD. Worth flagging that the SP advertises AuthnRequestsSigned=\"false\"\n    and WantAssertionsSigned=\"false\"; for a HIPAA-regulated workload most\n    identity teams would expect signed assertions to be required.\n\n# ---------------------------------------------------------------------------\n\
  # Observed enforcement\n# ---------------------------------------------------------------------------\nenforcement:\n  unauthenticated_response:\n    status: 401\n    body: '{\"message\":\"Unauthorized\"}'\n    content_type: application/json\n  paths_probed_anonymously: [/econsults, /users, /panelists, /reviews, /comments,\n    /workup-checklists/specialties, '/specialties/withAvailablePanelists/{filter}']\n  result: >-\n    All returned 401. Undocumented control paths (/NOT-A-REAL-PATH, /foo/bar)\n    returned 404 with a different body, which confirms the 401s are real\n    authentication rejections on routed endpoints and not a catch-all.\n  anomaly:\n    path: /patients\n    status: 500\n    body: '{\"message\":\"An error has occurred while processing your request\"}'\n    note: >-\n      GET /patients returns 500 rather than 401 when called anonymously. The\n      handler appears to dereference the authenticated user before the auth\n      middleware rejects the request. No data was\
  \ returned; recorded as an\n      observation for the provider, not as an access finding.\n\ndocs:\n  published: false\n  note: >-\n    No public authentication documentation was found. www.aristamd.com has no\n    developer or API section (/developers, /api both 404), and app.aristamd.com,\n    developer.aristamd.com and help.aristamd.com are all the same Angular\n    single-page app, which answers 200 with an identical 1820-byte shell for\n    every path including control paths.\n\nx-evidence:\n  fetched: '2026-08-06'\n  probes:\n  - {url: 'https://api.aristamd.com/api-docs', status: 200}\n  - {url: 'https://api.aristamd.com/oauth/token', status: 400}\n  - {url: 'https://api.aristamd.com/oauth/authorize', status: 401}\n  - {url: 'https://api.aristamd.com/saml2/metadata', status: 200}\n  - {url: 'https://api.aristamd.com/econsults', status: 401}\n  - {url: 'https://api.aristamd.com/.well-known/oauth-authorization-server', status: 404}\n  - {url: 'https://api.aristamd.com/.well-known/openid-configuration',\
  \ status: 404}\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aristamd/refs/heads/main/authentication/aristamd-authentication.yml
summary_line: oauth2/saml2 · 2 schemes
tags:
- Company
- Healthcare
- Digital Health
- Telehealth
- eConsult
- Specialty Care
- Referrals
- Care Coordination
- Health Plans
- Medicaid
- HL7
- Electronic Health Records
---
