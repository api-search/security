---
anonymous_access: false
api_key_in: []
api_specs:
- filename: logokit-com-brand-api-api-openapi.yml
  format: yaml
  label: logokit-com Brand API
  slug: logokit-com-brand-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/logokit-com/openapi/logokit-com-brand-api-api-openapi.yml
- filename: logokit-com-crypto-logo-api-api-openapi.yml
  format: yaml
  label: logokit-com Crypto Logo API
  slug: logokit-com-crypto-logo-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/logokit-com/openapi/logokit-com-crypto-logo-api-api-openapi.yml
- filename: logokit-com-logo-api-api-openapi.yml
  format: yaml
  label: logokit-com Logo API
  slug: logokit-com-logo-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/logokit-com/openapi/logokit-com-logo-api-api-openapi.yml
- filename: logokit-com-stock-logo-api-api-openapi.yml
  format: yaml
  label: logokit-com Stock Logo API
  slug: logokit-com-stock-logo-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/logokit-com/openapi/logokit-com-stock-logo-api-api-openapi.yml
auth_types: []
description: Authentication schemes for LogoKit APIs
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: Logokit Com Authentication
name_suffix: Authentication
oauth_flows: []
overview: logokit-com declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: logokit-com
provider_slug: logokit-com
scheme_count: 2
schemes:
- evidence: To authenticate requests made to the Logo API, you need to include your publishable API token as a query parameter in the request URL.
  how_to_obtain: Listed under Logo API Tokens in the Dashboard
  location: query
  name: Publishable API Token
  type: apiKey
- evidence: Brand API endpoints are authenticated using Bearer token authentication. You must provide a valid API token in the Authorization header of your request.
  header: Authorization
  how_to_obtain: Listed under Brand API Tokens in the Dashboard
  location: header
  name: Secret API Token
  type: http-bearer
slug: logokit-com-authentication
source_filename: logokit-com-authentication.yml
source_heading: Authentication Profile
source_url: https://docs.logokit.com/authentication.md
source_yaml: "generated: '2026-10-31'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://docs.logokit.com/authentication.md\nsources:\n- https://docs.logokit.com/authentication.md\n- https://docs.logokit.com/authentication\n- https://docs.logokit.com/quick-start.md\n- https://docs.logokit.com/quick-start\ndescription: Authentication schemes for LogoKit APIs\nschemes:\n- type: apiKey\n  name: Publishable API Token\n  evidence: To authenticate requests made to the Logo API, you need to include your publishable API token as a query parameter in the request\n    URL.\n  location: query\n  how_to_obtain: Listed under Logo API Tokens in the Dashboard\n- type: http-bearer\n  name: Secret API Token\n  evidence: Brand API endpoints are authenticated using Bearer token authentication. You must provide a valid API token in the Authorization header\n    of your request.\n  location: header\n  header: Authorization\n  how_to_obtain: Listed under Brand API Tokens in the Dashboard\n\
  docs: https://docs.logokit.com/authentication.md\n"
source_yaml_url: https://artifacts.apis.io/logokit-com/authentication/logokit-com-authentication.yml
summary_line: 2 schemes
tags:
- Company
- API
- Logos
- Branding
- Data
---
