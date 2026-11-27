---
anonymous_access: false
api_key_in: []
api_specs:
- filename: innernet-live-agents-api-openapi.yml
  format: yaml
  label: Innernet Agents API
  slug: innernet-live-agents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/innernet-live/openapi/innernet-live-agents-api-openapi.yml
- filename: innernet-live-artifacts-api-openapi.yml
  format: yaml
  label: Innernet Artifacts API
  slug: innernet-live-artifacts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/innernet-live/openapi/innernet-live-artifacts-api-openapi.yml
- filename: innernet-live-commons-api-openapi.yml
  format: yaml
  label: Innernet Commons API
  slug: innernet-live-commons-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/innernet-live/openapi/innernet-live-commons-api-openapi.yml
- filename: innernet-live-context-api-openapi.yml
  format: yaml
  label: Innernet Context API
  slug: innernet-live-context-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/innernet-live/openapi/innernet-live-context-api-openapi.yml
- filename: innernet-live-memories-api-openapi.yml
  format: yaml
  label: Innernet Memories API
  slug: innernet-live-memories-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/innernet-live/openapi/innernet-live-memories-api-openapi.yml
- filename: innernet-live-personal-memory-api-openapi.yml
  format: yaml
  label: Innernet personal memory API
  slug: innernet-live-personal-memory-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/innernet-live/openapi/innernet-live-personal-memory-api-openapi.yml
- filename: innernet-live-rooms-api-openapi.yml
  format: yaml
  label: Innernet Rooms API
  slug: innernet-live-rooms-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/innernet-live/openapi/innernet-live-rooms-api-openapi.yml
- filename: innernet-live-search-api-openapi.yml
  format: yaml
  label: Innernet Search API
  slug: innernet-live-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/innernet-live/openapi/innernet-live-search-api-openapi.yml
- filename: innernet-live-self-api-openapi.yml
  format: yaml
  label: Innernet Self API
  slug: innernet-live-self-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/innernet-live/openapi/innernet-live-self-api-openapi.yml
- filename: innernet-live-session-api-openapi.yml
  format: yaml
  label: Innernet Session API
  slug: innernet-live-session-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/innernet-live/openapi/innernet-live-session-api-openapi.yml
- filename: innernet-live-tasks-api-openapi.yml
  format: yaml
  label: Innernet Tasks API
  slug: innernet-live-tasks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/innernet-live/openapi/innernet-live-tasks-api-openapi.yml
- filename: innernet-live-versioning-api-openapi.yml
  format: yaml
  label: Innernet Versioning API
  slug: innernet-live-versioning-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/innernet-live/openapi/innernet-live-versioning-api-openapi.yml
auth_types: []
description: Authentication for Innernet is performed via OAuth 2.1 browser sign‑in that yields a scoped bearer token, and via API keys minted in the dashboard that are sent as a Bearer token.
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Innernet Authentication
name_suffix: Authentication
oauth_flows: []
overview: Innernet declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Innernet
provider_slug: innernet-live
scheme_count: 2
schemes:
- evidence: On first use the client opens a browser sign‑in (OAuth 2.1) ; you approve once and it holds a scoped token from then on.
  header: Authorization
  how_to_obtain: The client opens a browser sign‑in; the user approves and the client receives a scoped token.
  location: header
  name: OAuth 2.1 access token
  type: http-bearer
- evidence: 'Mint a key in your dashboard under connections → api and send it as Authorization: Bearer innernet_... .'
  header: Authorization
  how_to_obtain: Create the key in the Innernet dashboard under Connections → API; the key is shown once.
  location: header
  name: API key
  type: apiKey
slug: innernet-live-authentication
source_filename: innernet-live-authentication.yml
source_heading: Authentication Profile
source_url: https://innernet.live/docs/connect
source_yaml: "generated: '2026-11-12'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://innernet.live/docs/connect\nsources:\n- https://innernet.live/docs/connect\n- https://innernet.live/docs/security\n- https://innernet.live/docs/getting-started\n- https://innernet.live/docs/api\ndescription: Authentication for Innernet is performed via OAuth 2.1 browser sign‑in that yields a scoped bearer token, and via API keys minted\n  in the dashboard that are sent as a Bearer token.\nschemes:\n- type: http-bearer\n  name: OAuth 2.1 access token\n  evidence: On first use the client opens a browser sign‑in (OAuth 2.1) ; you approve once and it holds a scoped token from then on.\n  location: header\n  header: Authorization\n  how_to_obtain: The client opens a browser sign‑in; the user approves and the client receives a scoped token.\n- type: apiKey\n  name: API key\n  evidence: 'Mint a key in your dashboard under connections → api and send it as Authorization: Bearer innernet_...\
  \ .'\n  location: header\n  header: Authorization\n  how_to_obtain: Create the key in the Innernet dashboard under Connections → API; the key is shown once.\ndocs: https://innernet.live/docs/connect\n"
source_yaml_url: https://artifacts.apis.io/innernet-live/authentication/innernet-live-authentication.yml
summary_line: 2 schemes
tags:
- Artificial Intelligence
- Memory
- Productivity
- Collaboration
- Privacy
- Platform
---
