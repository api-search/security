---
anonymous_access: true
api_key_in: []
api_specs:
- filename: launch529-com-openapi-generated.yml
  format: yaml
  label: Launch529 API
  slug: launch529-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/launch529-com/openapi/_ae-authored/launch529-com-openapi-generated.yml
auth_types: []
description: Launch529 uses a simple API key sent as a Bearer token in the Authorization header for authenticated endpoints; open endpoints require no authentication.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Launch529 Authentication
name_suffix: Authentication
oauth_flows: []
overview: Launch529 declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Launch529
provider_slug: launch529-com
scheme_count: 2
schemes:
- evidence: 'Send your key as a bearer token: curl -X POST https://launch529.com/api/v1/tools/add_planned_child \ -H "Authorization: Bearer YOUR_API_KEY"'
  header: Authorization
  how_to_obtain: Create an API key under Connect → AI in the Launch529 dashboard.
  location: header
  name: API Key
  type: http-bearer
- evidence: Leave Authentication on None.
  name: None
  type: none
slug: launch529-com-authentication
source_filename: launch529-com-authentication.yml
source_heading: Authentication Profile
source_url: https://launch529.com/connect/developers
source_yaml: "generated: '2026-11-15'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://launch529.com/connect/developers\nsources:\n- https://launch529.com/connect/developers\ndescription: Launch529 uses a simple API key sent as a Bearer token in the Authorization header for authenticated endpoints; open endpoints require\n  no authentication.\nschemes:\n- type: http-bearer\n  name: API Key\n  evidence: 'Send your key as a bearer token: curl -X POST https://launch529.com/api/v1/tools/add_planned_child \\ -H \"Authorization: Bearer YOUR_API_KEY\"'\n  location: header\n  header: Authorization\n  how_to_obtain: Create an API key under Connect → AI in the Launch529 dashboard.\n- type: none\n  name: None\n  evidence: Leave Authentication on None.\ndocs: https://launch529.com/connect/developers\n"
source_yaml_url: https://artifacts.apis.io/launch529-com/authentication/launch529-com-authentication.yml
summary_line: 2 schemes
tags:
- 529 Savings
- College Savings Planner
- Expense Tracking
- IRS Compliance
---
