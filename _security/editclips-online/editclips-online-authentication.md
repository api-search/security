---
anonymous_access: false
api_key_in: []
api_specs:
- filename: editclips-online-balance-api-openapi.yml
  format: yaml
  label: EditClips.online Balance API
  slug: editclips-online-balance-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/editclips-online/openapi/editclips-online-balance-api-openapi.yml
- filename: editclips-online-jobs-api-openapi.yml
  format: yaml
  label: EditClips.online Jobs API
  slug: editclips-online-jobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/editclips-online/openapi/editclips-online-jobs-api-openapi.yml
- filename: editclips-online-tools-api-openapi.yml
  format: yaml
  label: EditClips.online Tools API
  slug: editclips-online-tools-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/editclips-online/openapi/editclips-online-tools-api-openapi.yml
auth_types: []
description: EditClips.online uses API keys as Bearer tokens or X‑API‑Key headers for authentication.
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: EditClips.online Authentication
name_suffix: Authentication
oauth_flows: []
overview: EditClips.online declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: EditClips.online
provider_slug: editclips-online
scheme_count: 2
schemes:
- evidence: Authentication is the same Bearer API key used by the REST API (an X-API-Key header also works).
  header: Authorization
  how_to_obtain: Create an API key from the Developer dashboard under API Keys.
  location: header
  name: Bearer
  type: http-bearer
- evidence: Authentication is the same Bearer API key used by the REST API (an X-API-Key header also works).
  header: X-API-Key
  how_to_obtain: Create an API key from the Developer dashboard under API Keys.
  location: header
  name: X-API-Key
  type: apiKey
slug: editclips-online-authentication
source_filename: editclips-online-authentication.yml
source_heading: Authentication Profile
source_url: https://editclips.online/docs/guides/mcp
source_yaml: "generated: '2026-11-06'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://editclips.online/docs/guides/mcp\nsources:\n- https://editclips.online/docs/guides/mcp\n- https://editclips.online/docs/quickstart\ndescription: EditClips.online uses API keys as Bearer tokens or X‑API‑Key headers for authentication.\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: Authentication is the same Bearer API key used by the REST API (an X-API-Key header also works).\n  location: header\n  header: Authorization\n  how_to_obtain: Create an API key from the Developer dashboard under API Keys.\n- type: apiKey\n  name: X-API-Key\n  evidence: Authentication is the same Bearer API key used by the REST API (an X-API-Key header also works).\n  location: header\n  header: X-API-Key\n  how_to_obtain: Create an API key from the Developer dashboard under API Keys.\nnote: No OAuth2 flows are documented.\ndocs: https://editclips.online/docs/guides/mcp\n"
source_yaml_url: https://artifacts.apis.io/editclips-online/authentication/editclips-online-authentication.yml
summary_line: 2 schemes
tags:
- Video Editing
- Audio Editing
- Image Editing
- AI Tools
- Browser-Based
- Privacy
- Media Processing
---
