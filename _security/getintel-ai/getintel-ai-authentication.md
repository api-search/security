---
anonymous_access: false
api_key_in: []
api_specs:
- filename: getintel-ai-api-openapi-generated.yml
  format: yaml
  label: GetIntel api API
  slug: api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getintel-ai/openapi/_ae-authored/getintel-ai-api-openapi-generated.yml
- filename: getintel-ai-core-openapi-generated.yml
  format: yaml
  label: GetIntel core API
  slug: core-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getintel-ai/openapi/_ae-authored/getintel-ai-core-openapi-generated.yml
- filename: getintel-ai-v1-openapi-generated.yml
  format: yaml
  label: GetIntel v1 API
  slug: v1-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getintel-ai/openapi/_ae-authored/getintel-ai-v1-openapi-generated.yml
auth_types: []
description: GetIntel API authentication uses API keys sent as Bearer tokens in the Authorization header.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: GetIntel Authentication
name_suffix: Authentication
oauth_flows: []
overview: GetIntel declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: GetIntel
provider_slug: getintel-ai
scheme_count: 1
schemes:
- evidence: Create a GetIntel API key, send it as a Bearer token, choose the brand with brand_id, and revoke keys you no longer use.
  header: Authorization
  how_to_obtain: Create keys in Integrations → Developers → GetIntel API; the full key is shown once when created.
  location: header
  name: Bearer
  type: http-bearer
slug: getintel-ai-authentication
source_filename: getintel-ai-authentication.yml
source_heading: Authentication Profile
source_url: https://getintel.ai/docs/api/authentication/
source_yaml: "generated: '2026-11-10'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://getintel.ai/docs/api/authentication/\nsources:\n- https://getintel.ai/docs/api/authentication/\n- https://getintel.ai/docs/api/authentication.md\n- https://getintel.ai/docs/mcp/tokens-and-permissions/\n- https://getintel.ai/docs/getting-started/quickstart/\ndescription: GetIntel API authentication uses API keys sent as Bearer tokens in the Authorization header.\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: Create a GetIntel API key, send it as a Bearer token, choose the brand with brand_id, and revoke keys you no longer use.\n  location: header\n  header: Authorization\n  how_to_obtain: Create keys in Integrations → Developers → GetIntel API; the full key is shown once when created.\ndocs: https://getintel.ai/docs/api/authentication/\n"
source_yaml_url: https://artifacts.apis.io/getintel-ai/authentication/getintel-ai-authentication.yml
summary_line: 1 scheme
tags:
- Artificial Intelligence
- Visibility
- Marketing
- Analytics
- Software-as-a-Service
---
