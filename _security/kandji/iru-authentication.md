---
anonymous_access: false
api_key_in:
- header
api_specs:
- filename: kandji-audit-api-openapi.yml
  format: yaml
  label: Iru Audit API
  slug: kandji-audit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kandji/refs/heads/main/openapi/kandji-audit-api-openapi.yml
- filename: kandji-behavioral-detections-api-openapi.yml
  format: yaml
  label: Iru Behavioral Detections API
  slug: kandji-behavioral-detections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kandji/refs/heads/main/openapi/kandji-behavioral-detections-api-openapi.yml
- filename: kandji-blueprints-api-openapi.yml
  format: yaml
  label: Iru Blueprints API
  slug: kandji-blueprints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kandji/refs/heads/main/openapi/kandji-blueprints-api-openapi.yml
- filename: kandji-devices-api-openapi.yml
  format: yaml
  label: Iru Devices API
  slug: kandji-devices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kandji/refs/heads/main/openapi/kandji-devices-api-openapi.yml
- filename: kandji-integrations-api-openapi.yml
  format: yaml
  label: Iru Integrations API
  slug: kandji-integrations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kandji/refs/heads/main/openapi/kandji-integrations-api-openapi.yml
- filename: kandji-library-api-openapi.yml
  format: yaml
  label: Iru Library API
  slug: kandji-library-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kandji/refs/heads/main/openapi/kandji-library-api-openapi.yml
- filename: kandji-prism-api-openapi.yml
  format: yaml
  label: Iru Prism API
  slug: kandji-prism-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kandji/refs/heads/main/openapi/kandji-prism-api-openapi.yml
- filename: kandji-self-service-api-openapi.yml
  format: yaml
  label: Iru Self Service API
  slug: kandji-self-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kandji/refs/heads/main/openapi/kandji-self-service-api-openapi.yml
- filename: kandji-settings-api-openapi.yml
  format: yaml
  label: Iru Settings API
  slug: kandji-settings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kandji/refs/heads/main/openapi/kandji-settings-api-openapi.yml
- filename: kandji-tags-api-openapi.yml
  format: yaml
  label: Iru Tags API
  slug: kandji-tags-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kandji/refs/heads/main/openapi/kandji-tags-api-openapi.yml
- filename: kandji-threat-details-api-openapi.yml
  format: yaml
  label: Iru Threat Details API
  slug: kandji-threat-details-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kandji/refs/heads/main/openapi/kandji-threat-details-api-openapi.yml
- filename: kandji-upload-to-s3-api-openapi.yml
  format: yaml
  label: Iru Upload To S3 API
  slug: kandji-upload-to-s3-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kandji/refs/heads/main/openapi/kandji-upload-to-s3-api-openapi.yml
- filename: kandji-users-api-openapi.yml
  format: yaml
  label: Iru Users API
  slug: kandji-users-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kandji/refs/heads/main/openapi/kandji-users-api-openapi.yml
- filename: kandji-vulnerability-management-api-openapi.yml
  format: yaml
  label: Iru Vulnerability Management API
  slug: kandji-vulnerability-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kandji/refs/heads/main/openapi/kandji-vulnerability-management-api-openapi.yml
- filename: how-to-set-up-the-iru-endpoint-api-in-postman.md
  format: yaml
  label: Iru Endpoint Management API
  slug: iru-endpoint-management-api
  spec_type: Postman
  url: https://docs.iru.com/en/endpoint/api/how-to-set-up-the-iru-endpoint-api-in-postman.md
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Iru Authentication
name_suffix: Authentication
oauth_flows: []
overview: Iru secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Iru
provider_slug: kandji
scheme_count: 1
schemes:
- description: Iru Endpoint uses tenant-level bearer tokens to control access to the API. Tokens are created in the Access area (Account Menu > Access > API tokens tab). Each token has a Name and Description and is shown exactly once at creation ("You will not be able to see the token or the MCP configuration again"). Tokens can optionally be MCP-enabled for use with MCP clients.
  format: Bearer <token>
  header: Authorization
  in: header
  name: bearerAuth
  scheme: bearer
  sources:
  - https://docs.iru.com/en/endpoint/api/iru-api-overview.md
  type: http
slug: iru-authentication
source_filename: iru-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: searched\nsource: https://docs.iru.com/en/endpoint/api/iru-api-overview.md\ndocs: https://support.kandji.io/kb/kandji-api\nsummary:\n  types: [http]\n  scheme: bearer\n  api_key_in: [header]\n  oauth2_flows: []\nschemes:\n  - name: bearerAuth\n    type: http\n    scheme: bearer\n    in: header\n    header: Authorization\n    format: \"Bearer <token>\"\n    description: >-\n      Iru Endpoint uses tenant-level bearer tokens to control access to the API.\n      Tokens are created in the Access area (Account Menu > Access > API tokens\n      tab). Each token has a Name and Description and is shown exactly once at\n      creation (\"You will not be able to see the token or the MCP configuration\n      again\"). Tokens can optionally be MCP-enabled for use with MCP clients.\n    sources:\n      - https://docs.iru.com/en/endpoint/api/iru-api-overview.md\npermissions:\n  model: per-token scoped permissions (not OAuth scopes)\n  description: >-\n  \
  \  Each API token carries a configurable set of permissions, grouped into\n    sections (for example \"Blueprints Management\"). Checking or unchecking a\n    section header toggles every permission in that section. Permissions are\n    edited on the token detail view (Configure / Edit) after creation and can be\n    revoked at any time. This is a permission-grant model over a bearer token,\n    not an OAuth2 scope surface, so no scopes/ artifact is emitted.\ntoken_host:\n  form: <subdomain>.api.kandji.io\n  example: accuhive.api.kandji.io\n  note: >-\n    The tenant-specific API URL is displayed on the API tokens page after the\n    first token is created.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kandji/refs/heads/main/authentication/iru-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Device Management
- Mobile Device Management
- apple-management
- Endpoint Security
- endpoint-detection-response
- Vulnerability Management
- Compliance Automation
- Workforce Identity
- IT Operations
- MCP
- agent-native
---
