---
anonymous_access: false
api_key_in: []
api_specs:
- filename: imagestep-dev-agent-api-openapi.yml
  format: yaml
  label: ImageStep Agent API
  slug: imagestep-dev-agent-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/imagestep-dev/openapi/imagestep-dev-agent-api-openapi.yml
- filename: imagestep-dev-ai-models-api-openapi.yml
  format: yaml
  label: ImageStep AI Models API
  slug: imagestep-dev-ai-models-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/imagestep-dev/openapi/imagestep-dev-ai-models-api-openapi.yml
- filename: imagestep-dev-api-key-management-api-openapi.yml
  format: yaml
  label: ImageStep API Key Management API
  slug: imagestep-dev-api-key-management-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/imagestep-dev/openapi/imagestep-dev-api-key-management-api-openapi.yml
- filename: imagestep-dev-asset-management-api-openapi.yml
  format: yaml
  label: ImageStep Asset Management API
  slug: imagestep-dev-asset-management-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/imagestep-dev/openapi/imagestep-dev-asset-management-api-openapi.yml
- filename: imagestep-dev-job-management-api-openapi.yml
  format: yaml
  label: ImageStep Job Management API
  slug: imagestep-dev-job-management-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/imagestep-dev/openapi/imagestep-dev-job-management-api-openapi.yml
- filename: imagestep-dev-ops-api-openapi.yml
  format: yaml
  label: ImageStep Ops API
  slug: imagestep-dev-ops-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/imagestep-dev/openapi/imagestep-dev-ops-api-openapi.yml
- filename: imagestep-dev-preset-management-api-openapi.yml
  format: yaml
  label: ImageStep Preset Management API
  slug: imagestep-dev-preset-management-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/imagestep-dev/openapi/imagestep-dev-preset-management-api-openapi.yml
- filename: imagestep-dev-synchronous-images-api-openapi.yml
  format: yaml
  label: ImageStep Synchronous images API
  slug: imagestep-dev-synchronous-images-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/imagestep-dev/openapi/imagestep-dev-synchronous-images-api-openapi.yml
- filename: imagestep-dev-template-management-api-openapi.yml
  format: yaml
  label: ImageStep Template Management API
  slug: imagestep-dev-template-management-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/imagestep-dev/openapi/imagestep-dev-template-management-api-openapi.yml
- filename: imagestep-dev-usage-api-openapi.yml
  format: yaml
  label: ImageStep Usage API
  slug: imagestep-dev-usage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/imagestep-dev/openapi/imagestep-dev-usage-api-openapi.yml
- filename: imagestep-dev-webhooks-api-openapi.yml
  format: yaml
  label: ImageStep Webhooks API
  slug: imagestep-dev-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/imagestep-dev/openapi/imagestep-dev-webhooks-api-openapi.yml
auth_types: []
description: ImageStep uses API keys for authentication.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: ImageStep Authentication
name_suffix: Authentication
oauth_flows: []
overview: ImageStep declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: ImageStep
provider_slug: imagestep-dev
scheme_count: 1
schemes:
- evidence: 'Send `Authorization: ApiKey <key>`'
  header: Authorization
  how_to_obtain: Create an API key in the console (Get a key).
  location: header
  name: Authorization
  type: apiKey
slug: imagestep-dev-authentication
source_filename: imagestep-dev-authentication.yml
source_heading: Authentication Profile
source_url: https://imagestep.dev/docs/api/api-keys
source_yaml: "generated: '2026-11-12'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://imagestep.dev/docs/api/api-keys\nsources:\n- https://imagestep.dev/docs/api/api-keys\n- https://api.imagestep.dev/v3/api-docs/api-key-accessible\n- https://imagestep.dev/docs/quickstart\ndescription: ImageStep uses API keys for authentication.\nschemes:\n- type: apiKey\n  name: Authorization\n  evidence: 'Send `Authorization: ApiKey <key>`'\n  location: header\n  header: Authorization\n  how_to_obtain: Create an API key in the console (Get a key).\nnote: No OAuth2 or other authentication methods are documented.\ndocs: https://imagestep.dev/docs/api/api-keys\n"
source_yaml_url: https://artifacts.apis.io/imagestep-dev/authentication/imagestep-dev-authentication.yml
summary_line: 1 scheme
tags:
- Automation
- AIOps
- Deterministic Ops
- SDK
- CLI
---
