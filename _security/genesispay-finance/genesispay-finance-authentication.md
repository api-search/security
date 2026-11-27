---
anonymous_access: false
api_key_in: []
api_specs:
- filename: genesispay-finance-openapi-generated.yml
  format: yaml
  label: GenesisPay API
  slug: genesispay-finance-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/genesispay-finance/openapi/_ae-authored/genesispay-finance-openapi-generated.yml
auth_types: []
description: 'Authenticated endpoints take Authorization: Bearer <secret>'
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: GenesisPay Authentication
name_suffix: Authentication
oauth_flows: []
overview: GenesisPay declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: GenesisPay
provider_slug: genesispay-finance
scheme_count: 1
schemes:
- evidence: 'Authenticated endpoints take Authorization: Bearer <secret> — seller endpoints use gp_sk_ keys, agent endpoints use gp_ag_ keys.'
  header: Authorization
  how_to_obtain: Keys are created in the dashboard, shown once, and revocable.
  location: header
  name: Bearer
  type: http-bearer
slug: genesispay-finance-authentication
source_filename: genesispay-finance-authentication.yml
source_heading: Authentication Profile
source_url: https://genesispay.finance/docs/api
source_yaml: "generated: '2026-11-09'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://genesispay.finance/docs/api\nsources:\n- https://genesispay.finance/docs/api\n- https://genesispay.finance/docs/sellers\n- https://genesispay.finance/docs/agents\n- https://genesispay.finance/docs/mcp\ndescription: 'Authenticated endpoints take Authorization: Bearer <secret>'\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: 'Authenticated endpoints take Authorization: Bearer <secret> — seller endpoints use gp_sk_ keys, agent endpoints use gp_ag_ keys.'\n  location: header\n  header: Authorization\n  how_to_obtain: Keys are created in the dashboard, shown once, and revocable.\ndocs: https://genesispay.finance/docs/api\n"
source_yaml_url: https://artifacts.apis.io/genesispay-finance/authentication/genesispay-finance-authentication.yml
summary_line: 1 scheme
tags:
- Artificial Intelligence
- Payments
- E-Commerce
- Stablecoins
- Non-Custodial
---
