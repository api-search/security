---
anonymous_access: false
api_key_in: []
api_specs:
- filename: letshum-com-openapi-generated.yml
  format: yaml
  label: Hum API
  slug: letshum-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/letshum-com/openapi/_ae-authored/letshum-com-openapi-generated.yml
auth_types: []
description: Authentication methods published for Hum APIs
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Hum Authentication
name_suffix: Authentication
oauth_flows: []
overview: Hum declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Hum
provider_slug: letshum-com
scheme_count: 2
schemes:
- evidence: 'Use `GET /ping` as the first authenticated request:'
  header: Authorization
  how_to_obtain: API keys are issued by Hum for each environment. Request keys from your Hum contact or email support@letshum.com. Keys are prefixed with `hum_sandbox_` for Sandbox or `hum_` for Production.
  location: header
  name: Bearer
  type: http-bearer
- evidence: Hum does not require an account or API key.
  name: none
  type: other
slug: letshum-com-authentication
source_filename: letshum-com-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.letshum.com/environments.md
source_yaml: "generated: '2026-11-15'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.letshum.com/environments.md\nsources:\n- https://docs.letshum.com/environments.md\n- https://docs.letshum.com/mcp/quickstart.md\ndescription: Authentication methods published for Hum APIs\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: 'Use `GET /ping` as the first authenticated request:'\n  location: header\n  header: Authorization\n  how_to_obtain: API keys are issued by Hum for each environment. Request keys from your Hum contact or email support@letshum.com. Keys are prefixed\n    with `hum_sandbox_` for Sandbox or `hum_` for Production.\n- type: other\n  name: none\n  evidence: Hum does not require an account or API key.\ndocs: https://docs.letshum.com/environments.md\n"
source_yaml_url: https://artifacts.apis.io/letshum-com/authentication/letshum-com-authentication.yml
summary_line: 2 schemes
tags:
- Internet
- Marketplace
- White Label
- Real Estate
- Software-as-a-Service
---
