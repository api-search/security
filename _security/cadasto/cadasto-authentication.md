---
api_key_in: []
api_specs:
- filename: cadasto-ehr-api-openapi.json
  format: json
  label: Cadasto EHR API
  slug: cadasto-ehr-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cadasto/refs/heads/main/openapi/cadasto-ehr-api-openapi.json
- filename: cadasto-query-api-openapi.json
  format: json
  label: Cadasto Query API (AQL)
  slug: cadasto-query-api-aql
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cadasto/refs/heads/main/openapi/cadasto-query-api-openapi.json
- filename: cadasto-definition-api-openapi.json
  format: json
  label: Cadasto Definition API
  slug: cadasto-definition-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cadasto/refs/heads/main/openapi/cadasto-definition-api-openapi.json
- filename: cadasto-demographic-api-openapi.json
  format: json
  label: Cadasto Demographic API
  slug: cadasto-demographic-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cadasto/refs/heads/main/openapi/cadasto-demographic-api-openapi.json
- filename: cadasto-admin-api-openapi.json
  format: json
  label: Cadasto Admin API
  slug: cadasto-admin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cadasto/refs/heads/main/openapi/cadasto-admin-api-openapi.json
- filename: cadasto-system-api-openapi.json
  format: json
  label: Cadasto System API
  slug: cadasto-system-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cadasto/refs/heads/main/openapi/cadasto-system-api-openapi.json
- filename: cadasto-extra-api-openapi.json
  format: json
  label: Cadasto Additional API
  slug: cadasto-additional-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cadasto/refs/heads/main/openapi/cadasto-extra-api-openapi.json
- filename: cadasto-smart-on-openehr-openapi.json
  format: json
  label: Cadasto SMART on openEHR
  slug: cadasto-smart-on-openehr
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cadasto/refs/heads/main/openapi/cadasto-smart-on-openehr-openapi.json
auth_types:
- oauth2
- http
description: ''
kind: authentication
layout: security
method: searched
name: Cadasto Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cadasto secures its APIs with oauth2 and http across 3 declared security schemes, as derived from its OpenAPI definitions.
provider_name: Cadasto
provider_slug: cadasto
scheme_count: 3
schemes:
- authorization_endpoint: https://{mycompany}.auth.prod.cadasto.io/oauth/authorize
  client_authentication: HTTP Basic (preferred) or client_id/client_secret in the form body (documented as less preferred)
  errors:
    codes:
      invalid_client: Wrong client_id or client_secret
      invalid_grant: Incorrect grant_type
      invalid_request: Invalid client credentials or refresh token
      invalid_scope: Requested scope not allowed for this client
    format: RFC 6749 section 5.2 ({"error", "error_description"})
  flow: clientCredentials
  name: oauth2_client_credentials
  optional_parameters:
    scope: space-separated, e.g. "api.read api.write"
  refresh_strategy: No refresh_token is issued. The docs instruct clients to read expires_in and request a new token before expiry with a safety margin.
  refresh_token: false
  required_parameters:
    audience: https://{mycompany}.api.prod.cadasto.io/openehr/v1
    grant_type: client_credentials
  sources:
  - https://docs.cadasto.io/docs/guides/authentication
  token_endpoint: https://{mycompany}.auth.prod.cadasto.io/oauth/token
  token_lifetime_seconds: 3600
  token_type: Bearer
  type: oauth2
  usage: Authorization:...Bearer <access_token> on every API request
- applies_to: Cadasto Additional API (the only published document that declares a securityScheme)
  bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/cadasto-extra-api-openapi.json
  type: http
- applies_to: Third-party app launch against a Cadasto tenant
  detail: Cadasto declares SMART-on-openEHR 1.1.0 "Fully supported" in its published conformance statement, and publishes a pointer OpenAPI document at https://docs.cadasto.io/smart-on-openehr rather than restating the specification. Redirect URIs and CORS origins are registered at credential-issuance time (docs FAQ).
  flow: authorizationCode
  name: smart_on_openehr
  pkce: required for interactive flows
  sources:
  - https://docs.cadasto.io/smart-on-openehr
  - https://www.cadasto.com/wp-content/uploads/2026/06/Cadasto-CDR-openEHR-conformance-statement-June-2026.pdf
  type: oauth2
