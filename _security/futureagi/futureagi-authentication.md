---
anonymous_access: false
api_key_in: []
api_specs:
- filename: futureagi-api-openapi.json
  format: json
  label: Future AGI API API
  slug: future-agi-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/futureagi/openapi/_original/futureagi-api-openapi.json
auth_types: []
description: Authentication methods published for Future AGI
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Futureagi Authentication
name_suffix: Authentication
oauth_flows: []
overview: Future AGI declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Future AGI
provider_slug: futureagi
scheme_count: 1
schemes:
- evidence: API keys authenticate your application with Future AGI. Each key pair consists of an API Key ( FI_API_KEY ) and a Secret Key ( FI_SECRET_KEY ).
  how_to_obtain: Create via Settings > API Keys in the Future AGI dashboard (https://app.futureagi.com/dashboard/keys).
  name: FI_API_KEY / FI_SECRET_KEY
  type: apiKey
slug: futureagi-authentication
source_filename: futureagi-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.futureagi.com/docs/admin-settings/api-keys
source_yaml: "generated: '2026-10-20'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.futureagi.com/docs/admin-settings/api-keys\nsources:\n- https://docs.futureagi.com/docs/admin-settings/api-keys\n- https://docs.futureagi.com/docs/self-hosting/configuration/launch-mode\n- https://docs.futureagi.com/docs/observe/quickstart\n- https://docs.futureagi.com/docs/observe/guides/setup-alerts\ndescription: Authentication methods published for Future AGI\nschemes:\n- type: apiKey\n  name: FI_API_KEY / FI_SECRET_KEY\n  evidence: API keys authenticate your application with Future AGI. Each key pair consists of an API Key ( FI_API_KEY ) and a Secret Key ( FI_SECRET_KEY\n    ).\n  how_to_obtain: Create via Settings > API Keys in the Future AGI dashboard (https://app.futureagi.com/dashboard/keys).\ndocs: https://docs.futureagi.com/docs/admin-settings/api-keys\n"
source_yaml_url: https://artifacts.apis.io/futureagi/authentication/futureagi-authentication.yml
summary_line: 1 scheme
tags:
- Company
- AI
- Platform
- Agents
- Simulation
- Monitoring
---
