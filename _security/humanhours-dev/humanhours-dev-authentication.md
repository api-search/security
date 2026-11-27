---
anonymous_access: false
api_key_in: []
api_specs:
- filename: humanhours-dev-openapi-generated.yml
  format: yaml
  label: HumanHours API
  slug: humanhours-dev-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/humanhours-dev/openapi/_ae-authored/humanhours-dev-openapi-generated.yml
auth_types: []
description: HumanHours uses an API key provided as a Bearer token in the Authorization header.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: HumanHours Authentication
name_suffix: Authentication
oauth_flows: []
overview: HumanHours declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: HumanHours
provider_slug: humanhours-dev
scheme_count: 1
schemes:
- evidence: 'Authorization: Bearer $HUMANHOURS_API_KEY'
  header: Authorization
  how_to_obtain: Create an API key in the dashboard under /api-keys and copy the raw key.
  location: header
  name: Bearer
  type: http-bearer
slug: humanhours-dev-authentication
source_filename: humanhours-dev-authentication.yml
source_heading: Authentication Profile
source_url: https://humanhours.dev/blog/fully-loaded-ai-agent-cost
source_yaml: "generated: '2026-11-11'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://humanhours.dev/blog/fully-loaded-ai-agent-cost\nsources:\n- https://humanhours.dev/blog/fully-loaded-ai-agent-cost\n- https://humanhours.dev/docs/model-cost\n- https://humanhours.dev/docs/quickstart\n- https://humanhours.dev/api/docs-raw/quickstart\ndescription: HumanHours uses an API key provided as a Bearer token in the Authorization header.\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: 'Authorization: Bearer $HUMANHOURS_API_KEY'\n  location: header\n  header: Authorization\n  how_to_obtain: Create an API key in the dashboard under /api-keys and copy the raw key.\nnote: No other authentication methods (apiKey, oauth2, etc.) are documented on the provided pages.\ndocs: https://humanhours.dev/blog/fully-loaded-ai-agent-cost\n"
source_yaml_url: https://artifacts.apis.io/humanhours-dev/authentication/humanhours-dev-authentication.yml
summary_line: 1 scheme
tags:
- Artificial Intelligence
- Finance
- Automation
- Analytics
- Software-as-a-Service
- Company
---
