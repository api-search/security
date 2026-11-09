---
anonymous_access: false
api_key_in: []
api_specs:
- filename: betslipdoctor-ai-board-api-openapi.yml
  format: yaml
  label: BetSlip Doctor Board API
  slug: betslipdoctor-ai-board-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/betslipdoctor-ai/openapi/betslipdoctor-ai-board-api-openapi.yml
- filename: betslipdoctor-ai-grade-api-openapi.yml
  format: yaml
  label: BetSlip Doctor Grade API
  slug: betslipdoctor-ai-grade-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/betslipdoctor-ai/openapi/betslipdoctor-ai-grade-api-openapi.yml
- filename: betslipdoctor-ai-history-api-openapi.yml
  format: yaml
  label: BetSlip Doctor History API
  slug: betslipdoctor-ai-history-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/betslipdoctor-ai/openapi/betslipdoctor-ai-history-api-openapi.yml
- filename: betslipdoctor-ai-reports-api-openapi.yml
  format: yaml
  label: BetSlip Doctor Reports API
  slug: betslipdoctor-ai-reports-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/betslipdoctor-ai/openapi/betslipdoctor-ai-reports-api-openapi.yml
- filename: betslipdoctor-ai-slips-api-openapi.yml
  format: yaml
  label: BetSlip Doctor Slips API
  slug: betslipdoctor-ai-slips-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/betslipdoctor-ai/openapi/betslipdoctor-ai-slips-api-openapi.yml
auth_types: []
description: Authentication for BetSlip Doctor agents
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Betslipdoctor Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: BetSlip Doctor declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: BetSlip Doctor
provider_slug: betslipdoctor-ai
scheme_count: 1
schemes:
- evidence: Every tool call uses OAuth 2.1 authorization code + PKCE and runs as exactly one BetSlip Doctor user.
  flows:
  - authorization_code
  how_to_obtain: Clients must register dynamically with the authorization server at https://api.betslipdoctor.ai/.well-known/oauth-authorization-server and use PKCE S256.
  name: OAuth 2.1
  scopes:
  - slips.read
  - slips.grade
  - slips.track
  - history.read
  - reports.read
  - odds.read
  - doctor.use
  - tail.read
  - tail.post
  - sportsbooks.read
  - sportsbooks.manage
  type: oauth2
slug: betslipdoctor-ai-authentication
source_filename: betslipdoctor-ai-authentication.yml
source_heading: Authentication Profile
source_url: https://betslipdoctor.ai/guides/nfl-2026-kickoff-setup-and-onside-declaration
source_yaml: "generated: '2026-11-02'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://betslipdoctor.ai/guides/nfl-2026-kickoff-setup-and-onside-declaration\nsources:\n- https://betslipdoctor.ai/guides/nfl-2026-kickoff-setup-and-onside-declaration\n- https://betslipdoctor.ai/docs/mcp-connect.md\ndescription: Authentication for BetSlip Doctor agents\nschemes:\n- type: oauth2\n  name: OAuth 2.1\n  evidence: Every tool call uses OAuth 2.1 authorization code + PKCE and runs as exactly one BetSlip Doctor user.\n  flows:\n  - authorization_code\n  scopes:\n  - slips.read\n  - slips.grade\n  - slips.track\n  - history.read\n  - reports.read\n  - odds.read\n  - doctor.use\n  - tail.read\n  - tail.post\n  - sportsbooks.read\n  - sportsbooks.manage\n  how_to_obtain: Clients must register dynamically with the authorization server at https://api.betslipdoctor.ai/.well-known/oauth-authorization-server\n    and use PKCE S256.\ndocs: https://betslipdoctor.ai/guides/nfl-2026-kickoff-setup-and-onside-declaration\n"
source_yaml_url: https://artifacts.apis.io/betslipdoctor-ai/authentication/betslipdoctor-ai-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Sports
- Betting
- Analytics
- Mobile
---
