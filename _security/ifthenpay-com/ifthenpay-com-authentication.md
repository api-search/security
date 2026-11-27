---
anonymous_access: false
api_key_in: []
api_specs:
- filename: ifthenpay-com-openapi-generated.yml
  format: yaml
  label: Ifthenpay API
  slug: ifthenpay-com-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ifthenpay-com/openapi/_ae-authored/ifthenpay-com-openapi-generated.yml
auth_types: []
description: Authentication is performed by generating a JWT bearer token via POST /api/v1/auth/token using a backofficeKey. The returned token must be sent in the Authorization header as a Bearer token for all subsequent calls.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Ifthenpay Authentication
name_suffix: Authentication
oauth_flows: []
overview: Ifthenpay declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Ifthenpay
provider_slug: ifthenpay-com
scheme_count: 1
schemes:
- evidence: All subsequent API calls require this bearer token in the header.
  header: Authorization
  how_to_obtain: POST to /api/v1/auth/token with JSON body containing backofficeKey to receive an access_token.
  location: header
  name: JWT Bearer
  type: http-bearer
slug: ifthenpay-com-authentication
source_filename: ifthenpay-com-authentication.yml
source_heading: Authentication Profile
source_url: https://www.ifthenpay.com/docs/en/api/directdebit/
source_yaml: "generated: '2026-11-12'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://www.ifthenpay.com/docs/en/api/directdebit/\nsources:\n- https://www.ifthenpay.com/docs/en/api/directdebit/\ndescription: Authentication is performed by generating a JWT bearer token via POST /api/v1/auth/token using a backofficeKey. The returned token\n  must be sent in the Authorization header as a Bearer token for all subsequent calls.\nschemes:\n- type: http-bearer\n  name: JWT Bearer\n  evidence: All subsequent API calls require this bearer token in the header.\n  location: header\n  header: Authorization\n  how_to_obtain: POST to /api/v1/auth/token with JSON body containing backofficeKey to receive an access_token.\ndocs: https://www.ifthenpay.com/docs/en/api/directdebit/\n"
source_yaml_url: https://artifacts.apis.io/ifthenpay-com/authentication/ifthenpay-com-authentication.yml
summary_line: 1 scheme
tags:
- Payments
- Fintech
- E-Commerce
- Point-of-Sale
- Direct Debits
- Payment Gateway
- Digital Banking
---
