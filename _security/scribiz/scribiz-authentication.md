---
anonymous_access: false
api_key_in: []
api_specs:
- filename: scribiz-account-api-openapi.yml
  format: yaml
  label: Scribiz Account API
  slug: scribiz-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/scribiz/openapi/scribiz-account-api-openapi.yml
- filename: scribiz-auth-api-openapi.yml
  format: yaml
  label: Scribiz Auth API
  slug: scribiz-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/scribiz/openapi/scribiz-auth-api-openapi.yml
- filename: scribiz-billing-api-openapi.yml
  format: yaml
  label: Scribiz Billing API
  slug: scribiz-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/scribiz/openapi/scribiz-billing-api-openapi.yml
- filename: scribiz-gemini-proxy-api-openapi.yml
  format: yaml
  label: Scribiz Gemini proxy API
  slug: scribiz-gemini-proxy-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/scribiz/openapi/scribiz-gemini-proxy-api-openapi.yml
- filename: scribiz-jobs-api-openapi.yml
  format: yaml
  label: Scribiz Jobs API
  slug: scribiz-jobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/scribiz/openapi/scribiz-jobs-api-openapi.yml
- filename: scribiz-mcp-api-openapi.yml
  format: yaml
  label: Scribiz MCP API
  slug: scribiz-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/scribiz/openapi/scribiz-mcp-api-openapi.yml
- filename: scribiz-service-api-openapi.yml
  format: yaml
  label: Scribiz Service API
  slug: scribiz-service-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/scribiz/openapi/scribiz-service-api-openapi.yml
- filename: scribiz-uploads-api-openapi.yml
  format: yaml
  label: Scribiz Uploads API
  slug: scribiz-uploads-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/scribiz/openapi/scribiz-uploads-api-openapi.yml
- filename: scribiz-youtube-captions-api-openapi.yml
  format: yaml
  label: Scribiz YouTube captions API
  slug: scribiz-youtube-captions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/scribiz/openapi/scribiz-youtube-captions-api-openapi.yml
auth_types: []
description: Scribiz API authentication uses API keys sent either as a Bearer token in the Authorization header or in an X-API-Key header.
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Scribiz Authentication
name_suffix: Authentication
oauth_flows: []
overview: Scribiz declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Scribiz
provider_slug: scribiz
scheme_count: 2
schemes:
- evidence: 'Send a key as a bearer token, or in an `X-API-Key` header:'
  header: Authorization
  how_to_obtain: Create a key in the dashboard under API keys after signing in with an email link.
  location: header
  name: Authorization
  type: http-bearer
- evidence: You can send the key in an `X-API-Key` header instead.
  header: X-API-Key
  how_to_obtain: Create a key in the dashboard under API keys after signing in with an email link.
  location: header
  name: X-API-Key
  type: apiKey
slug: scribiz-authentication
source_filename: scribiz-authentication.yml
source_heading: Authentication Profile
source_url: https://scribiz.com/auth.md
source_yaml: "generated: '2026-11-08'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://scribiz.com/auth.md\nsources:\n- https://scribiz.com/auth.md\n- https://scribiz.com/docs/authentication.md\n- https://scribiz.com/docs/api/authentication.md\n- https://scribiz.com/docs/authentication\ndescription: Scribiz API authentication uses API keys sent either as a Bearer token in the Authorization header or in an X-API-Key header.\nschemes:\n- type: http-bearer\n  name: Authorization\n  evidence: 'Send a key as a bearer token, or in an `X-API-Key` header:'\n  location: header\n  header: Authorization\n  how_to_obtain: Create a key in the dashboard under API keys after signing in with an email link.\n- type: apiKey\n  name: X-API-Key\n  evidence: You can send the key in an `X-API-Key` header instead.\n  location: header\n  header: X-API-Key\n  how_to_obtain: Create a key in the dashboard under API keys after signing in with an email link.\nnote: No OAuth2 flows are\
  \ described for Scribiz.\ndocs: https://scribiz.com/auth.md\n"
source_yaml_url: https://artifacts.apis.io/scribiz/authentication/scribiz-authentication.yml
summary_line: 2 schemes
tags:
- Transcript
- Video
- Audio
- Subtitle
- Summarizer
- OCR
- Mac App
---
