---
anonymous_access: false
api_key_in: []
api_specs:
- filename: cloudsek-bulk-api-openapi.yml
  format: yaml
  label: Cloudsek Bulk API
  slug: cloudsek-bulk-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudsek/refs/heads/main/openapi/cloudsek-bulk-api-openapi.yml
- filename: cloudsek-comments-api-openapi.yml
  format: yaml
  label: Cloudsek Comments API
  slug: cloudsek-comments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudsek/refs/heads/main/openapi/cloudsek-comments-api-openapi.yml
- filename: cloudsek-events-api-openapi.yml
  format: yaml
  label: Cloudsek Events API
  slug: cloudsek-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudsek/refs/heads/main/openapi/cloudsek-events-api-openapi.yml
- filename: cloudsek-incidents-api-openapi.yml
  format: yaml
  label: Cloudsek Incidents API
  slug: cloudsek-incidents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudsek/refs/heads/main/openapi/cloudsek-incidents-api-openapi.yml
- filename: cloudsek-jobs-api-openapi.yml
  format: yaml
  label: Cloudsek Jobs API
  slug: cloudsek-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudsek/refs/heads/main/openapi/cloudsek-jobs-api-openapi.yml
- filename: cloudsek-snapshot-api-openapi.yml
  format: yaml
  label: Cloudsek Snapshot API
  slug: cloudsek-snapshot-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cloudsek/refs/heads/main/openapi/cloudsek-snapshot-api-openapi.yml
auth_types: []
description: Authentication schemes for CloudSEK API
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Cloudsek Authentication
name_suffix: Authentication
oauth_flows: []
overview: Cloudsek declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Cloudsek
provider_slug: cloudsek
scheme_count: 1
schemes:
- evidence: 'Every request carries a bearer token in the Authorization header: Authorization: Bearer <your-access-token>'
  header: Authorization
  how_to_obtain: Create or rotate it in the CloudSEK platform under Integrations → Alerts API → Create token (or Rotate Token).
  location: header
  name: Bearer token
  type: http-bearer
slug: cloudsek-authentication
source_filename: cloudsek-authentication.yml
source_heading: Authentication Profile
source_url: https://api.cloudsek.com/docs/intro/
source_yaml: "generated: '2026-10-09'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://api.cloudsek.com/docs/intro/\nsources:\n- https://api.cloudsek.com/docs/intro/\n- https://api.cloudsek.com/docs/mcp/\n- https://api.cloudsek.com/docs/mcp/claude-desktop/\ndescription: Authentication schemes for CloudSEK API\nschemes:\n- type: http-bearer\n  name: Bearer token\n  evidence: 'Every request carries a bearer token in the Authorization header: Authorization: Bearer <your-access-token>'\n  location: header\n  header: Authorization\n  how_to_obtain: Create or rotate it in the CloudSEK platform under Integrations → Alerts API → Create token (or Rotate Token).\ndocs: https://api.cloudsek.com/docs/intro/\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cloudsek/refs/heads/main/authentication/cloudsek-authentication.yml
summary_line: 1 scheme
tags:
- Security
- Threat Intelligence
- Attack Path
- Predictive Analytics
- Cyber Risk
---