slug: cadasto-authentication
source_filename: cadasto-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-02'\nmethod: searched\nsource: >-\n  https://docs.cadasto.io/docs/guides/authentication (OAuth 2.0 Client Credentials guide),\n  https://docs.cadasto.io/docs/faq (credential issuance and environment isolation),\n  https://docs.cadasto.io/docs/quick-start (Authorization header usage), and the\n  securitySchemes block of openapi/cadasto-extra-api-openapi.json.\n  Upgraded from the derived profile: the six openEHR ITS-REST documents Cadasto publishes carry\n  an EMPTY components.securitySchemes and `security: []`, because they are the standard's own\n  documents. The real auth contract is documented in prose, not in those specs.\ndocs: https://docs.cadasto.io/docs/guides/authentication\n\nsummary:\n  primary: OAuth 2.0 Client Credentials (RFC 6749 section 4.4), Bearer token (RFC 6750)\n  interactive: SMART on openEHR / authorization code with PKCE (redirect URIs issued on request)\n  types: [oauth2, http]\n  self_service: false\n  note: >-\n    Credentials\
  \ are not self-service. client_id and client_secret are issued by Cadasto after a\n    tenant environment is provisioned, per environment (development, acceptation, production),\n    on request via the template published in the docs FAQ.\n\nservice_discovery:\n  document: /.well-known/smart-configuration\n  host: https://{mycompany}.auth.prod.cadasto.io\n  method: documented\n  probed: false\n  probe_note: >-\n    NOT PROBED — the auth host is per-tenant and templated; there is no anonymous host to\n    resolve. Recorded from the docs, which show the response shape verbatim.\n  advertises:\n    - authorization_endpoint\n    - token_endpoint\n    - grant_types_supported\n    - scopes_supported\n    - (may include API service URLs, e.g. org.openehr.rest, client auth methods, SMART capabilities)\n\nschemes:\n- name: oauth2_client_credentials\n  type: oauth2\n  flow: clientCredentials\n  token_endpoint: https://{mycompany}.auth.prod.cadasto.io/oauth/token\n  authorization_endpoint: https://{mycompany}.auth.prod.cadasto.io/oauth/authorize\n\
  \  client_authentication: HTTP Basic (preferred) or client_id/client_secret in the form body (documented as less preferred)\n  required_parameters:\n    grant_type: client_credentials\n    audience: https://{mycompany}.api.prod.cadasto.io/openehr/v1\n  optional_parameters:\n    scope: space-separated, e.g. \"api.read api.write\"\n  token_type: Bearer\n  token_lifetime_seconds: 3600\n  refresh_token: false\n  refresh_strategy: >-\n    No refresh_token is issued. The docs instruct clients to read expires_in and request a new\n    token before expiry with a safety margin.\n  usage: Authorization:...Bearer <access_token> on every API request\n  errors:\n    format: RFC 6749 section 5.2 ({\"error\", \"error_description\"})\n    codes:\n      invalid_client: Wrong client_id or client_secret\n      invalid_grant: Incorrect grant_type\n      invalid_request: Invalid client credentials or refresh token\n      invalid_scope: Requested scope not allowed for this client\n  sources:\n  - https://docs.cadasto.io/docs/guides/authentication\n\
  \n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  applies_to: Cadasto Additional API (the only published document that declares a securityScheme)\n  sources:\n  - openapi/cadasto-extra-api-openapi.json\n\n- name: smart_on_openehr\n  type: oauth2\n  flow: authorizationCode\n  pkce: required for interactive flows\n  applies_to: Third-party app launch against a Cadasto tenant\n  detail: >-\n    Cadasto declares SMART-on-openEHR 1.1.0 \"Fully supported\" in its published conformance\n    statement, and publishes a pointer OpenAPI document at\n    https://docs.cadasto.io/smart-on-openehr rather than restating the specification. Redirect\n    URIs and CORS origins are registered at credential-issuance time (docs FAQ).\n  sources:\n  - https://docs.cadasto.io/smart-on-openehr\n  - https://www.cadasto.com/wp-content/uploads/2026/06/Cadasto-CDR-openEHR-conformance-statement-June-2026.pdf\n\nenvironments:\n  names: [development, acceptation, production]\n  isolation: >-\n\
  \    Credentials are issued and isolated per environment; the docs FAQ states each set must be\n    treated independently.\n\ncredential_handling_guidance:\n  published: true\n  points:\n    - Never check client_secret into source control; use a secret manager, environment variables or vault.\n    - Rotate immediately on compromise.\n    - Per-environment isolation is mandatory.\n  source: https://docs.cadasto.io/docs/faq\n\ngaps:\n  - The six openEHR ITS-REST OpenAPI documents declare no securitySchemes and an empty security\n    array, so a generated client reads them as unauthenticated. Only the Additional API document\n    declares bearerAuth.\n  - No mutualTLS, no API-key scheme, and no OpenID Connect discovery document is published on an\n    anonymously reachable host.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cadasto/refs/heads/main/authentication/cadasto-authentication.yml
summary_line: oauth2/http · 3 schemes
tags:
- Healthcare
- Health IT
- openEHR
- Electronic Health Records
- Clinical Data Repository
- Interoperability
- FHIR
- Vendor Neutral Archive
- Clinical Data
- AQL
- MCP
- Agent Skills
- Netherlands
---
