---
anonymous_access: false
api_key_in: []
api_specs:
- filename: masko-ai-analyze-api-openapi.yml
  format: yaml
  label: Masko AI Analyze API
  slug: masko-ai-analyze-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/masko-ai/openapi/masko-ai-analyze-api-openapi.yml
- filename: masko-ai-assets-api-openapi.yml
  format: yaml
  label: Masko AI Assets API
  slug: masko-ai-assets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/masko-ai/openapi/masko-ai-assets-api-openapi.yml
- filename: masko-ai-authentication-api-openapi.yml
  format: yaml
  label: Masko AI Authentication API
  slug: masko-ai-authentication-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/masko-ai/openapi/masko-ai-authentication-api-openapi.yml
- filename: masko-ai-canvases-api-openapi.yml
  format: yaml
  label: Masko AI Canvases API
  slug: masko-ai-canvases-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/masko-ai/openapi/masko-ai-canvases-api-openapi.yml
- filename: masko-ai-collections-api-openapi.yml
  format: yaml
  label: Masko AI Collections API
  slug: masko-ai-collections-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/masko-ai/openapi/masko-ai-collections-api-openapi.yml
- filename: masko-ai-credits-api-openapi.yml
  format: yaml
  label: Masko AI Credits API
  slug: masko-ai-credits-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/masko-ai/openapi/masko-ai-credits-api-openapi.yml
- filename: masko-ai-feedback-api-openapi.yml
  format: yaml
  label: Masko AI Feedback API
  slug: masko-ai-feedback-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/masko-ai/openapi/masko-ai-feedback-api-openapi.yml
- filename: masko-ai-generate-api-openapi.yml
  format: yaml
  label: Masko AI Generate API
  slug: masko-ai-generate-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/masko-ai/openapi/masko-ai-generate-api-openapi.yml
- filename: masko-ai-items-api-openapi.yml
  format: yaml
  label: Masko AI Items API
  slug: masko-ai-items-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/masko-ai/openapi/masko-ai-items-api-openapi.yml
- filename: masko-ai-jobs-api-openapi.yml
  format: yaml
  label: Masko AI Jobs API
  slug: masko-ai-jobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/masko-ai/openapi/masko-ai-jobs-api-openapi.yml
- filename: masko-ai-mascots-api-openapi.yml
  format: yaml
  label: Masko AI Mascots API
  slug: masko-ai-mascots-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/masko-ai/openapi/masko-ai-mascots-api-openapi.yml
- filename: masko-ai-projects-api-openapi.yml
  format: yaml
  label: Masko AI Projects API
  slug: masko-ai-projects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/masko-ai/openapi/masko-ai-projects-api-openapi.yml
- filename: masko-ai-references-api-openapi.yml
  format: yaml
  label: Masko AI References API
  slug: masko-ai-references-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/masko-ai/openapi/masko-ai-references-api-openapi.yml
- filename: masko-ai-settings-api-openapi.yml
  format: yaml
  label: Masko AI Settings API
  slug: masko-ai-settings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/masko-ai/openapi/masko-ai-settings-api-openapi.yml
- filename: masko-ai-sounds-api-openapi.yml
  format: yaml
  label: Masko AI Sounds API
  slug: masko-ai-sounds-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/masko-ai/openapi/masko-ai-sounds-api-openapi.yml
- filename: masko-ai-styles-api-openapi.yml
  format: yaml
  label: Masko AI Styles API
  slug: masko-ai-styles-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/masko-ai/openapi/masko-ai-styles-api-openapi.yml
- filename: masko-ai-suggestions-api-openapi.yml
  format: yaml
  label: Masko AI Suggestions API
  slug: masko-ai-suggestions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/masko-ai/openapi/masko-ai-suggestions-api-openapi.yml
- filename: masko-ai-upload-api-openapi.yml
  format: yaml
  label: Masko AI Upload API
  slug: masko-ai-upload-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/masko-ai/openapi/masko-ai-upload-api-openapi.yml
- filename: masko-ai-voice-api-openapi.yml
  format: yaml
  label: Masko AI Voice API
  slug: masko-ai-voice-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/masko-ai/openapi/masko-ai-voice-api-openapi.yml
- filename: masko-ai-webhooks-api-openapi.yml
  format: yaml
  label: Masko AI Webhooks API
  slug: masko-ai-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/masko-ai/openapi/masko-ai-webhooks-api-openapi.yml
auth_types: []
description: Masko supports API key authentication via a Bearer token and OAuth2 login for the CLI using PKCE and device code flows.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Masko AI Authentication
name_suffix: Authentication
oauth_flows: []
overview: Masko AI declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Masko AI
provider_slug: masko-ai
scheme_count: 1
schemes:
- evidence: 'Send a bearer credential with protected REST requests: an API key for a backend or script, or browser login for the Masko CLI (`masko login`).'
  header: Authorization
  how_to_obtain: Create an API key in the Masko dashboard (API keys page). The key looks like `masko_{64-hex-characters}` and is saved as `MASKO_API_KEY`.
  location: header
  name: Bearer
  type: http-bearer
slug: masko-ai-authentication
source_filename: masko-ai-authentication.yml
source_heading: Authentication Profile
source_url: https://masko.ai/docs/authentication.md
source_yaml: "generated: '2026-11-18'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://masko.ai/docs/authentication.md\nsources:\n- https://masko.ai/docs/authentication.md\n- https://masko.ai/docs/authentication/cli.md\n- https://masko.ai/docs/authentication\n- https://masko.ai/docs/authentication/cli\ndescription: Masko supports API key authentication via a Bearer token and OAuth2 login for the CLI using PKCE and device code flows.\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: 'Send a bearer credential with protected REST requests: an API key for a backend or script, or browser login for the Masko CLI (`masko\n    login`).'\n  location: header\n  header: Authorization\n  how_to_obtain: Create an API key in the Masko dashboard (API keys page). The key looks like `masko_{64-hex-characters}` and is saved as `MASKO_API_KEY`.\ndocs: https://masko.ai/docs/authentication.md\nnote: 1 extracted row(s) were dropped because their quote was not on the page.\n"
source_yaml_url: https://artifacts.apis.io/masko-ai/authentication/masko-ai-authentication.yml
summary_line: 1 scheme
tags:
- Animated Characters
- Mobile App SDK
- Web App Integration
- REST API
- Cross‑Platform Player
- Sticker Export
---
