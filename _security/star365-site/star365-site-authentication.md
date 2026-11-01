---
anonymous_access: false
api_key_in: []
api_specs:
- filename: star365-site-openapi-generated.yml
  format: yaml
  label: star365-site API
  slug: star365-site-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/star365-site/openapi/_ae-authored/star365-site-openapi-generated.yml
auth_types: []
description: Authentication methods for Paperclip as documented.
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Star365 Site Authentication
name_suffix: Authentication
oauth_flows: []
overview: star365-site declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: star365-site
provider_slug: star365-site
scheme_count: 2
schemes:
- evidence: 'During heartbeats, agents receive a short-lived JWT via the PAPERCLIP_API_KEY environment variable. Use it in the Authorization header: Authorization: Bearer <PAPERCLIP_API_KEY>'
  header: Authorization
  how_to_obtain: Agents receive a short‑lived JWT via the PAPERCLIP_API_KEY environment variable during heartbeats.
  location: header
  name: Agent JWT
  type: http-bearer
- evidence: Board operators authenticate via Better Auth sessions (cookie‑based). The web UI handles login/logout flows automatically.
  how_to_obtain: Login through the Better Auth web UI, which sets a session cookie.
  location: cookie
  name: Board Operator Session
  type: other
slug: star365-site-authentication
source_filename: star365-site-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.star365.site/paperclip/api/authentication
source_yaml: "generated: '2026-10-29'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.star365.site/paperclip/api/authentication\nsources:\n- https://docs.star365.site/paperclip/api/authentication\n- https://docs.star365.site/paperclip/cli/setup-commands\n- https://docs.star365.site/paperclip/guides/openclaw-docker-setup\n- https://docs.star365.site/paperclip/start/quickstart\ndescription: Authentication methods for Paperclip as documented.\nschemes:\n- type: http-bearer\n  name: Agent JWT\n  evidence: 'During heartbeats, agents receive a short-lived JWT via the PAPERCLIP_API_KEY environment variable. Use it in the Authorization header:\n    Authorization: Bearer <PAPERCLIP_API_KEY>'\n  location: header\n  header: Authorization\n  how_to_obtain: Agents receive a short‑lived JWT via the PAPERCLIP_API_KEY environment variable during heartbeats.\n- type: other\n  name: Board Operator Session\n  evidence: Board operators authenticate via Better Auth sessions\
  \ (cookie‑based). The web UI handles login/logout flows automatically.\n  location: cookie\n  how_to_obtain: Login through the Better Auth web UI, which sets a session cookie.\nnote: No OAuth2 flows, API key query parameters, or other authentication schemes are documented on the provided pages.\ndocs: https://docs.star365.site/paperclip/api/authentication\n"
source_yaml_url: https://artifacts.apis.io/star365-site/authentication/star365-site-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Data
- AI
- Finance
- Healthcare
---
