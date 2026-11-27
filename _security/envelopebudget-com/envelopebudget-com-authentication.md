---
anonymous_access: false
api_key_in: []
api_specs:
- filename: envelopebudget-com-accounts-api-openapi.yml
  format: yaml
  label: EnvelopeBudget Accounts API
  slug: envelopebudget-com-accounts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/envelopebudget-com/openapi/envelopebudget-com-accounts-api-openapi.yml
- filename: envelopebudget-com-auth-api-openapi.yml
  format: yaml
  label: EnvelopeBudget Auth API
  slug: envelopebudget-com-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/envelopebudget-com/openapi/envelopebudget-com-auth-api-openapi.yml
- filename: envelopebudget-com-envelopes-api-openapi.yml
  format: yaml
  label: EnvelopeBudget Envelopes API
  slug: envelopebudget-com-envelopes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/envelopebudget-com/openapi/envelopebudget-com-envelopes-api-openapi.yml
- filename: envelopebudget-com-transactions-api-openapi.yml
  format: yaml
  label: EnvelopeBudget Transactions API
  slug: envelopebudget-com-transactions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/envelopebudget-com/openapi/envelopebudget-com-transactions-api-openapi.yml
auth_types: []
description: Authentication for EnvelopeBudget API uses a Bearer token passed in the Authorization header.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: EnvelopeBudget Authentication
name_suffix: Authentication
oauth_flows: []
overview: EnvelopeBudget declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: EnvelopeBudget
provider_slug: envelopebudget-com
scheme_count: 1
schemes:
- evidence: 'Authorization: Bearer YOUR_SECRET_TOKEN'
  header: Authorization
  how_to_obtain: Obtain a token by calling the Create Api Key endpoint (POST /api/auth/api-key) after logging in.
  location: header
  name: Bearer
  type: http-bearer
slug: envelopebudget-com-authentication
source_filename: envelopebudget-com-authentication.yml
source_heading: Authentication Profile
source_url: https://envelopebudget.com/api/docs#POST/api/auth/api-key
source_yaml: "generated: '2026-11-07'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://envelopebudget.com/api/docs#POST/api/auth/api-key\nsources:\n- https://envelopebudget.com/api/docs#POST/api/auth/api-key\n- https://envelopebudget.com/api/docs#GET/api/auth/api-key\n- https://envelopebudget.com/api/docs#DELETE/api/auth/api-key/{api_key_id}\ndescription: Authentication for EnvelopeBudget API uses a Bearer token passed in the Authorization header.\nschemes:\n- type: http-bearer\n  name: Bearer\n  evidence: 'Authorization: Bearer YOUR_SECRET_TOKEN'\n  location: header\n  header: Authorization\n  how_to_obtain: Obtain a token by calling the Create Api Key endpoint (POST /api/auth/api-key) after logging in.\nnote: No other authentication schemes (apiKey, oauth2, etc.) are documented on the provided pages.\ndocs: https://envelopebudget.com/api/docs#POST/api/auth/api-key\n"
source_yaml_url: https://artifacts.apis.io/envelopebudget-com/authentication/envelopebudget-com-authentication.yml
summary_line: 1 scheme
tags:
- Finance
- Budgeting
- Personal Finance
- Couples
- Families
---
