---
anonymous_access: false
api_key_in: []
api_specs:
- filename: arena-predictions-com-api-keys-api-openapi.yml
  format: yaml
  label: Arena API keys API
  slug: arena-predictions-com-api-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arena-predictions-com/openapi/arena-predictions-com-api-keys-api-openapi.yml
- filename: arena-predictions-com-identity-api-openapi.yml
  format: yaml
  label: Arena Identity API
  slug: arena-predictions-com-identity-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arena-predictions-com/openapi/arena-predictions-com-identity-api-openapi.yml
- filename: arena-predictions-com-markets-api-openapi.yml
  format: yaml
  label: Arena Markets API
  slug: arena-predictions-com-markets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arena-predictions-com/openapi/arena-predictions-com-markets-api-openapi.yml
- filename: arena-predictions-com-portfolio-api-openapi.yml
  format: yaml
  label: Arena Portfolio API
  slug: arena-predictions-com-portfolio-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arena-predictions-com/openapi/arena-predictions-com-portfolio-api-openapi.yml
- filename: arena-predictions-com-records-api-openapi.yml
  format: yaml
  label: Arena Records API
  slug: arena-predictions-com-records-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arena-predictions-com/openapi/arena-predictions-com-records-api-openapi.yml
- filename: arena-predictions-com-status-api-openapi.yml
  format: yaml
  label: Arena Status API
  slug: arena-predictions-com-status-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arena-predictions-com/openapi/arena-predictions-com-status-api-openapi.yml
- filename: arena-predictions-com-trading-api-openapi.yml
  format: yaml
  label: Arena Trading API
  slug: arena-predictions-com-trading-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arena-predictions-com/openapi/arena-predictions-com-trading-api-openapi.yml
- filename: arena-predictions-com-usage-api-openapi.yml
  format: yaml
  label: Arena Usage API
  slug: arena-predictions-com-usage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arena-predictions-com/openapi/arena-predictions-com-usage-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: Arena Authentication
name_suffix: Authentication
oauth_flows: []
overview: Arena declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Arena
provider_slug: arena-predictions-com
scheme_count: 2
schemes:
- bearerFormat: arena_sk_
  description: Send an arena_sk_ key as a bearer token. Scopes decide what it can do.
  header: Authorization
  scheme: bearer
  type: http
- bearerFormat: arena_sk_
  description: Clients that cannot set Authorization may send x-arena-key header.
  header: x-arena-key
  scheme: bearer
  type: http
slug: arena-predictions-com-authentication
source_filename: arena-predictions-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: searched\nsource: https://docs.arena-predictions.com/authentication.md\nschemes:\n  - type: http\n    scheme: bearer\n    bearerFormat: arena_sk_\n    description: Send an arena_sk_ key as a bearer token. Scopes decide what it can do.\n    header: Authorization\n  - type: http\n    scheme: bearer\n    bearerFormat: arena_sk_\n    description: Clients that cannot set Authorization may send x-arena-key header.\n    header: x-arena-key"
source_yaml_url: https://artifacts.apis.io/arena-predictions-com/authentication/arena-predictions-com-authentication.yml
summary_line: 2 schemes
tags:
- Prediction Markets
- Paper Trading
- Sandbox
- CLI
---
