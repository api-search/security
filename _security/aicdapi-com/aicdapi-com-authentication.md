---
anonymous_access: false
api_key_in: []
api_specs:
- filename: aicdapi-com-agenda-hits-api-openapi.yml
  format: yaml
  label: aicdapi-com Agenda hits API
  slug: aicdapi-com-agenda-hits-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aicdapi-com/openapi/aicdapi-com-agenda-hits-api-openapi.yml
- filename: aicdapi-com-customer-civic-data-api-openapi.yml
  format: yaml
  label: aicdapi-com Customer civic data API
  slug: aicdapi-com-customer-civic-data-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aicdapi-com/openapi/aicdapi-com-customer-civic-data-api-openapi.yml
- filename: aicdapi-com-data-reports-api-openapi.yml
  format: yaml
  label: aicdapi-com Data reports API
  slug: aicdapi-com-data-reports-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aicdapi-com/openapi/aicdapi-com-data-reports-api-openapi.yml
- filename: aicdapi-com-mcp-api-openapi.yml
  format: yaml
  label: aicdapi-com MCP API
  slug: aicdapi-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aicdapi-com/openapi/aicdapi-com-mcp-api-openapi.yml
- filename: aicdapi-com-public-api-specification-api-openapi.yml
  format: yaml
  label: aicdapi-com Public API specification API
  slug: aicdapi-com-public-api-specification-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aicdapi-com/openapi/aicdapi-com-public-api-specification-api-openapi.yml
- filename: aicdapi-com-research-coverage-api-openapi.yml
  format: yaml
  label: aicdapi-com Research coverage API
  slug: aicdapi-com-research-coverage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aicdapi-com/openapi/aicdapi-com-research-coverage-api-openapi.yml
- filename: aicdapi-com-sources-api-openapi.yml
  format: yaml
  label: aicdapi-com Sources API
  slug: aicdapi-com-sources-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/aicdapi-com/openapi/aicdapi-com-sources-api-openapi.yml
auth_types: []
description: Authentication schemes for AICD API
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Aicdapi Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: aicdapi-com declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: aicdapi-com
provider_slug: aicdapi-com
scheme_count: 1
schemes:
- evidence: 'Authentication: Authorization bearer header from AICD_API_KEY.'
  header: Authorization
  how_to_obtain: Create an API key in the account UI; the key is used as a bearer token.
  location: header
  name: Bearer
  type: http-bearer
slug: aicdapi-com-authentication
source_filename: aicdapi-com-authentication.yml
source_heading: Authentication Profile
source_url: https://aicdapi.com/help/api-keys.md
source_yaml: "generated: '2026-10-30'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://aicdapi.com/help/api-keys.md\nsources:\n- https://aicdapi.com/help/api-keys.md\n- https://aicdapi.com/help/api-keys/llms.txt\n- https://aicdapi.com/help/getting-started.md\n- https://aicdapi.com/help/mcp-setup.md\ndescription: Authentication schemes for AICD API\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: 'Authentication: Authorization bearer header from AICD_API_KEY.'\n  location: header\n  header: Authorization\n  how_to_obtain: Create an API key in the account UI; the key is used as a bearer token.\ndocs: https://aicdapi.com/help/api-keys.md\n"
source_yaml_url: https://artifacts.apis.io/aicdapi-com/authentication/aicdapi-com-authentication.yml
summary_line: 1 scheme
tags:
- Company
- CivicData
- Government
- API
- MCP
---
