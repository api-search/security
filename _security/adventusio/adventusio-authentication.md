---
anonymous_access: false
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: probed
name: Adventusio Authentication
name_suffix: Authentication
oauth_flows: []
overview: Adventus.io declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Adventus.io
provider_slug: adventusio
scheme_count: 2
schemes:
- description: Session bearer token returned by the userLogin (recruiter / institution staff) or studentLogin mutation. Both mutations return an auth payload type (UserAuthPayload / StudentAuthPayload) and there are matching userLogout / studentLogout mutations, so the token is server-revocable.
  evidence: graphql/adventusio.graphql
  header: Authorization
  id: bearer-token
  in: header
  issued_by:
  - arguments:
    - email
    - password
    audience: recruiter, agent and institution staff accounts
    mutation: userLogin
    returns: UserAuthPayload
  - arguments:
    - email
    - password
    audience: student accounts
    mutation: studentLogin
    returns: StudentAuthPayload
  method: derived
  recovery:
  - userForgotPassword / userResetPassword
  - studentForgotPassword / studentResetPassword
  revoked_by:
  - userLogout
  - studentLogout
  scheme: bearer
  type: http
- description: 'A second, distinct credential. The Adventus Connect queries pendingConnectCount(accessToken: String!) and connectInvites(accessToken: String!) take the token as a REQUIRED GraphQL ARGUMENT rather than an Authorization header. This is an invitation-scoped token delivered out of band (ConnectSource enum values are EMAIL and WEB), not the session bearer above.'
  evidence: graphql/adventusio.graphql
  id: connect-access-token
  in: query
  method: derived
  note: Passing a credential as a query argument means it can land in GraphQL query logs, APM traces and error payloads that a header-borne token would not reach. Recorded as observed, not endorsed.
  parameter: accessToken
  type: apiKey
slug: adventusio-authentication
source_filename: adventusio-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-09'\nmethod: probed\nsource: https://api.adventus.io/graphql (anonymous introspection + live unauthenticated probes, 2026-09-09)\nprovider: Adventus.io\napi: adventusio-graphql\nsummary: >-\n  Adventus.io does not publish an authentication guide. Everything below was\n  established by introspecting the live GraphQL endpoint and by observing what\n  the server returns to an unauthenticated caller. There is no OAuth 2.0\n  authorization server, no OpenID Connect discovery document and no API-key\n  provisioning surface reachable without a partner account: the only\n  credential issuers in the contract are two password-login mutations.\nschemes:\n- id: bearer-token\n  type: http\n  scheme: bearer\n  in: header\n  header: Authorization\n  description: >-\n    Session bearer token returned by the userLogin (recruiter / institution\n    staff) or studentLogin mutation. Both mutations return an auth payload type\n    (UserAuthPayload / StudentAuthPayload) and there\
  \ are matching userLogout /\n    studentLogout mutations, so the token is server-revocable.\n  issued_by:\n  - mutation: userLogin\n    arguments: [email, password]\n    returns: UserAuthPayload\n    audience: recruiter, agent and institution staff accounts\n  - mutation: studentLogin\n    arguments: [email, password]\n    returns: StudentAuthPayload\n    audience: student accounts\n  revoked_by: [userLogout, studentLogout]\n  recovery:\n  - userForgotPassword / userResetPassword\n  - studentForgotPassword / studentResetPassword\n  evidence: graphql/adventusio.graphql\n  method: derived\n- id: connect-access-token\n  type: apiKey\n  in: query\n  parameter: accessToken\n  description: >-\n    A second, distinct credential. The Adventus Connect queries\n    pendingConnectCount(accessToken: String!) and\n    connectInvites(accessToken: String!) take the token as a REQUIRED GraphQL\n    ARGUMENT rather than an Authorization header. This is an invitation-scoped\n    token delivered out of band\
  \ (ConnectSource enum values are EMAIL and WEB),\n    not the session bearer above.\n  note: >-\n    Passing a credential as a query argument means it can land in GraphQL query\n    logs, APM traces and error payloads that a header-borne token would not\n    reach. Recorded as observed, not endorsed.\n  evidence: graphql/adventusio.graphql\n  method: derived\nanonymous_surface:\n  description: >-\n    A subset of reference data answers with no credential at all. Confirmed by\n    live unauthenticated POST on 2026-09-09.\n  verified: probed\n  operations:\n  - field: countries\n    http_status: 200\n    result: full country list returned\n  - field: studyLevels\n    http_status: 200\n    result: 11 study levels returned\n  - field: languages\n    http_status: 200\n    result: schema-confirmed; same anonymous class\n  - field: gradingSystems\n    http_status: 200\n    result: schema-confirmed; same anonymous class\n  - field: __schema\n    http_status: 200\n    result: full introspection\
  \ returned (99 types)\ngated_surface:\n  description: >-\n    Every student, order, institution, document, messaging and statistics field\n    is gated. The server answers HTTP 200 with a GraphQL errors[] entry rather\n    than an HTTP 401.\n  verified: probed\n  observed:\n  - field: students\n    http_status: 200\n    graphql_error_code: UNAUTHENTICATED\n    message: '401: Unauthorized'\n  - field: myAgent\n    http_status: 200\n    graphql_error_code: UNAUTHENTICATED\n    message: '401: Unauthorized'\n  - field: institution\n    http_status: 200\n    graphql_error_code: UNAUTHENTICATED\n    message: '401: Unauthorized'\ndiscovery_documents_absent:\n  note: >-\n    Probed 2026-09-09 on adventus.io, www.adventus.io, api.adventus.io,\n    app.adventus.io and blog.adventus.io. See\n    well-known/adventusio-well-known.yml for the full status table.\n  paths:\n  - path: /.well-known/openid-configuration\n    result: no host served a document\n  - path: /.well-known/oauth-authorization-server\n\
  \    result: no host served a document\n  - path: /.well-known/oauth-protected-resource\n    result: no host served a document\noauth_scopes: none\nmtls: false\ntransport:\n  tls_minimum_observed: TLSv1.2\n  hsts_on_api_host: true\n  hsts_max_age: 2592000\n  hsts_include_subdomains: true\n  note: >-\n    HSTS observed directly on the POST /graphql response from api.adventus.io\n    on 2026-09-09 (strict-transport-security max-age=2592000; includeSubdomains).\n    The domain-security probe records hsts null for that host because it reads\n    the 404 root, not the GraphQL path.\n  provider_claim: >-\n    \"All communications are encrypted via industry standard HTTPS/TLS (TLS 1.2\n    or higher)\" -- https://adventus.io/recruiters/security/\ngaps:\n- No published authentication documentation of any kind.\n- No token lifetime, refresh mechanism or expiry semantics stated anywhere in the\n  contract or on the public site.\n- No scope, role or permission model exposed in the schema.\n- Credential\
  \ provisioning requires a partner account; there is no self-serve API key.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/adventusio/refs/heads/main/authentication/adventusio-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Education
- International Education
- Student Recruitment
- Marketplace
- GraphQL
- Higher Education
- EdTech
- Admissions
- Analytics
---
