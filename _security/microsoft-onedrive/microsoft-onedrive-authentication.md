---
anonymous_access: false
api_key_in: []
api_specs:
- filename: microsoft-onedrive-drives-drive-actions-api-openapi.yml
  format: yaml
  label: Microsoft OneDrive Drives.drive.Actions API
  slug: microsoft-onedrive-drives-drive-actions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-onedrive/openapi/microsoft-onedrive-drives-drive-actions-api-openapi.yml
- filename: microsoft-onedrive-drives-drive-api-openapi.yml
  format: yaml
  label: Microsoft OneDrive Drives.drive API
  slug: microsoft-onedrive-drives-drive-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-onedrive/openapi/microsoft-onedrive-drives-drive-api-openapi.yml
- filename: microsoft-onedrive-drives-drive-functions-api-openapi.yml
  format: yaml
  label: Microsoft OneDrive Drives.drive.Functions API
  slug: microsoft-onedrive-drives-drive-functions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-onedrive/openapi/microsoft-onedrive-drives-drive-functions-api-openapi.yml
- filename: microsoft-onedrive-drives-driveitem-api-openapi.yml
  format: yaml
  label: Microsoft OneDrive Drives.drive Item API
  slug: microsoft-onedrive-drives-driveitem-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-onedrive/openapi/microsoft-onedrive-drives-driveitem-api-openapi.yml
- filename: microsoft-onedrive-drives-list-api-openapi.yml
  format: yaml
  label: Microsoft OneDrive Drives.list API
  slug: microsoft-onedrive-drives-list-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-onedrive/openapi/microsoft-onedrive-drives-list-api-openapi.yml
- filename: microsoft-onedrive-drives-user-api-openapi.yml
  format: yaml
  label: Microsoft OneDrive Drives.user API
  slug: microsoft-onedrive-drives-user-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-onedrive/openapi/microsoft-onedrive-drives-user-api-openapi.yml
- filename: microsoft-onedrive-groups-drive-api-openapi.yml
  format: yaml
  label: Microsoft OneDrive Groups.drive API
  slug: microsoft-onedrive-groups-drive-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-onedrive/openapi/microsoft-onedrive-groups-drive-api-openapi.yml
- filename: microsoft-onedrive-groups-site-api-openapi.yml
  format: yaml
  label: Microsoft OneDrive Groups.site API
  slug: microsoft-onedrive-groups-site-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-onedrive/openapi/microsoft-onedrive-groups-site-api-openapi.yml
- filename: microsoft-onedrive-me-drive-api-openapi.yml
  format: yaml
  label: Microsoft OneDrive Me.drive API
  slug: microsoft-onedrive-me-drive-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-onedrive/openapi/microsoft-onedrive-me-drive-api-openapi.yml
- filename: microsoft-onedrive-sites-drive-api-openapi.yml
  format: yaml
  label: Microsoft OneDrive Sites.drive API
  slug: microsoft-onedrive-sites-drive-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-onedrive/openapi/microsoft-onedrive-sites-drive-api-openapi.yml
- filename: microsoft-onedrive-users-drive-api-openapi.yml
  format: yaml
  label: Microsoft OneDrive Users.drive API
  slug: microsoft-onedrive-users-drive-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/microsoft-onedrive/openapi/microsoft-onedrive-users-drive-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Microsoft OneDrive Authentication
name_suffix: Authentication
oauth_flows: []
overview: Microsoft OneDrive secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Microsoft OneDrive
provider_slug: microsoft-onedrive
scheme_count: 1
schemes:
- bearerFormat: JWT
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/_superseded/microsoft-onedrive-drive-items-api-openapi.yml
  - openapi/_superseded/microsoft-onedrive-drives-api-openapi.yml
  - openapi/_superseded/microsoft-onedrive-sharing-api-openapi.yml
  type: http
slug: microsoft-onedrive-authentication
source_filename: microsoft-onedrive-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: derived\nsource: openapi/_superseded/microsoft-onedrive-drive-items-api-openapi.yml, openapi/_superseded/microsoft-onedrive-drives-api-openapi.yml,\n  openapi/_superseded/microsoft-onedrive-sharing-api-openapi.yml\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: JWT\n  sources:\n  - openapi/_superseded/microsoft-onedrive-drive-items-api-openapi.yml\n  - openapi/_superseded/microsoft-onedrive-drives-api-openapi.yml\n  - openapi/_superseded/microsoft-onedrive-sharing-api-openapi.yml\n"
source_yaml_url: https://artifacts.apis.io/microsoft-onedrive/authentication/microsoft-onedrive-authentication.yml
summary_line: http · 1 scheme
tags:
- Cloud Storage
- File Storage
- File
- Microsoft
- Microsoft 365
---
