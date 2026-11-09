---
anonymous_access: false
api_key_in: []
api_specs:
- filename: dodomain-io-api-openapi.json
  format: json
  label: DoDomain API API
  slug: dodomain-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dodomain-io/openapi/_original/dodomain-io-api-openapi.json
auth_types: []
description: Authentication methods as described on DoDomain documentation.
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Dodomain Io Authentication
name_suffix: Authentication
oauth_flows: []
overview: DoDomain declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: DoDomain
provider_slug: dodomain-io
scheme_count: 2
schemes:
- evidence: 'OAuth access token : the credential AI assistants use, sent as Authorization: Bearer <token> .'
  header: Authorization
  how_to_obtain: Obtain via OAuth consent flow; requires apps:write scope and appropriate team role.
  location: header
  name: OAuth access token
  type: http-bearer
- evidence: 'Session token ( dd_sess_... ): a single-session capability returned by POST /api/v1/sessions . Session-scoped endpoints are public and authorize by the unguessable token itself.'
  header: Authorization
  how_to_obtain: Create a session via POST /api/v1/sessions; the response includes a token.
  location: header
  name: Session token
  type: http-bearer
slug: dodomain-io-authentication
source_filename: dodomain-io-authentication.yml
source_heading: Authentication Profile
source_url: https://dodomain.io/docs/api
source_yaml: "generated: '2026-11-05'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://dodomain.io/docs/api\nsources:\n- https://dodomain.io/docs/api\n- https://dev.dodomain.io/domain-connect/cloudflare\n- https://dodomain.io/agent-setup/prompt.md\n- https://dodomain.io/docs/getting-started\ndescription: Authentication methods as described on DoDomain documentation.\nschemes:\n- type: http-bearer\n  name: OAuth access token\n  evidence: 'OAuth access token : the credential AI assistants use, sent as Authorization: Bearer <token> .'\n  location: header\n  header: Authorization\n  how_to_obtain: Obtain via OAuth consent flow; requires apps:write scope and appropriate team role.\n- type: http-bearer\n  name: Session token\n  evidence: 'Session token ( dd_sess_... ): a single-session capability returned by POST /api/v1/sessions . Session-scoped endpoints are public\n    and authorize by the unguessable token itself.'\n  location: header\n  header: Authorization\n\
  \  how_to_obtain: Create a session via POST /api/v1/sessions; the response includes a token.\nnote: No OAuth flow URLs or scopes are explicitly listed in the documentation; therefore token_url, authorize_url, and scopes are left empty.\n  1 extracted row(s) were dropped because their quote was not on the page.\ndocs: https://dodomain.io/docs/api\n"
source_yaml_url: https://artifacts.apis.io/dodomain-io/authentication/dodomain-io-authentication.yml
summary_line: 2 schemes
tags:
- Software-as-a-Service
- DNS
- CustomDomain
- Integration
---
