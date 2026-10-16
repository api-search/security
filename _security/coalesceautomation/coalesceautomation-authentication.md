---
anonymous_access: false
api_key_in: []
api_specs:
- filename: coalesceautomation-openapi-generated.yml
  format: yaml
  label: Coalesceautomation API
  slug: coalesceautomation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/coalesceautomation/refs/heads/main/openapi/_ae-authored/coalesceautomation-openapi-generated.yml
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
- AI
- San Francisco
---
