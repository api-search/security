---
anonymous_access: false
api_key_in: []
api_specs:
- filename: briq-cloud-v1-openapi.json
  format: json
  label: briq API V1 API
  slug: briq-api-v1-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/briq-cloud/openapi/_original/briq-cloud-v1-openapi.json
auth_types: []
description: Authentication
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: briq Authentication
name_suffix: Authentication
oauth_flows: []
overview: briq declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: briq
provider_slug: briq-cloud
scheme_count: 1
schemes:
- evidence: 'Send an API key, created on the dashboard''s Agents page, as a Bearer token:'
  header: Authorization
  how_to_obtain: Create a key on the dashboard's Agents page.
  location: header
  name: Bearer token
  type: http-bearer
slug: briq-cloud-authentication
source_filename: briq-cloud-authentication.yml
source_heading: Authentication Profile
source_url: https://briq.cloud/docs/api/overview
source_yaml: "generated: '2026-11-03'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://briq.cloud/docs/api/overview\nsources:\n- https://briq.cloud/docs/api/overview\n- https://briq.cloud/docs/cli\n- https://briq.cloud/docs/getting-started.md\n- https://briq.cloud/docs/setup/clients.md\ndescription: Authentication\nschemes:\n- type: http-bearer\n  name: Bearer token\n  evidence: 'Send an API key, created on the dashboard''s Agents page, as a Bearer token:'\n  location: header\n  header: Authorization\n  how_to_obtain: Create a key on the dashboard's Agents page.\ndocs: https://briq.cloud/docs/api/overview\n"
source_yaml_url: https://artifacts.apis.io/briq-cloud/authentication/briq-cloud-authentication.yml
summary_line: 1 scheme
tags:
- Artificial Intelligence
- Cloud
- Sandbox
- Database
- Platform
- Company
---
