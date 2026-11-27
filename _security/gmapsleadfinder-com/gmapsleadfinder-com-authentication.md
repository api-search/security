---
anonymous_access: false
api_key_in: []
api_specs:
- filename: gmapsleadfinder-com-jobs-api-openapi.yml
  format: yaml
  label: GMaps Lead Finder Jobs API
  slug: gmapsleadfinder-com-jobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gmapsleadfinder-com/openapi/gmapsleadfinder-com-jobs-api-openapi.yml
- filename: gmapsleadfinder-com-mcp-api-openapi.yml
  format: yaml
  label: GMaps Lead Finder MCP API
  slug: gmapsleadfinder-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gmapsleadfinder-com/openapi/gmapsleadfinder-com-mcp-api-openapi.yml
- filename: gmapsleadfinder-com-me-api-openapi.yml
  format: yaml
  label: GMaps Lead Finder Me API
  slug: gmapsleadfinder-com-me-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gmapsleadfinder-com/openapi/gmapsleadfinder-com-me-api-openapi.yml
- filename: gmapsleadfinder-com-photo-jobs-api-openapi.yml
  format: yaml
  label: GMaps Lead Finder Photo Jobs API
  slug: gmapsleadfinder-com-photo-jobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gmapsleadfinder-com/openapi/gmapsleadfinder-com-photo-jobs-api-openapi.yml
- filename: gmapsleadfinder-com-review-jobs-api-openapi.yml
  format: yaml
  label: GMaps Lead Finder Review Jobs API
  slug: gmapsleadfinder-com-review-jobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/gmapsleadfinder-com/openapi/gmapsleadfinder-com-review-jobs-api-openapi.yml
auth_types: []
description: Authentication
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: GMaps Lead Finder Authentication
name_suffix: Authentication
oauth_flows: []
overview: GMaps Lead Finder declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: GMaps Lead Finder
provider_slug: gmapsleadfinder-com
scheme_count: 1
schemes:
- evidence: Every /api/v1 request requires an Authorization header with your personal API key.
  header: Authorization
  how_to_obtain: Keys start with gmf_ and are issued in Account after you sign in on an agent‑capable plan.
  location: header
  name: Bearer
  type: http-bearer
slug: gmapsleadfinder-com-authentication
source_filename: gmapsleadfinder-com-authentication.yml
source_heading: Authentication Profile
source_url: https://gmapsleadfinder.com/docs/api
source_yaml: "generated: '2026-11-10'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://gmapsleadfinder.com/docs/api\nsources:\n- https://gmapsleadfinder.com/docs/api\ndescription: Authentication\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: Every /api/v1 request requires an Authorization header with your personal API key.\n  location: header\n  header: Authorization\n  how_to_obtain: Keys start with gmf_ and are issued in Account after you sign in on an agent‑capable plan.\ndocs: https://gmapsleadfinder.com/docs/api\n"
source_yaml_url: https://artifacts.apis.io/gmapsleadfinder-com/authentication/gmapsleadfinder-com-authentication.yml
summary_line: 1 scheme
tags:
- Maps Scraper
- Data Enrichment
---
