---
anonymous_access: false
api_key_in: []
api_specs:
- filename: opentrack-containers-api-openapi.yml
  format: yaml
  label: OpenTrack /containers API
  slug: opentrack-containers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/opentrack/openapi/opentrack-containers-api-openapi.yml
- filename: opentrack-events-api-openapi.yml
  format: yaml
  label: OpenTrack /events API
  slug: opentrack-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/opentrack/openapi/opentrack-events-api-openapi.yml
- filename: opentrack-master-bills-api-openapi.yml
  format: yaml
  label: OpenTrack /master Bills API
  slug: opentrack-master-bills-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/opentrack/openapi/opentrack-master-bills-api-openapi.yml
- filename: opentrack-v1-partners-ingestion-api-openapi.yml
  format: yaml
  label: OpenTrack /v1/partners/ingestion API
  slug: opentrack-v1-partners-ingestion-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/opentrack/openapi/opentrack-v1-partners-ingestion-api-openapi.yml
- filename: opentrack-webhooks-api-openapi.yml
  format: yaml
  label: OpenTrack /webhooks API
  slug: opentrack-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/opentrack/openapi/opentrack-webhooks-api-openapi.yml
auth_types: []
description: Authentication schemes published on the OpenTrack documentation pages.
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: OpenTrack Authentication
name_suffix: Authentication
oauth_flows: []
overview: OpenTrack declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: OpenTrack
provider_slug: opentrack
scheme_count: 2
schemes:
- evidence: Include this API key in the header of your requests to authenticate with the OpenTrack API.
  header: Opentrack-API-Key
  how_to_obtain: Log in to the OpenTrack dashboard, navigate to Settings → Developers, and copy your Opentrack-API-Key.
  location: header
  name: Opentrack-API-Key
  type: apiKey
- evidence: Sign in through your browser when you connect. There is no API key to paste.
  how_to_obtain: Sign in through the browser when connecting an MCP client; no API key is required.
  name: MCP browser sign‑in
  type: other
slug: opentrack-authentication
source_filename: opentrack-authentication.yml
source_heading: Authentication Profile
source_url: https://developers.opentrack.co/docs/getting-started.md
source_yaml: "generated: '2026-11-15'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://developers.opentrack.co/docs/getting-started.md\nsources:\n- https://developers.opentrack.co/docs/getting-started.md\n- https://developers.opentrack.co/docs/getting-started\n- https://developers.opentrack.co/docs/mcp\ndescription: Authentication schemes published on the OpenTrack documentation pages.\nschemes:\n- type: apiKey\n  name: Opentrack-API-Key\n  evidence: Include this API key in the header of your requests to authenticate with the OpenTrack API.\n  location: header\n  header: Opentrack-API-Key\n  how_to_obtain: Log in to the OpenTrack dashboard, navigate to Settings → Developers, and copy your Opentrack-API-Key.\n- type: other\n  name: MCP browser sign‑in\n  evidence: Sign in through your browser when you connect. There is no API key to paste.\n  how_to_obtain: Sign in through the browser when connecting an MCP client; no API key is required.\ndocs: https://developers.opentrack.co/docs/getting-started.md\n"
source_yaml_url: https://artifacts.apis.io/opentrack/authentication/opentrack-authentication.yml
summary_line: 2 schemes
tags:
- Container Visibility
- Freight Tracking
- Logistics Software
- API Integration
- Supply Chain Analytics
- Customs Data
---
