---
anonymous_access: false
api_key_in: []
api_specs:
- filename: falconbuilder-dev-openapi-generated.yml
  format: yaml
  label: Falcon Builder API
  slug: falconbuilder-dev-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/falconbuilder-dev/openapi/_ae-authored/falconbuilder-dev-openapi-generated.yml
auth_types: []
description: Authentication schemes for Falcon Builder
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Falcon Builder Authentication
name_suffix: Authentication
oauth_flows: []
overview: Falcon Builder declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Falcon Builder
provider_slug: falconbuilder-dev
scheme_count: 2
schemes:
- evidence: Generic API key credential for HTTP requests.
  header: X-API-Key
  how_to_obtain: Store any API key securely and use it across HTTP Request nodes.
  location: header
  name: Custom API Key
  type: apiKey
- evidence: User-managed Zoom OAuth app — no admin role or paid plan needed.
  how_to_obtain: Paste the Client ID and Secret, then the meeting host authorizes with one click.
  name: Zoom (User OAuth)
  scopes:
  - meeting:read:meeting
  - meeting:read:list_meetings
  - meeting:write:meeting
  - meeting:update:meeting
  - meeting:delete:meeting
  type: oauth2
slug: falconbuilder-dev-authentication
source_filename: falconbuilder-dev-authentication.yml
source_heading: Authentication Profile
source_url: https://www.falconbuilder.dev/docs/credentials/custom-api-key.md
source_yaml: "generated: '2026-11-07'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://www.falconbuilder.dev/docs/credentials/custom-api-key.md\nsources:\n- https://www.falconbuilder.dev/docs/credentials/custom-api-key.md\n- https://www.falconbuilder.dev/docs/credentials/custom-api-key.md\n- https://www.falconbuilder.dev/docs/credentials/zoom-oauth\n- https://www.falconbuilder.dev/docs/credentials/zoom-oauth.md\ndescription: Authentication schemes for Falcon Builder\nschemes:\n- type: apiKey\n  name: Custom API Key\n  evidence: Generic API key credential for HTTP requests.\n  location: header\n  header: X-API-Key\n  how_to_obtain: Store any API key securely and use it across HTTP Request nodes.\n- type: oauth2\n  name: Zoom (User OAuth)\n  evidence: User-managed Zoom OAuth app — no admin role or paid plan needed.\n  scopes:\n  - meeting:read:meeting\n  - meeting:read:list_meetings\n  - meeting:write:meeting\n  - meeting:update:meeting\n  - meeting:delete:meeting\n\
  \  how_to_obtain: Paste the Client ID and Secret, then the meeting host authorizes with one click.\ndocs: https://www.falconbuilder.dev/docs/credentials/custom-api-key.md\n"
source_yaml_url: https://artifacts.apis.io/falconbuilder-dev/authentication/falconbuilder-dev-authentication.yml
summary_line: 2 schemes
tags:
- Artificial Intelligence
- No-Code
- Platform
- Automation
- Workflows
---
