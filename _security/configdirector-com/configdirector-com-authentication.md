---
anonymous_access: false
api_key_in: []
api_specs:
- filename: configdirector-com-api-tokens-api-openapi.yml
  format: yaml
  label: ConfigDirector API tokens API
  slug: configdirector-com-api-tokens-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/configdirector-com/openapi/configdirector-com-api-tokens-api-openapi.yml
- filename: configdirector-com-configs-api-openapi.yml
  format: yaml
  label: ConfigDirector Configs API
  slug: configdirector-com-configs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/configdirector-com/openapi/configdirector-com-configs-api-openapi.yml
- filename: configdirector-com-discovery-api-openapi.yml
  format: yaml
  label: ConfigDirector Discovery API
  slug: configdirector-com-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/configdirector-com/openapi/configdirector-com-discovery-api-openapi.yml
- filename: configdirector-com-documentation-api-openapi.yml
  format: yaml
  label: ConfigDirector Documentation API
  slug: configdirector-com-documentation-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/configdirector-com/openapi/configdirector-com-documentation-api-openapi.yml
- filename: configdirector-com-environments-api-openapi.yml
  format: yaml
  label: ConfigDirector Environments API
  slug: configdirector-com-environments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/configdirector-com/openapi/configdirector-com-environments-api-openapi.yml
- filename: configdirector-com-projects-api-openapi.yml
  format: yaml
  label: ConfigDirector Projects API
  slug: configdirector-com-projects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/configdirector-com/openapi/configdirector-com-projects-api-openapi.yml
- filename: configdirector-com-scanned-repositories-api-openapi.yml
  format: yaml
  label: ConfigDirector Scanned repositories API
  slug: configdirector-com-scanned-repositories-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/configdirector-com/openapi/configdirector-com-scanned-repositories-api-openapi.yml
- filename: configdirector-com-segments-api-openapi.yml
  format: yaml
  label: ConfigDirector Segments API
  slug: configdirector-com-segments-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/configdirector-com/openapi/configdirector-com-segments-api-openapi.yml
- filename: configdirector-com-tags-api-openapi.yml
  format: yaml
  label: ConfigDirector Tags API
  slug: configdirector-com-tags-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/configdirector-com/openapi/configdirector-com-tags-api-openapi.yml
- filename: configdirector-com-webhooks-api-openapi.yml
  format: yaml
  label: ConfigDirector Webhooks API
  slug: configdirector-com-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/configdirector-com/openapi/configdirector-com-webhooks-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: ConfigDirector Authentication
name_suffix: Authentication
oauth_flows: []
overview: ConfigDirector secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: ConfigDirector
provider_slug: configdirector-com
scheme_count: 1
schemes:
- description: API token created in the dashboard under API tokens. A token belongs to the member who created it, carries a chosen subset of permissions and never more than its creator's role grants; it can have an expiration date, and expired tokens are deleted 7 days after they expire.
  failure: '403 with {"error": ..., "code": ...}; codes API_TOKEN_NOT_FOUND, API_TOKEN_EXPIRED, API_TOKEN_OWNER_REMOVED'
  header: 'Authorization: Bearer YOUR-API-TOKEN'
  introspection: GET /api-token (getApiToken) describes the calling token, its organization and permissions
  name: bearerAuth
  permissions_doc: https://docs.configdirector.com/integrations/admin-api#permissions
  scheme: bearer
  sources:
  - openapi/configdirector-com-openapi.yml
  - https://docs.configdirector.com/raw/integrations/admin-api.md
  type: http
slug: configdirector-com-authentication
source_filename: configdirector-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://docs.configdirector.com/raw/integrations/admin-api.md\ndocs: https://docs.configdirector.com/integrations/admin-api#authentication\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  header: 'Authorization: Bearer YOUR-API-TOKEN'\n  description: API token created in the dashboard under API tokens. A token belongs to the member who created it,\n    carries a chosen subset of permissions and never more than its creator's role grants; it can have an expiration\n    date, and expired tokens are deleted 7 days after they expire.\n  permissions_doc: https://docs.configdirector.com/integrations/admin-api#permissions\n  failure: '403 with {\"error\": ..., \"code\": ...}; codes API_TOKEN_NOT_FOUND, API_TOKEN_EXPIRED, API_TOKEN_OWNER_REMOVED'\n  introspection: GET /api-token (getApiToken) describes the calling token, its organization and permissions\n  sources:\n  - openapi/configdirector-com-openapi.yml\n\
  \  - https://docs.configdirector.com/raw/integrations/admin-api.md\nnotes: Token permissions (projects:read, configs:archive, webhooks:manage ...) are API-token permissions, not OAuth\n  scopes; no OAuth flow is documented for the Admin API. SDKs authenticate with client/server SDK keys per environment\n  (5 of each per environment).\n"
source_yaml_url: https://artifacts.apis.io/configdirector-com/authentication/configdirector-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Feature Flags
- Remote Configuration
- Configuration Management
- Developer Tools
- OpenFeature
- SDK
- MCP
---
