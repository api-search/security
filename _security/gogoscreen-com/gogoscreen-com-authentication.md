---
anonymous_access: false
api_key_in: []
api_specs:
- filename: gogoscreen-com-account-api-openapi.yml
  format: yaml
  label: GogoScreen Account API
  slug: gogoscreen-com-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gogoscreen-com/openapi/gogoscreen-com-account-api-openapi.yml
- filename: gogoscreen-com-assistant-api-openapi.yml
  format: yaml
  label: GogoScreen Assistant API
  slug: gogoscreen-com-assistant-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gogoscreen-com/openapi/gogoscreen-com-assistant-api-openapi.yml
- filename: gogoscreen-com-catalog-api-openapi.yml
  format: yaml
  label: GogoScreen Catalog API
  slug: gogoscreen-com-catalog-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gogoscreen-com/openapi/gogoscreen-com-catalog-api-openapi.yml
- filename: gogoscreen-com-keys-api-openapi.yml
  format: yaml
  label: GogoScreen Keys API
  slug: gogoscreen-com-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gogoscreen-com/openapi/gogoscreen-com-keys-api-openapi.yml
- filename: gogoscreen-com-marketing-api-openapi.yml
  format: yaml
  label: GogoScreen Marketing API
  slug: gogoscreen-com-marketing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gogoscreen-com/openapi/gogoscreen-com-marketing-api-openapi.yml
- filename: gogoscreen-com-renders-api-openapi.yml
  format: yaml
  label: GogoScreen Renders API
  slug: gogoscreen-com-renders-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gogoscreen-com/openapi/gogoscreen-com-renders-api-openapi.yml
- filename: gogoscreen-com-storyboards-api-openapi.yml
  format: yaml
  label: GogoScreen Storyboards API
  slug: gogoscreen-com-storyboards-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gogoscreen-com/openapi/gogoscreen-com-storyboards-api-openapi.yml
- filename: gogoscreen-com-templates-api-openapi.yml
  format: yaml
  label: GogoScreen Templates API
  slug: gogoscreen-com-templates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gogoscreen-com/openapi/gogoscreen-com-templates-api-openapi.yml
- filename: gogoscreen-com-usage-api-openapi.yml
  format: yaml
  label: GogoScreen Usage API
  slug: gogoscreen-com-usage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gogoscreen-com/openapi/gogoscreen-com-usage-api-openapi.yml
- filename: gogoscreen-com-voices-api-openapi.yml
  format: yaml
  label: GogoScreen Voices API
  slug: gogoscreen-com-voices-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gogoscreen-com/openapi/gogoscreen-com-voices-api-openapi.yml
- filename: gogoscreen-com-wallet-api-openapi.yml
  format: yaml
  label: GogoScreen Wallet API
  slug: gogoscreen-com-wallet-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gogoscreen-com/openapi/gogoscreen-com-wallet-api-openapi.yml
- filename: gogoscreen-com-webhooks-api-openapi.yml
  format: yaml
  label: GogoScreen Webhooks API
  slug: gogoscreen-com-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gogoscreen-com/openapi/gogoscreen-com-webhooks-api-openapi.yml
auth_types: []
description: Authentication
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: GogoScreen Authentication
name_suffix: Authentication
oauth_flows: []
overview: GogoScreen declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: GogoScreen
provider_slug: gogoscreen-com
scheme_count: 2
schemes:
- evidence: Every call to the public API carries one API key. The key acts for one account, spends that account's video time, and holds only the scopes it was issued with.
  header: Authorization
  how_to_obtain: Create a key in the developer console at app.gogoscreen.com/dashboard/developers; the key is shown once as a plaintext string prefixed with gsk_live_.
  location: header
  name: Authorization
  scopes:
  - account:read
  - catalog:read
  - marketing:export
  - marketing:read
  - marketing:write
  - renders:read
  - renders:write
  - storyboards:read
  - storyboards:write
  - usage:read
  - wallet:read
  - webhooks:manage
  type: http-bearer
- evidence: Every call to the public API carries one API key. The key acts for one account, spends that account's video time, and holds only the scopes it was issued with.
  header: X-API-Key
  how_to_obtain: Create a key in the developer console at app.gogoscreen.com/dashboard/developers; the key is shown once as a plaintext string prefixed with gsk_live_.
  location: header
  name: X-API-Key
  scopes:
  - account:read
  - catalog:read
  - marketing:export
  - marketing:read
  - marketing:write
  - renders:read
  - renders:write
  - storyboards:read
  - storyboards:write
  - usage:read
  - wallet:read
  - webhooks:manage
  type: apiKey
slug: gogoscreen-com-authentication
source_filename: gogoscreen-com-authentication.yml
source_heading: Authentication Profile
source_url: https://gogoscreen.com/docs/authentication
source_yaml: "generated: '2026-11-10'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://gogoscreen.com/docs/authentication\nsources:\n- https://gogoscreen.com/docs/authentication\n- https://gogoscreen.com/docs/api/keys\n- https://gogoscreen.com/docs/api/keys/create\n- https://gogoscreen.com/docs/api/keys/get\ndescription: Authentication\nschemes:\n- type: http-bearer\n  name: Authorization\n  evidence: Every call to the public API carries one API key. The key acts for one account, spends that account's video time, and holds only the\n    scopes it was issued with.\n  location: header\n  header: Authorization\n  scopes:\n  - account:read\n  - catalog:read\n  - marketing:export\n  - marketing:read\n  - marketing:write\n  - renders:read\n  - renders:write\n  - storyboards:read\n  - storyboards:write\n  - usage:read\n  - wallet:read\n  - webhooks:manage\n  how_to_obtain: Create a key in the developer console at app.gogoscreen.com/dashboard/developers; the key is\
  \ shown once as a plaintext string\n    prefixed with gsk_live_.\n- type: apiKey\n  name: X-API-Key\n  evidence: Every call to the public API carries one API key. The key acts for one account, spends that account's video time, and holds only the\n    scopes it was issued with.\n  location: header\n  header: X-API-Key\n  scopes:\n  - account:read\n  - catalog:read\n  - marketing:export\n  - marketing:read\n  - marketing:write\n  - renders:read\n  - renders:write\n  - storyboards:read\n  - storyboards:write\n  - usage:read\n  - wallet:read\n  - webhooks:manage\n  how_to_obtain: Create a key in the developer console at app.gogoscreen.com/dashboard/developers; the key is shown once as a plaintext string\n    prefixed with gsk_live_.\ndocs: https://gogoscreen.com/docs/authentication\n"
source_yaml_url: https://artifacts.apis.io/gogoscreen-com/authentication/gogoscreen-com-authentication.yml
summary_line: 2 schemes
tags:
- demo video
- Web App
- Developers
---
