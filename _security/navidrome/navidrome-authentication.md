---
anonymous_access: false
api_key_in: []
api_specs:
- filename: navidrome-server-api-openapi.yml
  format: yaml
  label: Navidrome Server API
  slug: navidrome-server-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/navidrome/openapi/navidrome-server-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Navidrome Authentication
name_suffix: Authentication
oauth_flows: []
overview: Navidrome declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Navidrome
provider_slug: navidrome
scheme_count: 1
schemes:
- description: Authentication via reverse proxy forwarding the authenticated user in the Remote-User HTTP header (configurable via ExtAuth.UserHeader).
  header: Remote-User
  notes: Enabled when ExtAuth.TrustedSources is configured; Navidrome validates source IP before trusting the header.
  type: externalized
slug: navidrome-authentication
source_filename: navidrome-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-10-28'\nmethod: searched\nsource:\n  - https://www.navidrome.org/docs/getting-started/extauth-quickstart/\n  - https://www.navidrome.org/docs/usage/integration/authentication\nschemes:\n  - type: externalized\n    description: \"Authentication via reverse proxy forwarding the authenticated user in the Remote-User HTTP header (configurable via ExtAuth.UserHeader).\"\n    header: Remote-User\n    notes: \"Enabled when ExtAuth.TrustedSources is configured; Navidrome validates source IP before trusting the header.\"\n"
source_yaml_url: https://artifacts.apis.io/navidrome/authentication/navidrome-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Music
- Streaming
- Self-Hosted
- Open-Source
- Media-Server
---
