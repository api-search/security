---
anonymous_access: false
api_key_in: []
api_specs:
- filename: genko-me-contents-api-openapi.yml
  format: yaml
  label: genko.me Contents API
  slug: genko-me-contents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/genko-me/openapi/genko-me-contents-api-openapi.yml
- filename: genko-me-schema-api-openapi.yml
  format: yaml
  label: genko.me Schema API
  slug: genko-me-schema-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/genko-me/openapi/genko-me-schema-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: genko.me Authentication
name_suffix: Authentication
oauth_flows: []
overview: genko.me declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: genko.me
provider_slug: genko-me
scheme_count: 1
schemes:
- evidence: APIへ直接接続するときは、`X-API-KEY`ヘッダーに付けます。
  header: X-API-KEY
  how_to_obtain: Generated in workspace settings (APIキーページ)
  location: header
  name: API Key
  type: apiKey
slug: genko-me-authentication
source_filename: genko-me-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.genko.me/studio/api-keys.md
source_yaml: "generated: '2026-11-09'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.genko.me/studio/api-keys.md\nsources:\n- https://docs.genko.me/studio/api-keys.md\n- https://docs.genko.me/getting-started.md\n- https://docs.genko.me/frameworks/next/getting-started.md\n- https://docs.genko.me/frameworks/react/getting-started.md\nschemes:\n- type: apiKey\n  name: API Key\n  evidence: APIへ直接接続するときは、`X-API-KEY`ヘッダーに付けます。\n  location: header\n  header: X-API-KEY\n  how_to_obtain: Generated in workspace settings (APIキーページ)\ndocs: https://docs.genko.me/studio/api-keys.md\n"
source_yaml_url: https://artifacts.apis.io/genko-me/authentication/genko-me-authentication.yml
summary_line: 1 scheme
tags:
- Headless CMS
- Content Management
- Japanese
- Software-as-a-Service
---
