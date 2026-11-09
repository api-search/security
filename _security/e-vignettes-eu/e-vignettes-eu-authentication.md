---
anonymous_access: false
api_key_in: []
api_specs:
- filename: e-vignettes-eu-countries-api-openapi.yml
  format: yaml
  label: Vignette ID Countries API
  slug: e-vignettes-eu-countries-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/e-vignettes-eu/openapi/e-vignettes-eu-countries-api-openapi.yml
- filename: e-vignettes-eu-products-api-openapi.yml
  format: yaml
  label: Vignette ID Products API
  slug: e-vignettes-eu-products-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/e-vignettes-eu/openapi/e-vignettes-eu-products-api-openapi.yml
auth_types: []
description: Vignette ID uses a static partner API key sent as an HTTP Authorization header of the form `Bearer YOUR_PARTNER_API_KEY`.
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: E Vignettes Eu Authentication
name_suffix: Authentication
oauth_flows: []
overview: Vignette ID declares 1 security scheme(s) across its OpenAPI definitions.
provider_name: Vignette ID
provider_slug: e-vignettes-eu
scheme_count: 1
schemes:
- evidence: 'One authentication method is supported: a static partner API key, sent as an HTTP Authorization header of the form Bearer followed by a single space and the key.'
  header: Authorization
  how_to_obtain: Apply through the partner form at https://e-vignettes.eu/partner; the key is then read from the Partner Panel, section For Developers.
  location: header
  name: Bearer token
  type: apiKey
slug: e-vignettes-eu-authentication
source_filename: e-vignettes-eu-authentication.yml
source_heading: Authentication Profile
source_url: https://e-vignettes.eu/auth.md
source_yaml: "generated: '2026-11-06'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://e-vignettes.eu/auth.md\nsources:\n- https://e-vignettes.eu/auth.md\ndescription: Vignette ID uses a static partner API key sent as an HTTP Authorization header of the form `Bearer YOUR_PARTNER_API_KEY`.\nschemes:\n- type: apiKey\n  name: Bearer token\n  evidence: 'One authentication method is supported: a static partner API key, sent as an HTTP Authorization header of the form Bearer followed\n    by a single space and the key.'\n  location: header\n  header: Authorization\n  how_to_obtain: Apply through the partner form at https://e-vignettes.eu/partner; the key is then read from the Partner Panel, section For Developers.\nnote: OAuth 2.0 and OpenID Connect are not supported.\ndocs: https://e-vignettes.eu/auth.md\n"
source_yaml_url: https://artifacts.apis.io/e-vignettes-eu/authentication/e-vignettes-eu-authentication.yml
summary_line: 1 scheme
tags:
- Company
- Transportation
- Payments
- Europe
- Digital
---
