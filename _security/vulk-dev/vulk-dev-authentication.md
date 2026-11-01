---
anonymous_access: false
api_key_in: []
api_specs:
- filename: vulk-dev-models-api-openapi.yml
  format: yaml
  label: vulk-dev Models API
  slug: vulk-dev-models-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/vulk-dev/openapi/vulk-dev-models-api-openapi.yml
- filename: vulk-dev-operations-api-openapi.yml
  format: yaml
  label: vulk-dev Operations API
  slug: vulk-dev-operations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/vulk-dev/openapi/vulk-dev-operations-api-openapi.yml
- filename: vulk-dev-pay-as-you-go-previous-vulk-api-openapi.yml
  format: yaml
  label: vulk-dev Pay-as-you-go (previous VULK) API
  slug: vulk-dev-pay-as-you-go-previous-vulk-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/vulk-dev/openapi/vulk-dev-pay-as-you-go-previous-vulk-api-openapi.yml
- filename: vulk-dev-projects-api-openapi.yml
  format: yaml
  label: vulk-dev Projects API
  slug: vulk-dev-projects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/vulk-dev/openapi/vulk-dev-projects-api-openapi.yml
- filename: vulk-dev-usage-api-openapi.yml
  format: yaml
  label: vulk-dev Usage API
  slug: vulk-dev-usage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/vulk-dev/openapi/vulk-dev-usage-api-openapi.yml
auth_types: []
description: VULK API authentication uses an API key sent as a Bearer token in the Authorization header.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Vulk Dev Authentication
name_suffix: Authentication
oauth_flows: []
overview: vulk-dev declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: vulk-dev
provider_slug: vulk-dev
scheme_count: 1
schemes:
- evidence: 'Missing API key. Send it as "Authorization: Bearer vk_sk_…". Keys are created in Settings › API keys.'
  header: Authorization
  how_to_obtain: Create a key in Settings › API keys.
  location: header
  name: API key
  type: http-bearer
slug: vulk-dev-authentication
source_filename: vulk-dev-authentication.yml
source_heading: Authentication Profile
source_url: https://support.vulk.dev/docs/account/byok
source_yaml: "generated: '2026-10-30'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://support.vulk.dev/docs/account/byok\nsources:\n- https://support.vulk.dev/docs/account/byok\n- https://support.vulk.dev/docs/api/api-keys\n- https://support.vulk.dev/docs/troubleshooting/api-auth-issues\n- https://support.vulk.dev/docs/creating-projects/backend-apps\ndescription: VULK API authentication uses an API key sent as a Bearer token in the Authorization header.\nschemes:\n- type: http-bearer\n  name: API key\n  evidence: 'Missing API key. Send it as \"Authorization: Bearer vk_sk_…\". Keys are created in Settings › API keys.'\n  location: header\n  header: Authorization\n  how_to_obtain: Create a key in Settings › API keys.\nnote: No OAuth2, apiKey, http-basic, jwt, hmac, mtls, or other schemes are documented.\ndocs: https://support.vulk.dev/docs/account/byok\n"
source_yaml_url: https://artifacts.apis.io/vulk-dev/authentication/vulk-dev-authentication.yml
summary_line: 1 scheme
tags:
- Company
- AI
- AppBuilder
- NoCode
- 3D
---
