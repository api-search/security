---
anonymous_access: true
api_key_in: []
api_specs:
- filename: tessa-tech-agent-directory-openapi.yml
  format: yaml
  label: TESSA Agent Directory API
  slug: tessa-agent-directory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tessa-tech/refs/heads/main/openapi/tessa-tech-agent-directory-openapi.yml
auth_types:
- none
- oauth2
- admin-token
description: ''
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Tessa Tech Authentication
name_suffix: Authentication
oauth_flows:
- authorizationCode
overview: TESSA Marketing & Technology secures its APIs with none, oauth2, and admin-token across 4 declared security schemes, as derived from its OpenAPI definitions. OAuth 2.0 is offered via the authorizationCode flow(s).
provider_name: TESSA Marketing & Technology
provider_slug: tessa-tech
scheme_count: 4
schemes:
- agent_note: The four side-effecting MCP tools / A2A skills (request_strategy_session, request_introduction, claim_listing, request_quote) are reachable with no credential. The only identity input is the prospect_email / claim_email the caller supplies; TESSA verifies claims out-of-band by email within one business day per the tool text.
  evidence: No WWW-Authenticate on any response; no securitySchemes in the spec; no RFC 9728 document on aiagent.tessa.tech (404).
  name: anonymous
  surfaces:
  - https://aiagent.tessa.tech/.well-known/agent-card.json
  - https://aiagent.tessa.tech/a2a (JSON-RPC; tasks/get answered with A2A -32001 for an unknown id)
  - https://aiagent.tessa.tech/mcp/ (initialize 200, tools/list 200 with 10 tools; session via mcp-session-id header)
  - https://aiagent.tessa.tech/openapi.json, /docs, /redoc, /healthz, /s, /s/{slug}/agent-card.json
  type: none
- declared_in_spec: false
  evidence: HTTP 401 {"detail":"Invalid or missing admin token"} on GET /admin/requests and GET /internal/visibility.json (2026-09-19). Header name not disclosed.
  name: admin-token
  scheme: bearer
  surfaces:
  - /admin/requests
  - /admin/first-hit
  - /internal/visibility
  - /internal/visibility.json
  type: http
- authorization_response_iss_parameter_supported: true
  bearer_methods_supported:
  - header
  client_registration: OAuth Client ID Metadata Documents (client_id_metadata_document_supported true); no /register endpoint advertised (RFC 7591 dynamic registration not offered)
  discovery:
    authorization_server: well-known/tessa-tech-oauth-authorization-server.json
    protected_resource: well-known/tessa-tech-oauth-protected-resource.json
  evidence: Anonymous POST tools/list to the resource returned 401 {"code":"mcp_unauthorized","message":"MCP authentication required."} with no WWW-Authenticate header; both discovery documents fetched 200 on 2026-09-19.
  flows:
  - authorizationUrl: https://tessa.tech/oauth/authorize
    flow: authorizationCode
    pkce: S256
    refreshUrl: https://tessa.tech/oauth/token
    revocationUrl: https://tessa.tech/oauth/revoke
    scopes:
      mcp: Access the WordPress MCP server (the only scope the authorization server advertises; no description is published).
    tokenUrl: https://tessa.tech/oauth/token
  grant_types_supported:
  - authorization_code
  - refresh_token
  issuer: https://tessa.tech
  name: wordpress-mcp-oauth
  resource: https://tessa.tech/wp-json/mcp/mcp-oauth-server
  response_types_supported:
  - code
  sources:
  - well-known/tessa-tech-oauth-authorization-server.json
  - well-known/tessa-tech-oauth-protected-resource.json
  token_endpoint_auth_methods_supported:
  - none
  type: oauth2
- evidence: The WP REST index advertises authentication.application-passwords with authorization endpoint https://tessa.tech/wp-admin/authorize-application.php. Recorded because it is published; the WordPress REST API is not one of the API entries in apis.yml.
  name: wordpress-application-passwords
  scheme: basic
  surfaces:
  - https://tessa.tech/wp-json/ (core WordPress REST API
  - wp/v2 and plugin namespaces)
  type: http
