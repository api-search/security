---
anonymous_access: false
api_key_in: []
api_specs:
- filename: agentanalytics-sh-api-openapi.yml
  format: yaml
  label: Agent Analytics API API
  slug: agent-analytics-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentanalytics-sh/openapi/_original/agentanalytics-sh-api-openapi.yml
auth_types: []
description: 'Agent Analytics uses three credential types: agent sessions (bearer tokens), API keys, and project tokens.'
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Agentanalytics Sh Authentication
name_suffix: Authentication
oauth_flows: []
overview: Agent Analytics declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: Agent Analytics
provider_slug: agentanalytics-sh
scheme_count: 3
schemes:
- evidence: Agent Analytics uses three different credentials. They serve different jobs and should not be swapped.
  header: Authorization
  how_to_obtain: Obtained via the hosted browser approval flow or CLI login, stored locally.
  location: header
  name: Agent session
  type: http-bearer
- evidence: Pass it with the X-API-Key header or the ?key= query parameter.
  header: X-API-Key
  how_to_obtain: Generate from the dashboard (app.agentanalytics.sh) for server‑side use.
  location: header/query
  name: API key
  type: apiKey
- evidence: The token is public by design. It identifies the project for event ingestion and is expected to appear in HTML.
  how_to_obtain: Embedded in the tracker script tag on the client side.
  location: query
  name: Project token
  type: apiKey
slug: agentanalytics-sh-authentication
source_filename: agentanalytics-sh-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.agentanalytics.sh/reference/authentication/
source_yaml: "generated: '2026-10-31'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.agentanalytics.sh/reference/authentication/\nsources:\n- https://docs.agentanalytics.sh/reference/authentication/\n- https://docs.agentanalytics.sh/reference/authentication/\n- https://docs.agentanalytics.sh/reference/auth-md/\n- https://docs.agentanalytics.sh/getting-started/\ndescription: 'Agent Analytics uses three credential types: agent sessions (bearer tokens), API keys, and project tokens.'\nschemes:\n- type: http-bearer\n  name: Agent session\n  evidence: Agent Analytics uses three different credentials. They serve different jobs and should not be swapped.\n  location: header\n  header: Authorization\n  how_to_obtain: Obtained via the hosted browser approval flow or CLI login, stored locally.\n- type: apiKey\n  name: API key\n  evidence: Pass it with the X-API-Key header or the ?key= query parameter.\n  location: header/query\n  header: X-API-Key\n  how_to_obtain:\
  \ Generate from the dashboard (app.agentanalytics.sh) for server‑side use.\n- type: apiKey\n  name: Project token\n  evidence: The token is public by design. It identifies the project for event ingestion and is expected to appear in HTML.\n  location: query\n  how_to_obtain: Embedded in the tracker script tag on the client side.\nnote: No OAuth2 flows, token URLs, or scopes are explicitly documented.\ndocs: https://docs.agentanalytics.sh/reference/authentication/\n"
source_yaml_url: https://artifacts.apis.io/agentanalytics-sh/authentication/agentanalytics-sh-authentication.yml
summary_line: 3 schemes
tags:
- Analytics
- Artificial Intelligence
- Web Analytics
- Open Source
- Software-as-a-Service
---
