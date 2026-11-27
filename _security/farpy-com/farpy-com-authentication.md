---
anonymous_access: false
api_key_in: []
api_specs:
- filename: farpy-com-api-keys-api-openapi.yml
  format: yaml
  label: Farpy Api Keys API
  slug: farpy-com-api-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/farpy-com/openapi/farpy-com-api-keys-api-openapi.yml
- filename: farpy-com-capabilities-api-openapi.yml
  format: yaml
  label: Farpy Capabilities API
  slug: farpy-com-capabilities-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/farpy-com/openapi/farpy-com-capabilities-api-openapi.yml
- filename: farpy-com-health-api-openapi.yml
  format: yaml
  label: Farpy Health API
  slug: farpy-com-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/farpy-com/openapi/farpy-com-health-api-openapi.yml
- filename: farpy-com-limits-api-openapi.yml
  format: yaml
  label: Farpy Limits API
  slug: farpy-com-limits-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/farpy-com/openapi/farpy-com-limits-api-openapi.yml
- filename: farpy-com-pricing-api-openapi.yml
  format: yaml
  label: Farpy Pricing API
  slug: farpy-com-pricing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/farpy-com/openapi/farpy-com-pricing-api-openapi.yml
- filename: farpy-com-renders-api-openapi.yml
  format: yaml
  label: Farpy Renders API
  slug: farpy-com-renders-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/farpy-com/openapi/farpy-com-renders-api-openapi.yml
- filename: farpy-com-workspace-api-openapi.yml
  format: yaml
  label: Farpy Workspace API
  slug: farpy-com-workspace-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/farpy-com/openapi/farpy-com-workspace-api-openapi.yml
auth_types: []
description: Authentication schemes as documented on the Farpy Quickstart page
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Farpy Authentication
name_suffix: Authentication
oauth_flows: []
overview: Farpy declares 3 security scheme(s) across its OpenAPI definitions.
provider_name: Farpy
provider_slug: farpy-com
scheme_count: 3
schemes:
- evidence: 'Browser: session cookie.'
  location: cookie
  name: session cookie
  type: apiKey
- evidence: 'Inspect/start: Job API farpy_agent_… Bearer key.'
  header: Authorization
  how_to_obtain: Export FARPY_AGENT_KEY environment variable (e.g., export FARPY_AGENT_KEY="farpy_agent_...")
  location: header
  name: farpy_agent_key
  scopes:
  - jobs:inspect
  - jobs:quote
  - jobs:start
  - jobs:status
  type: http-bearer
- evidence: 'Public API V1 /v1/renders : Account Settings farpy_… key.'
  header: Authorization
  how_to_obtain: Export FARPY_ACCOUNT_KEY environment variable (e.g., export FARPY_ACCOUNT_KEY="farpy_...")
  location: header
  name: farpy_account_key
  type: http-bearer
slug: farpy-com-authentication
source_filename: farpy-com-authentication.yml
source_heading: Authentication Profile
source_url: https://farpy.com/api/quickstart/
source_yaml: "generated: '2026-11-08'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://farpy.com/api/quickstart/\nsources:\n- https://farpy.com/api/quickstart/\ndescription: Authentication schemes as documented on the Farpy Quickstart page\nschemes:\n- type: apiKey\n  name: session cookie\n  evidence: 'Browser: session cookie.'\n  location: cookie\n- type: http-bearer\n  name: farpy_agent_key\n  evidence: 'Inspect/start: Job API farpy_agent_… Bearer key.'\n  location: header\n  header: Authorization\n  scopes:\n  - jobs:inspect\n  - jobs:quote\n  - jobs:start\n  - jobs:status\n  how_to_obtain: Export FARPY_AGENT_KEY environment variable (e.g., export FARPY_AGENT_KEY=\"farpy_agent_...\")\n- type: http-bearer\n  name: farpy_account_key\n  evidence: 'Public API V1 /v1/renders : Account Settings farpy_… key.'\n  location: header\n  header: Authorization\n  how_to_obtain: Export FARPY_ACCOUNT_KEY environment variable (e.g., export FARPY_ACCOUNT_KEY=\"farpy_...\"\
  )\ndocs: https://farpy.com/api/quickstart/\n"
source_yaml_url: https://artifacts.apis.io/farpy-com/authentication/farpy-com-authentication.yml
summary_line: 3 schemes
tags:
- Company
- GPU
- Rendering
- Blender
- Cloud
---
