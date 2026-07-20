---
api_key_in:
- header
api_specs:
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
method: searched
name: Iru Authentication
name_suffix: Authentication
oauth_flows: []
overview: Iru secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Iru
provider_slug: iru
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
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/iru/refs/heads/main/authentication/iru-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Device Management
- Apple MDM
- Endpoint Security
- Identity and Access Management
- Compliance
- Vulnerability Management
- IT Management
- Security
---
