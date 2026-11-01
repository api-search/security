---
anonymous_access: false
api_key_in: []
api_specs:
- filename: makespdf-com-artifacts-api-openapi.yml
  format: yaml
  label: makespdf-com Artifacts API
  slug: makespdf-com-artifacts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/makespdf-com/openapi/makespdf-com-artifacts-api-openapi.yml
- filename: makespdf-com-public-api-openapi.yml
  format: yaml
  label: makespdf-com Public API
  slug: makespdf-com-public-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/makespdf-com/openapi/makespdf-com-public-api-openapi.yml
- filename: makespdf-com-render-api-openapi.yml
  format: yaml
  label: makespdf-com Render API
  slug: makespdf-com-render-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/makespdf-com/openapi/makespdf-com-render-api-openapi.yml
- filename: makespdf-com-validate-api-openapi.yml
  format: yaml
  label: makespdf-com Validate API
  slug: makespdf-com-validate-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/makespdf-com/openapi/makespdf-com-validate-api-openapi.yml
- filename: makespdf-com-x402-api-openapi.yml
  format: yaml
  label: makespdf-com X402 API
  slug: makespdf-com-x402-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/makespdf-com/openapi/makespdf-com-x402-api-openapi.yml
auth_types: []
description: Authentication for makesPDF API
kind: authentication
layout: security
mechanism_count: 3
method: searched
name: Makespdf Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: makespdf-com declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: makespdf-com
provider_slug: makespdf-com
scheme_count: 3
schemes:
- evidence: 'Pass it as a Bearer token in the Authorization header:'
  header: Authorization
  how_to_obtain: Create an API key in Settings → API Keys and copy the generated key.
  location: header
  name: API Key
  type: http-bearer
- evidence: set MAKESPDF_DEV_TOKEN in apps/web/.dev.vars and send it as a Bearer token.
  header: Authorization
  how_to_obtain: Generate a token with `openssl rand -hex 32` and set the MAKESPDF_DEV_TOKEN environment variable.
  location: header
  name: Development Token
  type: http-bearer
- evidence: 'On approval: { "access_token": "mpdf_...", "token_type": "Bearer" }'
  flows:
  - device_code
  header: Authorization
  how_to_obtain: Request a device code via POST https://makespdf.com/api/v1/device/code, have the user approve, then poll POST https://makespdf.com/api/v1/device/token to receive an access token.
  location: header
  name: Device Authorization Flow Token
  type: http-bearer
slug: makespdf-com-authentication
source_filename: makespdf-com-authentication.yml
source_heading: Authentication Profile
source_url: https://makespdf.com/docs/getting-started
source_yaml: "generated: '2026-10-31'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://makespdf.com/docs/getting-started\nsources:\n- https://makespdf.com/docs/getting-started\n- https://makespdf.com/docs/getting-started.md\n- https://makespdf.com/docs/ai-setup\n- https://makespdf.com/docs/ai-setup.md\ndescription: Authentication for makesPDF API\nschemes:\n- type: http-bearer\n  name: API Key\n  evidence: 'Pass it as a Bearer token in the Authorization header:'\n  location: header\n  header: Authorization\n  how_to_obtain: Create an API key in Settings → API Keys and copy the generated key.\n- type: http-bearer\n  name: Development Token\n  evidence: set MAKESPDF_DEV_TOKEN in apps/web/.dev.vars and send it as a Bearer token.\n  location: header\n  header: Authorization\n  how_to_obtain: Generate a token with `openssl rand -hex 32` and set the MAKESPDF_DEV_TOKEN environment variable.\n- type: http-bearer\n  name: Device Authorization Flow Token\n  evidence:\
  \ 'On approval: { \"access_token\": \"mpdf_...\", \"token_type\": \"Bearer\" }'\n  location: header\n  header: Authorization\n  flows:\n  - device_code\n  how_to_obtain: Request a device code via POST https://makespdf.com/api/v1/device/code, have the user approve, then poll POST https://makespdf.com/api/v1/device/token\n    to receive an access token.\ndocs: https://makespdf.com/docs/getting-started\n"
source_yaml_url: https://artifacts.apis.io/makespdf-com/authentication/makespdf-com-authentication.yml
summary_line: 3 schemes
tags:
- Company
- PDF
- API
- Conversion
- Developer
---
