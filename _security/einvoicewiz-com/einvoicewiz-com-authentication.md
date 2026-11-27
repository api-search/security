---
anonymous_access: false
api_key_in: []
api_specs:
- filename: einvoicewiz-com-facturx-api-openapi.yml
  format: yaml
  label: einvoicewiz Facturx API
  slug: einvoicewiz-com-facturx-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/einvoicewiz-com/openapi/einvoicewiz-com-facturx-api-openapi.yml
- filename: einvoicewiz-com-generate-api-openapi.yml
  format: yaml
  label: einvoicewiz Generate API
  slug: einvoicewiz-com-generate-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/einvoicewiz-com/openapi/einvoicewiz-com-generate-api-openapi.yml
- filename: einvoicewiz-com-me-api-openapi.yml
  format: yaml
  label: einvoicewiz Me API
  slug: einvoicewiz-com-me-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/einvoicewiz-com/openapi/einvoicewiz-com-me-api-openapi.yml
- filename: einvoicewiz-com-signup-api-openapi.yml
  format: yaml
  label: einvoicewiz Signup API
  slug: einvoicewiz-com-signup-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/einvoicewiz-com/openapi/einvoicewiz-com-signup-api-openapi.yml
- filename: einvoicewiz-com-validate-api-openapi.yml
  format: yaml
  label: einvoicewiz Validate API
  slug: einvoicewiz-com-validate-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/einvoicewiz-com/openapi/einvoicewiz-com-validate-api-openapi.yml
- filename: einvoicewiz-com-verify-api-openapi.yml
  format: yaml
  label: einvoicewiz Verify API
  slug: einvoicewiz-com-verify-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/einvoicewiz-com/openapi/einvoicewiz-com-verify-api-openapi.yml
auth_types: []
description: Authentication is performed by providing the API key returned from the signup endpoint in the X-API-Key request header.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: einvoicewiz Authentication
name_suffix: Authentication
oauth_flows: []
overview: einvoicewiz declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: einvoicewiz
provider_slug: einvoicewiz-com
scheme_count: 1
schemes:
- evidence: 'curl -X POST https://einvoicewiz.com/v1/generate \ -H "X-API-Key: eiw_..." -H "Content-Type: application/json" -d ''{...}'''
  header: X-API-Key
  how_to_obtain: POST to /v1/signup with an email to receive an API key (20 free credits).
  location: header
  name: X-API-Key
  type: apiKey
slug: einvoicewiz-com-authentication
source_filename: einvoicewiz-com-authentication.yml
source_heading: Authentication Profile
source_url: https://einvoicewiz.com/developers
source_yaml: "generated: '2026-11-06'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://einvoicewiz.com/developers\nsources:\n- https://einvoicewiz.com/developers\ndescription: Authentication is performed by providing the API key returned from the signup endpoint in the X-API-Key request header.\nschemes:\n- type: apiKey\n  name: X-API-Key\n  evidence: 'curl -X POST https://einvoicewiz.com/v1/generate \\ -H \"X-API-Key: eiw_...\" -H \"Content-Type: application/json\" -d ''{...}'''\n  location: header\n  header: X-API-Key\n  how_to_obtain: POST to /v1/signup with an email to receive an API key (20 free credits).\ndocs: https://einvoicewiz.com/developers\n"
source_yaml_url: https://artifacts.apis.io/einvoicewiz-com/authentication/einvoicewiz-com-authentication.yml
summary_line: 1 scheme
tags:
- Invoicing
- e-invoice
- Conversion
- European
- Compliance
- Fintech
---
