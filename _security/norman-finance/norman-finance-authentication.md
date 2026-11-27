---
anonymous_access: false
api_key_in: []
api_specs:
- filename: norman-finance-openapi-generated.yml
  format: yaml
  label: Norman API
  slug: norman-finance-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/norman-finance/openapi/_ae-authored/norman-finance-openapi-generated.yml
auth_types: []
description: Authenticate with Bearer API keys
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Norman Authentication
name_suffix: Authentication
oauth_flows: []
overview: Norman declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Norman
provider_slug: norman-finance
scheme_count: 1
schemes:
- evidence: 'Send Authorization: Bearer nrm_… on every authenticated request.'
  header: Authorization
  how_to_obtain: Create a key in Automations → Integrations → Public API, choose its permissions, and copy it.
  location: header
  name: Bearer
  type: http-bearer
slug: norman-finance-authentication
source_filename: norman-finance-authentication.yml
source_heading: Authentication Profile
source_url: https://norman.finance/developers/authentication
source_yaml: "generated: '2026-11-19'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://norman.finance/developers/authentication\nsources:\n- https://norman.finance/developers/authentication\n- https://norman.finance/de/en/solutions\n- https://norman.finance/developers/quickstart\ndescription: Authenticate with Bearer API keys\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: 'Send Authorization: Bearer nrm_… on every authenticated request.'\n  location: header\n  header: Authorization\n  how_to_obtain: Create a key in Automations → Integrations → Public API, choose its permissions, and copy it.\nnote: No other authentication schemes (apiKey, oauth2, etc.) are documented on the provided pages.\ndocs: https://norman.finance/developers/authentication\n"
source_yaml_url: https://artifacts.apis.io/norman-finance/authentication/norman-finance-authentication.yml
summary_line: 1 scheme
tags:
- Bookkeeping
- Accounting
- Tax
- Artificial Intelligence
- Invoicing
- Germany
- Poland
---