slug: tessa-tech-authentication
source_filename: tessa-tech-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: searched\ndocs: https://tessa.tech/.well-known/oauth-authorization-server\nsource: >-\n  The provider's OpenAPI (openapi/tessa-tech-agent-directory-openapi.yml) declares NO securitySchemes and no\n  security requirements, so 0-working/derive-authentication.py correctly produced nothing. This profile is\n  assembled instead from live anonymous probes of every surface on 2026-09-19 and from the two OAuth discovery\n  documents TESSA publishes on its apex (well-known/tessa-tech-oauth-authorization-server.json,\n  well-known/tessa-tech-oauth-protected-resource.json).\nsummary:\n  types: [none, oauth2, admin-token]\n  api_key_in: []\n  oauth2_flows: [authorizationCode]\n  note: >-\n    Three distinct postures on two hosts. (1) Everything on aiagent.tessa.tech that an agent uses — the agent card,\n    the A2A JSON-RPC endpoint, the MCP server (initialize + tools/list), the OpenAPI, the service-card fleet — is\n    ANONYMOUS: no credential was sent\
  \ to any of them and none challenged. (2) A handful of operator routes on the\n    same host (/admin/*, /internal/*) answer 401 {\"detail\":\"Invalid or missing admin token\"} — a bearer/admin token\n    the OpenAPI does not describe. (3) The WordPress MCP server on tessa.tech is OAuth 2.1: RFC 8414 metadata names\n    the issuer, endpoints, PKCE S256, public clients only (token_endpoint_auth_methods_supported [\"none\"]), a single\n    scope \"mcp\", and client_id_metadata_document_supported true — the MCP-authorization client-registration\n    pattern in which the client_id is an https URL to a metadata document instead of a pre-registered id.\nschemes:\n  - name: anonymous\n    type: none\n    surfaces:\n      - https://aiagent.tessa.tech/.well-known/agent-card.json\n      - https://aiagent.tessa.tech/a2a (JSON-RPC; tasks/get answered with A2A -32001 for an unknown id)\n      - https://aiagent.tessa.tech/mcp/ (initialize 200, tools/list 200 with 10 tools; session via mcp-session-id\
  \ header)\n      - https://aiagent.tessa.tech/openapi.json, /docs, /redoc, /healthz, /s, /s/{slug}/agent-card.json\n    evidence: No WWW-Authenticate on any response; no securitySchemes in the spec; no RFC 9728 document on aiagent.tessa.tech (404).\n    agent_note: >-\n      The four side-effecting MCP tools / A2A skills (request_strategy_session, request_introduction, claim_listing,\n      request_quote) are reachable with no credential. The only identity input is the prospect_email / claim_email\n      the caller supplies; TESSA verifies claims out-of-band by email within one business day per the tool text.\n  - name: admin-token\n    type: http\n    scheme: bearer\n    declared_in_spec: false\n    surfaces: [/admin/requests, /admin/first-hit, /internal/visibility, /internal/visibility.json]\n    evidence: 'HTTP 401 {\"detail\":\"Invalid or missing admin token\"} on GET /admin/requests and GET /internal/visibility.json (2026-09-19). Header name not disclosed.'\n  - name: wordpress-mcp-oauth\n\
  \    type: oauth2\n    resource: https://tessa.tech/wp-json/mcp/mcp-oauth-server\n    flows:\n      - flow: authorizationCode\n        authorizationUrl: https://tessa.tech/oauth/authorize\n        tokenUrl: https://tessa.tech/oauth/token\n        refreshUrl: https://tessa.tech/oauth/token\n        revocationUrl: https://tessa.tech/oauth/revoke\n        pkce: S256\n        scopes:\n          mcp: Access the WordPress MCP server (the only scope the authorization server advertises; no description is published).\n    issuer: https://tessa.tech\n    response_types_supported: [code]\n    grant_types_supported: [authorization_code, refresh_token]\n    token_endpoint_auth_methods_supported: [none]\n    client_registration: OAuth Client ID Metadata Documents (client_id_metadata_document_supported true); no /register endpoint advertised (RFC 7591 dynamic registration not offered)\n    authorization_response_iss_parameter_supported: true\n    bearer_methods_supported: [header]\n    discovery:\n \
  \     authorization_server: well-known/tessa-tech-oauth-authorization-server.json\n      protected_resource: well-known/tessa-tech-oauth-protected-resource.json\n    evidence: >-\n      Anonymous POST tools/list to the resource returned 401 {\"code\":\"mcp_unauthorized\",\"message\":\"MCP authentication\n      required.\"} with no WWW-Authenticate header; both discovery documents fetched 200 on 2026-09-19.\n    sources: [well-known/tessa-tech-oauth-authorization-server.json, well-known/tessa-tech-oauth-protected-resource.json]\n  - name: wordpress-application-passwords\n    type: http\n    scheme: basic\n    surfaces: [https://tessa.tech/wp-json/ (core WordPress REST API, wp/v2 and plugin namespaces)]\n    evidence: 'The WP REST index advertises authentication.application-passwords with authorization endpoint https://tessa.tech/wp-admin/authorize-application.php. Recorded because it is published; the WordPress REST API is not one of the API entries in apis.yml.'\nsee_also:\n  scopes: scopes/tessa-tech-scopes.yml\n\
  \  mcp: mcp/tessa-tech-mcp.yml\n  well_known: well-known/tessa-tech-well-known.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tessa-tech/refs/heads/main/authentication/tessa-tech-authentication.yml
summary_line: none/oauth2/admin-token · 4 schemes
tags:
- Digital Marketing
- SEO
- Web Development
- Accessibility
- AI Agent Readiness
- Professional Services
- Agent Directory
- A2A
- MCP
- Agent-Native
- Company
---
