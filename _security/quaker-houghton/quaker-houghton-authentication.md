---
anonymous_access: true
api_key_in: []
api_specs:
- filename: quaker-houghton-tribe-events-v1-openapi-original.json
  format: json
  label: Quaker Houghton Events API
  slug: quaker-houghton-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quaker-houghton/refs/heads/main/openapi/_original/quaker-houghton-tribe-events-v1-openapi-original.json
- filename: quaker-houghton-tec-v1-openapi-original.json
  format: json
  label: Quaker Houghton TEC v1 Events API
  slug: quaker-houghton-tec-v1-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quaker-houghton/refs/heads/main/openapi/_original/quaker-houghton-tec-v1-openapi-original.json
auth_types: []
description: 'Authentication profile for every machine surface home.quakerhoughton.com publishes. Three distinct postures coexist on one host: anonymous keyless reads on the Events Calendar APIs, HTTP Basic (WordPress Application Passwords) on their writes, and OAuth 2.1 with PKCE on the MCP server. Quaker Houghton publishes no authentication documentation of its own — every fact here is read from a served contract or discovery document.'
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Quaker Houghton Authentication
name_suffix: Authentication
oauth_flows: []
overview: Quaker Houghton declares 4 security scheme(s) across its OpenAPI definitions.
provider_name: Quaker Houghton
provider_slug: quaker-houghton
scheme_count: 4
schemes:
- applies_to: 'createEvent, updateEvent, deleteEvent, createOrganizer, updateOrganizer, deleteOrganizer, createVenue, updateVenue, deleteVenue (every write in tec/v1). Every read declares security: [].'
  credential: WordPress username + Application Password (the plugin's standard mechanism); no public signup exists.
  name: BasicAuth
  scheme: basic
  source: openapi/_original/quaker-houghton-tec-v1-openapi-original.json#/components/securitySchemes/BasicAuth
  surfaces:
  - tec/v1
  type: http
- evidence: GET https://home.quakerhoughton.com/wp-json/tribe/events/v1/events answered HTTP 200 with no credentials on 2026-09-17 (total 0 events). The tribe/events/v1 document declares no securitySchemes at all; its POST/DELETE operations are enforced by WordPress capability checks (rest_forbidden 401) rather than a declared scheme.
  name: anonymous
  surfaces:
  - tribe/events/v1 reads
  - tec/v1 reads
  type: none
- bearer: header
  challenge: 'HTTP 401 with WWW-Authenticate: Bearer realm="https://home.quakerhoughton.com", resource_metadata="https://home.quakerhoughton.com/.well-known/oauth-protected-resource"'
  client_registration: 'client-ID metadata document (client_id_metadata_document_supported: true); no RFC 7591 endpoint'
  detail: scopes/quaker-houghton-scopes.yml
  flows:
  - authorizationUrl: https://home.quakerhoughton.com/oauth/authorize
    flow: authorizationCode
    pkce: required (S256)
    refreshUrl: https://home.quakerhoughton.com/oauth/token
    revocationUrl: https://home.quakerhoughton.com/oauth/revoke
    scopes:
      mcp: Access the MCP server
    tokenUrl: https://home.quakerhoughton.com/oauth/token
  name: QuakerHoughtonMCPOAuth
  source: https://home.quakerhoughton.com/.well-known/oauth-authorization-server
  surfaces:
  - MCP server https://home.quakerhoughton.com/wp-json/mcp/mcp-oauth-server
  type: oauth2
- evidence: Anonymous requests answer 401 rest_forbidden with no OAuth challenge; standard WordPress REST authentication applies.
  name: WordPressSession
  surfaces:
  - https://home.quakerhoughton.com/wp-json/mcp/mcp-adapter-default-server
  - /wp-json/wp-abilities/v1/abilities
  type: cookie-or-basic
slug: quaker-houghton-authentication
source_filename: quaker-houghton-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-09-17'\nmethod: searched\nsource: >-\n  openapi/_original/quaker-houghton-tec-v1-openapi-original.json (components.securitySchemes),\n  openapi/_original/quaker-houghton-tribe-events-v1-openapi-original.json,\n  https://home.quakerhoughton.com/.well-known/oauth-authorization-server,\n  https://home.quakerhoughton.com/.well-known/oauth-protected-resource, and the\n  WWW-Authenticate challenge observed on the MCP endpoint\ndocs: null\ndescription: >-\n  Authentication profile for every machine surface home.quakerhoughton.com publishes. Three\n  distinct postures coexist on one host: anonymous keyless reads on the Events Calendar APIs,\n  HTTP Basic (WordPress Application Passwords) on their writes, and OAuth 2.1 with PKCE on the\n  MCP server. Quaker Houghton publishes no authentication documentation of its own — every\n  fact here is read from a served contract or discovery document.\nschemes:\n- name: BasicAuth\n  type: http\n  scheme: basic\n  surfaces: [tec/v1]\n\
  \  applies_to: >-\n    createEvent, updateEvent, deleteEvent, createOrganizer, updateOrganizer, deleteOrganizer,\n    createVenue, updateVenue, deleteVenue (every write in tec/v1). Every read declares security: [].\n  source: openapi/_original/quaker-houghton-tec-v1-openapi-original.json#/components/securitySchemes/BasicAuth\n  credential: WordPress username + Application Password (the plugin's standard mechanism); no public signup exists.\n- name: anonymous\n  type: none\n  surfaces: [tribe/events/v1 reads, tec/v1 reads]\n  evidence: >-\n    GET https://home.quakerhoughton.com/wp-json/tribe/events/v1/events answered HTTP 200 with no\n    credentials on 2026-09-17 (total 0 events). The tribe/events/v1 document declares no\n    securitySchemes at all; its POST/DELETE operations are enforced by WordPress capability checks\n    (rest_forbidden 401) rather than a declared scheme.\n- name: QuakerHoughtonMCPOAuth\n  type: oauth2\n  surfaces: [MCP server https://home.quakerhoughton.com/wp-json/mcp/mcp-oauth-server]\n\
  \  flows:\n  - flow: authorizationCode\n    authorizationUrl: https://home.quakerhoughton.com/oauth/authorize\n    tokenUrl: https://home.quakerhoughton.com/oauth/token\n    refreshUrl: https://home.quakerhoughton.com/oauth/token\n    revocationUrl: https://home.quakerhoughton.com/oauth/revoke\n    pkce: required (S256)\n    scopes:\n      mcp: Access the MCP server\n  bearer: header\n  challenge: >-\n    HTTP 401 with WWW-Authenticate: Bearer realm=\"https://home.quakerhoughton.com\",\n    resource_metadata=\"https://home.quakerhoughton.com/.well-known/oauth-protected-resource\"\n  client_registration: \"client-ID metadata document (client_id_metadata_document_supported: true); no RFC 7591 endpoint\"\n  source: https://home.quakerhoughton.com/.well-known/oauth-authorization-server\n  detail: scopes/quaker-houghton-scopes.yml\n- name: WordPressSession\n  type: cookie-or-basic\n  surfaces: [https://home.quakerhoughton.com/wp-json/mcp/mcp-adapter-default-server, /wp-json/wp-abilities/v1/abilities]\n\
  \  evidence: Anonymous requests answer 401 rest_forbidden with no OAuth challenge; standard WordPress REST authentication applies.\napi_keys:\n  issued: false\n  note: No developer portal, signup or key-issuance flow exists anywhere on the Quaker Houghton estate.\nx-evidence:\n  fetched: '2026-09-17'\n  probes:\n  - url: https://home.quakerhoughton.com/wp-json/tribe/events/v1/events?per_page=2\n    status: 200\n  - url: https://home.quakerhoughton.com/wp-json/mcp/mcp-oauth-server\n    status: 401\n  - url: https://home.quakerhoughton.com/wp-json/mcp/mcp-adapter-default-server\n    status: 401\n  - url: https://home.quakerhoughton.com/wp-json/wp-abilities/v1/abilities\n    status: 401\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/quaker-houghton/refs/heads/main/authentication/quaker-houghton-authentication.yml
summary_line: 4 schemes
tags:
- Industrial Fluids
- Chemicals
- Manufacturing
- Metalworking
- Lubricants
- Event
- MCP
---
