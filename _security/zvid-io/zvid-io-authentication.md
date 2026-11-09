---
anonymous_access: false
api_key_in: []
api_specs:
- filename: zvid-io-api-keys-api-openapi.yml
  format: yaml
  label: zvid-io API Keys API
  slug: zvid-io-api-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/zvid-io/openapi/zvid-io-api-keys-api-openapi.yml
- filename: zvid-io-authoring-api-openapi.yml
  format: yaml
  label: zvid-io Authoring API
  slug: zvid-io-authoring-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/zvid-io/openapi/zvid-io-authoring-api-openapi.yml
- filename: zvid-io-bulk-render-api-openapi.yml
  format: yaml
  label: zvid-io Bulk Render API
  slug: zvid-io-bulk-render-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/zvid-io/openapi/zvid-io-bulk-render-api-openapi.yml
- filename: zvid-io-credits-api-openapi.yml
  format: yaml
  label: zvid-io Credits API
  slug: zvid-io-credits-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/zvid-io/openapi/zvid-io-credits-api-openapi.yml
- filename: zvid-io-library-api-openapi.yml
  format: yaml
  label: zvid-io Library API
  slug: zvid-io-library-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/zvid-io/openapi/zvid-io-library-api-openapi.yml
- filename: zvid-io-projects-api-openapi.yml
  format: yaml
  label: zvid-io Projects API
  slug: zvid-io-projects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/zvid-io/openapi/zvid-io-projects-api-openapi.yml
- filename: zvid-io-render-api-openapi.yml
  format: yaml
  label: zvid-io Render API
  slug: zvid-io-render-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/zvid-io/openapi/zvid-io-render-api-openapi.yml
- filename: zvid-io-stock-api-openapi.yml
  format: yaml
  label: zvid-io Stock API
  slug: zvid-io-stock-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/zvid-io/openapi/zvid-io-stock-api-openapi.yml
- filename: zvid-io-templates-api-openapi.yml
  format: yaml
  label: zvid-io Templates API
  slug: zvid-io-templates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/zvid-io/openapi/zvid-io-templates-api-openapi.yml
- filename: zvid-io-uploads-api-openapi.yml
  format: yaml
  label: zvid-io Uploads API
  slug: zvid-io-uploads-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/zvid-io/openapi/zvid-io-uploads-api-openapi.yml
- filename: zvid-io-user-api-openapi.yml
  format: yaml
  label: zvid-io User API
  slug: zvid-io-user-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/zvid-io/openapi/zvid-io-user-api-openapi.yml
- filename: zvid-io-webhooks-api-openapi.yml
  format: yaml
  label: zvid-io Webhooks API
  slug: zvid-io-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/zvid-io/openapi/zvid-io-webhooks-api-openapi.yml
- filename: zvid-io-zvid-api-api-openapi.yml
  format: yaml
  label: zvid-io Zvid API
  slug: zvid-io-zvid-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/zvid-io/openapi/zvid-io-zvid-api-api-openapi.yml
auth_types: []
description: Authentication methods for Zvid API endpoints
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Zvid Io Authentication
name_suffix: Authentication
oauth_flows: []
overview: zvid-io declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: zvid-io
provider_slug: zvid-io
scheme_count: 2
schemes:
- evidence: 'Option 1: x-api-key: YOUR_API_KEY (header). API key for authentication. Create one in your dashboard.'
  header: x-api-key
  how_to_obtain: Create an API key in the Zvid dashboard at app.zvid.io/api-keys and keep the credential on your server.
  location: header
  name: x-api-key
  type: apiKey
- evidence: 'Option 2: Authorization: Bearer YOUR_ACCESS_TOKEN . Dashboard JWT in Authorization: Bearer <token>, only on operations that explicitly list this scheme.'
  header: Authorization
  how_to_obtain: Obtain a JWT access token from the Zvid dashboard (Dashboard JWT) for use in the Authorization header.
  location: header
  name: Bearer
  type: http-bearer
slug: zvid-io-authentication
source_filename: zvid-io-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.zvid.io/docs/endpoints/list-api-keys/
source_yaml: "generated: '2026-10-31'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.zvid.io/docs/endpoints/list-api-keys/\nsources:\n- https://docs.zvid.io/docs/endpoints/list-api-keys/\n- https://docs.zvid.io/docs/endpoints/create-api-key/\n- https://docs.zvid.io/docs/endpoints/update-api-key/\n- https://docs.zvid.io/docs/endpoints/revoke-api-key/\ndescription: Authentication methods for Zvid API endpoints\nschemes:\n- type: apiKey\n  name: x-api-key\n  evidence: 'Option 1: x-api-key: YOUR_API_KEY (header). API key for authentication. Create one in your dashboard.'\n  location: header\n  header: x-api-key\n  how_to_obtain: Create an API key in the Zvid dashboard at app.zvid.io/api-keys and keep the credential on your server.\n- type: http-bearer\n  name: Bearer\n  evidence: 'Option 2: Authorization: Bearer YOUR_ACCESS_TOKEN . Dashboard JWT in Authorization: Bearer <token>, only on operations that explicitly\n    list this scheme.'\n  location: header\n\
  \  header: Authorization\n  how_to_obtain: Obtain a JWT access token from the Zvid dashboard (Dashboard JWT) for use in the Authorization header.\nnote: OAuth flows are mentioned only as a separate connection (https://mcp.zvid.io/mcp) but no token or authorize URLs, scopes, or flow details\n  are provided on these pages.\ndocs: https://docs.zvid.io/docs/endpoints/list-api-keys/\n"
source_yaml_url: https://artifacts.apis.io/zvid-io/authentication/zvid-io-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Video
- Automation
- Media
---
