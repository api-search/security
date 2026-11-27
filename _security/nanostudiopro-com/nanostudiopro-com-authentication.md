---
anonymous_access: false
api_key_in: []
api_specs:
- filename: nanostudiopro-com-account-api-openapi.yml
  format: yaml
  label: Nano Studio Pro Account API
  slug: nanostudiopro-com-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nanostudiopro-com/openapi/nanostudiopro-com-account-api-openapi.yml
- filename: nanostudiopro-com-assets-api-openapi.yml
  format: yaml
  label: Nano Studio Pro Assets API
  slug: nanostudiopro-com-assets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nanostudiopro-com/openapi/nanostudiopro-com-assets-api-openapi.yml
- filename: nanostudiopro-com-cutouts-api-openapi.yml
  format: yaml
  label: Nano Studio Pro Cutouts API
  slug: nanostudiopro-com-cutouts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nanostudiopro-com/openapi/nanostudiopro-com-cutouts-api-openapi.yml
- filename: nanostudiopro-com-detections-api-openapi.yml
  format: yaml
  label: Nano Studio Pro Detections API
  slug: nanostudiopro-com-detections-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nanostudiopro-com/openapi/nanostudiopro-com-detections-api-openapi.yml
- filename: nanostudiopro-com-device-auth-api-openapi.yml
  format: yaml
  label: Nano Studio Pro Device Auth API
  slug: nanostudiopro-com-device-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nanostudiopro-com/openapi/nanostudiopro-com-device-auth-api-openapi.yml
- filename: nanostudiopro-com-editing-api-openapi.yml
  format: yaml
  label: Nano Studio Pro Editing API
  slug: nanostudiopro-com-editing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nanostudiopro-com/openapi/nanostudiopro-com-editing-api-openapi.yml
- filename: nanostudiopro-com-entities-api-openapi.yml
  format: yaml
  label: Nano Studio Pro Entities API
  slug: nanostudiopro-com-entities-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nanostudiopro-com/openapi/nanostudiopro-com-entities-api-openapi.yml
- filename: nanostudiopro-com-generations-api-openapi.yml
  format: yaml
  label: Nano Studio Pro Generations API
  slug: nanostudiopro-com-generations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nanostudiopro-com/openapi/nanostudiopro-com-generations-api-openapi.yml
- filename: nanostudiopro-com-media-api-openapi.yml
  format: yaml
  label: Nano Studio Pro Media API
  slug: nanostudiopro-com-media-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nanostudiopro-com/openapi/nanostudiopro-com-media-api-openapi.yml
- filename: nanostudiopro-com-projects-api-openapi.yml
  format: yaml
  label: Nano Studio Pro Projects API
  slug: nanostudiopro-com-projects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nanostudiopro-com/openapi/nanostudiopro-com-projects-api-openapi.yml
- filename: nanostudiopro-com-search-api-openapi.yml
  format: yaml
  label: Nano Studio Pro Search API
  slug: nanostudiopro-com-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nanostudiopro-com/openapi/nanostudiopro-com-search-api-openapi.yml
- filename: nanostudiopro-com-sheets-api-openapi.yml
  format: yaml
  label: Nano Studio Pro Sheets API
  slug: nanostudiopro-com-sheets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nanostudiopro-com/openapi/nanostudiopro-com-sheets-api-openapi.yml
- filename: nanostudiopro-com-sounds-api-openapi.yml
  format: yaml
  label: Nano Studio Pro Sounds API
  slug: nanostudiopro-com-sounds-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nanostudiopro-com/openapi/nanostudiopro-com-sounds-api-openapi.yml
- filename: nanostudiopro-com-storyboards-api-openapi.yml
  format: yaml
  label: Nano Studio Pro Storyboards API
  slug: nanostudiopro-com-storyboards-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nanostudiopro-com/openapi/nanostudiopro-com-storyboards-api-openapi.yml
- filename: nanostudiopro-com-tasks-api-openapi.yml
  format: yaml
  label: Nano Studio Pro Tasks API
  slug: nanostudiopro-com-tasks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nanostudiopro-com/openapi/nanostudiopro-com-tasks-api-openapi.yml
- filename: nanostudiopro-com-video-api-openapi.yml
  format: yaml
  label: Nano Studio Pro Video API
  slug: nanostudiopro-com-video-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nanostudiopro-com/openapi/nanostudiopro-com-video-api-openapi.yml
- filename: nanostudiopro-com-videos-api-openapi.yml
  format: yaml
  label: Nano Studio Pro Videos API
  slug: nanostudiopro-com-videos-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nanostudiopro-com/openapi/nanostudiopro-com-videos-api-openapi.yml
auth_types: []
description: Authentication methods published on Nano Studio Pro documentation
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Nano Studio Pro Authentication
name_suffix: Authentication
oauth_flows: []
overview: Nano Studio Pro declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Nano Studio Pro
provider_slug: nanostudiopro-com
scheme_count: 2
schemes:
- evidence: Implements OAuth 2.0 Device Authorization Grant (RFC 8628) — the same flow gh auth login , vercel login , and gcloud auth login use.
  flows:
  - device_code
  how_to_obtain: Request a device code via POST https://nanostudiopro.com/api/device/code, have the user approve at the verification URL, then poll the token endpoint.
  name: Device Authorization
  scopes:
  - read
  - write
  token_url: https://nanostudiopro.com/api/device/token
  type: oauth2
- evidence: The token is a regular Personal Access Token. It works with every endpoint under /api/v1 .
  header: Authorization
  how_to_obtain: Obtain a personal access token via the device flow or from Settings · API Tokens.
  name: Bearer Token
  type: http-bearer
slug: nanostudiopro-com-authentication
source_filename: nanostudiopro-com-authentication.yml
source_heading: Authentication Profile
source_url: https://nanostudiopro.com/docs/device-auth
source_yaml: "generated: '2026-11-19'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://nanostudiopro.com/docs/device-auth\nsources:\n- https://nanostudiopro.com/docs/device-auth\n- https://nanostudiopro.com/\n- https://nanostudiopro.com/\ndescription: Authentication methods published on Nano Studio Pro documentation\nschemes:\n- type: oauth2\n  name: Device Authorization\n  evidence: Implements OAuth 2.0 Device Authorization Grant (RFC 8628) — the same flow gh auth login , vercel login , and gcloud auth login use.\n  flows:\n  - device_code\n  token_url: https://nanostudiopro.com/api/device/token\n  scopes:\n  - read\n  - write\n  how_to_obtain: Request a device code via POST https://nanostudiopro.com/api/device/code, have the user approve at the verification URL, then\n    poll the token endpoint.\n- type: http-bearer\n  name: Bearer Token\n  evidence: The token is a regular Personal Access Token. It works with every endpoint under /api/v1 .\n  header: Authorization\n\
  \  how_to_obtain: Obtain a personal access token via the device flow or from Settings · API Tokens.\ndocs: https://nanostudiopro.com/docs/device-auth\n"
source_yaml_url: https://artifacts.apis.io/nanostudiopro-com/authentication/nanostudiopro-com-authentication.yml
summary_line: 2 schemes
tags:
- AI Image Editor
- AI Video Generation
- Interactive Storyboards
- Character Creator
- Font Generator
- Search Engines
- E-Commerce
---
