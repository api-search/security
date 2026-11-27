---
anonymous_access: false
api_key_in: []
api_specs:
- filename: lexq-io-openapi-generated.yml
  format: yaml
  label: LexQ API
  slug: lexq-io-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/lexq-io/openapi/_ae-authored/lexq-io-openapi-generated.yml
auth_types: []
description: API Key Authentication
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: LexQ Authentication
name_suffix: Authentication
oauth_flows: []
overview: LexQ declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: LexQ
provider_slug: lexq-io
scheme_count: 1
schemes:
- evidence: 'LexQ uses API keys to authenticate all API requests. Include your key in the `x-api-key` header:'
  header: x-api-key
  how_to_obtain: Log in to the LexQ Console → Management → API Keys → Create API Key → Copy the key immediately — it will not be shown again
  location: header
  name: API Key
  type: apiKey
slug: lexq-io-authentication
source_filename: lexq-io-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.lexq.io/api/authentication.md
source_yaml: "generated: '2026-11-15'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.lexq.io/api/authentication.md\nsources:\n- https://docs.lexq.io/api/authentication.md\n- https://docs.lexq.io/cli/installation.md\n- https://docs.lexq.io/api/authentication\n- https://docs.lexq.io/quickstart.md\ndescription: API Key Authentication\nschemes:\n- type: apiKey\n  name: API Key\n  evidence: 'LexQ uses API keys to authenticate all API requests. Include your key in the `x-api-key` header:'\n  location: header\n  header: x-api-key\n  how_to_obtain: Log in to the LexQ Console → Management → API Keys → Create API Key → Copy the key immediately — it will not be shown again\ndocs: https://docs.lexq.io/api/authentication.md\n"
source_yaml_url: https://artifacts.apis.io/lexq-io/authentication/lexq-io-authentication.yml
summary_line: 1 scheme
tags:
- Decision Operations
- Rule Engine
- Business Rules
- Audit Trail
- Impact Simulation
---
