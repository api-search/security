---
anonymous_access: false
api_key_in: []
auth_types: []
description: MapsData uses a simple bearer token authentication scheme.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: MapsData Authentication
name_suffix: Authentication
oauth_flows: []
overview: MapsData declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: MapsData
provider_slug: mapsdata-ai
scheme_count: 1
schemes:
- evidence: 'Authentication is a bearer token: your MapsData API key, created in Settings.'
  header: Authorization
  how_to_obtain: Create a key in Settings under API keys.
  location: header
  name: Bearer
  scopes:
  - scrape:read
  - scrape:write
  type: http-bearer
slug: mapsdata-ai-authentication
source_filename: mapsdata-ai-authentication.yml
source_heading: Authentication Profile
source_url: https://mapsdata.ai/api-authentication
source_yaml: "generated: '2026-11-17'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://mapsdata.ai/api-authentication\nsources:\n- https://mapsdata.ai/api-authentication\n- https://mapsdata.ai/api-mcp\ndescription: MapsData uses a simple bearer token authentication scheme.\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: 'Authentication is a bearer token: your MapsData API key, created in Settings.'\n  location: header\n  header: Authorization\n  scopes:\n  - scrape:read\n  - scrape:write\n  how_to_obtain: Create a key in Settings under API keys.\nnote: The documentation mentions that hosted connectors can use OAuth 2.0 with an authorization code flow and PKCE, but no token or authorization\n  URLs are provided, so no OAuth scheme is listed.\ndocs: https://mapsdata.ai/api-authentication\n"
source_yaml_url: https://artifacts.apis.io/mapsdata-ai/authentication/mapsdata-ai-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Lead Generation
- Google Maps
- Email Scraping
- B2B
---
