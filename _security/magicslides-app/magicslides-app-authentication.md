---
anonymous_access: false
api_key_in: []
api_specs:
- filename: magicslides-app-presentations-api-openapi.yml
  format: yaml
  label: MagicSlides Presentations API
  slug: magicslides-app-presentations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/magicslides-app/openapi/magicslides-app-presentations-api-openapi.yml
- filename: magicslides-app-studio-api-openapi.yml
  format: yaml
  label: MagicSlides Studio API
  slug: magicslides-app-studio-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/magicslides-app/openapi/magicslides-app-studio-api-openapi.yml
auth_types: []
description: Authentication methods for MagicSlides API
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: MagicSlides Authentication
name_suffix: Authentication
oauth_flows: []
overview: MagicSlides declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: MagicSlides
provider_slug: magicslides-app
scheme_count: 2
schemes:
- evidence: Include your API key in the request body using the `apiKey` parameter.
  how_to_obtain: 'Log in to your MagicSlides dashboard, navigate to /dashboard/settings, generate a new API key and copy it (format: ms‑api‑{base64‑encoded‑payload}.{secret})'
  location: body
  name: apiKey
  type: apiKey
- evidence: Include both `email` and `accessId` in the request body.
  how_to_obtain: Find your access ID in the MagicSlides dashboard under API Settings and use your account email
  location: body
  name: email_accessId
  type: apiKey
slug: magicslides-app-authentication
source_filename: magicslides-app-authentication.yml
source_heading: Authentication Profile
source_url: https://www.magicslides.app/docs-api/auth
source_yaml: "generated: '2026-11-17'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://www.magicslides.app/docs-api/auth\nsources:\n- https://www.magicslides.app/docs-api/auth\n- https://www.magicslides.app/docs-api/auth.md\n- https://www.magicslides.app/docs-api/quick-start\n- https://www.magicslides.app/mcp\ndescription: Authentication methods for MagicSlides API\nschemes:\n- type: apiKey\n  name: apiKey\n  evidence: Include your API key in the request body using the `apiKey` parameter.\n  location: body\n  how_to_obtain: 'Log in to your MagicSlides dashboard, navigate to /dashboard/settings, generate a new API key and copy it (format: ms‑api‑{base64‑encoded‑payload}.{secret})'\n- type: apiKey\n  name: email_accessId\n  evidence: Include both `email` and `accessId` in the request body.\n  location: body\n  how_to_obtain: Find your access ID in the MagicSlides dashboard under API Settings and use your account email\nnote: No OAuth2, http‑bearer, http‑basic,\
  \ jwt, hmac, mtls, or other schemes are documented.\ndocs: https://www.magicslides.app/docs-api/auth\n"
source_yaml_url: https://artifacts.apis.io/magicslides-app/authentication/magicslides-app-authentication.yml
summary_line: 2 schemes
tags:
- Artificial Intelligence
- Presentation
- Automation
- Software-as-a-Service
- Productivity
---
