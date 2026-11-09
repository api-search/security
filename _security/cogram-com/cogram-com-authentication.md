---
anonymous_access: false
api_key_in: []
api_specs:
- filename: cogram-com-action-items-api-openapi.yml
  format: yaml
  label: Cogram Action Items API
  slug: cogram-com-action-items-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cogram-com/openapi/cogram-com-action-items-api-openapi.yml
- filename: cogram-com-audit-log-api-openapi.yml
  format: yaml
  label: Cogram Audit Log API
  slug: cogram-com-audit-log-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cogram-com/openapi/cogram-com-audit-log-api-openapi.yml
- filename: cogram-com-backup-runs-api-openapi.yml
  format: yaml
  label: Cogram Backup Runs API
  slug: cogram-com-backup-runs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cogram-com/openapi/cogram-com-backup-runs-api-openapi.yml
- filename: cogram-com-board-items-api-openapi.yml
  format: yaml
  label: Cogram Board Items API
  slug: cogram-com-board-items-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cogram-com/openapi/cogram-com-board-items-api-openapi.yml
- filename: cogram-com-data-exports-api-openapi.yml
  format: yaml
  label: Cogram Data Exports API
  slug: cogram-com-data-exports-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cogram-com/openapi/cogram-com-data-exports-api-openapi.yml
- filename: cogram-com-directory-api-openapi.yml
  format: yaml
  label: Cogram Directory API
  slug: cogram-com-directory-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cogram-com/openapi/cogram-com-directory-api-openapi.yml
- filename: cogram-com-project-templates-api-openapi.yml
  format: yaml
  label: Cogram Project Templates API
  slug: cogram-com-project-templates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cogram-com/openapi/cogram-com-project-templates-api-openapi.yml
- filename: cogram-com-project-types-api-openapi.yml
  format: yaml
  label: Cogram Project Types API
  slug: cogram-com-project-types-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cogram-com/openapi/cogram-com-project-types-api-openapi.yml
- filename: cogram-com-projects-api-openapi.yml
  format: yaml
  label: Cogram Projects API
  slug: cogram-com-projects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cogram-com/openapi/cogram-com-projects-api-openapi.yml
- filename: cogram-com-users-api-openapi.yml
  format: yaml
  label: Cogram Users API
  slug: cogram-com-users-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cogram-com/openapi/cogram-com-users-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Cogram Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cogram secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Cogram
provider_slug: cogram-com
scheme_count: 1
schemes:
- bearerFormat: Cogram organization API key
  description: Organization API key. Minted by admins in Organization Settings → Integrations → API Keys; shown once, may carry an expiry.
  name: HTTPBearer
  scheme: bearer
  sources:
  - openapi/api.cogram.com-v1-openapi.json
  type: http
slug: cogram-com-authentication
source_filename: cogram-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: derived\nsource: openapi/api.cogram.com-v1-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: HTTPBearer\n  type: http\n  scheme: bearer\n  bearerFormat: Cogram organization API key\n  description: Organization API key. Minted by admins in Organization Settings → Integrations\n    → API Keys; shown once, may carry an expiry.\n  sources:\n  - openapi/api.cogram.com-v1-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/cogram-com/authentication/cogram-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Artificial Intelligence
- Architecture
- Engineering
- Documentation
- Collaboration
---
