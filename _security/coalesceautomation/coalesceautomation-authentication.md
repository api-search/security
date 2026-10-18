---
anonymous_access: false
api_key_in: []
api_specs:
- filename: coalesceautomation-coalesceautomation-api-api-openapi.yml
  format: yaml
  label: Coalesceautomation Coalesceautomation API
  slug: coalesceautomation-coalesceautomation-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coalesceautomation/refs/heads/main/openapi/coalesceautomation-coalesceautomation-api-api-openapi.yml
- filename: coalesceautomation-environments-api-openapi.yml
  format: yaml
  label: Coalesceautomation Environments API
  slug: coalesceautomation-environments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coalesceautomation/refs/heads/main/openapi/coalesceautomation-environments-api-openapi.yml
- filename: coalesceautomation-projects-api-openapi.yml
  format: yaml
  label: Coalesceautomation Projects API
  slug: coalesceautomation-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coalesceautomation/refs/heads/main/openapi/coalesceautomation-projects-api-openapi.yml
- filename: coalesceautomation-public-api-openapi.yml
  format: yaml
  label: Coalesceautomation Public API
  slug: coalesceautomation-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coalesceautomation/refs/heads/main/openapi/coalesceautomation-public-api-openapi.yml
- filename: coalesceautomation-scheduler-api-openapi.yml
  format: yaml
  label: Coalesceautomation Scheduler API
  slug: coalesceautomation-scheduler-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coalesceautomation/refs/heads/main/openapi/coalesceautomation-scheduler-api-openapi.yml
- filename: coalesceautomation-workspaces-api-openapi.yml
  format: yaml
  label: Coalesceautomation Workspaces API
  slug: coalesceautomation-workspaces-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coalesceautomation/refs/heads/main/openapi/coalesceautomation-workspaces-api-openapi.yml
auth_types: []
description: Authentication methods for Coalesce APIs
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Coalesceautomation Authentication
name_suffix: Authentication
oauth_flows: []
overview: Coalesceautomation declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Coalesceautomation
provider_slug: coalesceautomation
scheme_count: 1
schemes:
- evidence: Coalesce uses Bearer Authentication to make API requests.
  header: Authorization
  how_to_obtain: Generate an Access Token via the Deploy tab in the Coalesce UI, or create a Catalog API Token in Settings > API in the Catalog app.
  location: header
  name: Bearer Authentication
  type: http-bearer
slug: coalesceautomation-authentication
source_filename: coalesceautomation-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.coalesce.io/docs/api/authentication
source_yaml: "generated: '2026-10-09'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.coalesce.io/docs/api/authentication\nsources:\n- https://docs.coalesce.io/docs/api/authentication\n- https://docs.coalesce.io/docs/catalog/developer/getting-your-api-keys\n- https://docs.coalesce.io/docs/catalog/administration/authentication/okta\n- https://docs.coalesce.io/docs/catalog/administration/authentication\ndescription: Authentication methods for Coalesce APIs\nschemes:\n- type: http-bearer\n  name: Bearer Authentication\n  evidence: Coalesce uses Bearer Authentication to make API requests.\n  location: header\n  header: Authorization\n  how_to_obtain: Generate an Access Token via the Deploy tab in the Coalesce UI, or create a Catalog API Token in Settings > API in the Catalog\n    app.\nnote: No OAuth2 flows, API key, or other authentication schemes are documented on the provided pages.\ndocs: https://docs.coalesce.io/docs/api/authentication\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/coalesceautomation/refs/heads/main/authentication/coalesceautomation-authentication.yml
summary_line: 1 scheme
tags:
- Data Platform
- Automation
- Metadata
- Cloud Integration
- Artificial Intelligence
- San Francisco
---
