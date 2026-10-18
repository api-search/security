---
anonymous_access: false
api_key_in: []
api_specs:
- filename: sprite-ai-cancel-api-openapi.yml
  format: yaml
  label: Sprite AI Cancel API
  slug: sprite-ai-cancel-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sprite-ai/refs/heads/main/openapi/sprite-ai-cancel-api-openapi.yml
- filename: sprite-ai-palettes-api-openapi.yml
  format: yaml
  label: Sprite AI Palettes API
  slug: sprite-ai-palettes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sprite-ai/refs/heads/main/openapi/sprite-ai-palettes-api-openapi.yml
- filename: sprite-ai-sprite-ai-api-api-openapi.yml
  format: yaml
  label: Sprite AI Sprite AI API
  slug: sprite-ai-sprite-ai-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sprite-ai/refs/heads/main/openapi/sprite-ai-sprite-ai-api-api-openapi.yml
- filename: sprite-ai-sprites-api-openapi.yml
  format: yaml
  label: Sprite AI Sprites API
  slug: sprite-ai-sprites-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sprite-ai/refs/heads/main/openapi/sprite-ai-sprites-api-openapi.yml
auth_types: []
description: Authentication schemes for Sprite AI API
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Sprite Ai Authentication
name_suffix: Authentication
oauth_flows: []
overview: Sprite AI declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Sprite AI
provider_slug: sprite-ai
scheme_count: 1
schemes:
- evidence: Authenticate every Sprite AI API request with a Bearer token.
  header: Authorization
  how_to_obtain: Create, name, and revoke keys on the API keys page.
  location: header
  name: Bearer
  type: http-bearer
slug: sprite-ai-authentication
source_filename: sprite-ai-authentication.yml
source_heading: Authentication Profile
source_url: https://www.sprite-ai.art/docs/authentication
source_yaml: "generated: '2026-10-11'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://www.sprite-ai.art/docs/authentication\nsources:\n- https://www.sprite-ai.art/docs/authentication\n- https://www.sprite-ai.art/guides/gamemaker-sprites\n- https://www.sprite-ai.art/guides/godot-sprites\ndescription: Authentication schemes for Sprite AI API\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: Authenticate every Sprite AI API request with a Bearer token.\n  location: header\n  header: Authorization\n  how_to_obtain: Create, name, and revoke keys on the API keys page.\nnote: No OAuth2, apiKey, http-basic, jwt, hmac, mtls, or other schemes are documented on the provided pages.\ndocs: https://www.sprite-ai.art/docs/authentication\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sprite-ai/refs/heads/main/authentication/sprite-ai-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Artificial Intelligence
- Gaming
- Graphics
- REST API
---
