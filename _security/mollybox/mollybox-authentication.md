---
api_key_in: []
api_specs:
- filename: mollybox-arcflow-openapi.json
  format: json
  label: Arcflow API
  slug: arcflow-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mollybox/refs/heads/main/openapi/mollybox-arcflow-openapi.json
auth_types:
- http
description: ''
kind: authentication
layout: security
method: derived
name: Mollybox Authentication
name_suffix: Authentication
oauth_flows: []
overview: MollyBox secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: MollyBox
provider_slug: mollybox
scheme_count: 1
schemes:
- applied_to:
  - get_identity_api_me_get
  - capture_resource_api_resources_post
  - list_resources_api_resources_get
  - import_resources_api_admin_import_resources_post
  - get_resource_api_resources__resource_id__get
  - update_resource_status_api_resources__resource_id__status_patch
  - open_resource_api_resources__resource_id__open_post
  name: HTTPBearer
  scheme: bearer
  sources:
  - openapi/mollybox-arcflow-openapi.json
  type: http
slug: mollybox-authentication
source_filename: mollybox-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-07-20'\nmethod: derived\nsource: openapi/mollybox-arcflow-openapi.json\nsummary:\n  types: [http]\n  http_schemes: [bearer]\n  api_key_in: []\n  oauth2_flows: []\n  notes: >-\n    All operations except GET /api/health require an HTTP Bearer token.\n    The server self-describes as a single-user, self-hosted deployment\n    (HealthResponse.mode and ServerIdentity.mode default to \"single-user\"),\n    so the bearer token is a server-level access token rather than a\n    per-user OAuth credential.\nschemes:\n  - name: HTTPBearer\n    type: http\n    scheme: bearer\n    applied_to:\n      - get_identity_api_me_get\n      - capture_resource_api_resources_post\n      - list_resources_api_resources_get\n      - import_resources_api_admin_import_resources_post\n      - get_resource_api_resources__resource_id__get\n      - update_resource_status_api_resources__resource_id__status_patch\n      - open_resource_api_resources__resource_id__open_post\n    sources: [openapi/mollybox-arcflow-openapi.json]\n\
  unauthenticated_operations:\n  - health_api_health_get\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mollybox/refs/heads/main/authentication/mollybox-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Consumer
- API
- Bookmarking
- Resource Capture
- Read It Later
- FastAPI
- Self-Hosted
---
