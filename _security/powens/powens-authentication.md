---
anonymous_access: false
api_key_in: []
api_specs:
- filename: powens-openapi-generated.yml
  format: yaml
  label: Powens API
  slug: powens-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/powens/openapi/_ae-authored/powens-openapi-generated.yml
auth_types: []
description: Authentication is performed by sending a Bearer token in the Authorization header.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Powens Authentication
name_suffix: Authentication
oauth_flows: []
overview: Powens declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Powens
provider_slug: powens
scheme_count: 1
schemes:
- evidence: 'The way to authenticate is by passing the `authorization: Bearer <token>` header in your request.'
  header: authorization
  location: header
  name: Bearer
  type: http-bearer
slug: powens-authentication
source_filename: powens-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.powens.com/documentation/integration-guides/quick-start.md
source_yaml: "generated: '2026-10-21'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.powens.com/documentation/integration-guides/quick-start.md\nsources:\n- https://docs.powens.com/documentation/integration-guides/quick-start.md\n- https://docs.powens.com/documentation/integration-guides/quick-start/api-overview.md\n- https://docs.powens.com/documentation/integration-guides/quick-start/add-a-first-user-and-connection.md\n- https://docs.powens.com/documentation/integration-guides/pay-by-bank/getting-started-with-pay-by-bank.md\ndescription: Authentication is performed by sending a Bearer token in the Authorization header.\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: 'The way to authenticate is by passing the `authorization: Bearer <token>` header in your request.'\n  location: header\n  header: authorization\nnote: No OAuth2, apiKey, or other authentication mechanisms are described on the provided pages.\ndocs: https://docs.powens.com/documentation/integration-guides/quick-start.md\n"
source_yaml_url: https://artifacts.apis.io/powens/authentication/powens-authentication.yml
summary_line: 1 scheme
tags:
- Company
- FinTech
- OpenFinance
- APIs
- Payments
---
