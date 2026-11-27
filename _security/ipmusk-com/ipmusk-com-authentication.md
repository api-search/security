---
anonymous_access: false
api_key_in: []
api_specs:
- filename: ipmusk-com-locations-api-openapi.yml
  format: yaml
  label: IPMusk Locations API
  slug: ipmusk-com-locations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ipmusk-com/openapi/ipmusk-com-locations-api-openapi.yml
- filename: ipmusk-com-me-api-openapi.yml
  format: yaml
  label: IPMusk Me API
  slug: ipmusk-com-me-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ipmusk-com/openapi/ipmusk-com-me-api-openapi.yml
- filename: ipmusk-com-openapi-json-api-openapi.yml
  format: yaml
  label: IPMusk Openapi.json API
  slug: ipmusk-com-openapi-json-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ipmusk-com/openapi/ipmusk-com-openapi-json-api-openapi.yml
- filename: ipmusk-com-orders-api-openapi.yml
  format: yaml
  label: IPMusk Orders API
  slug: ipmusk-com-orders-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ipmusk-com/openapi/ipmusk-com-orders-api-openapi.yml
- filename: ipmusk-com-plans-api-openapi.yml
  format: yaml
  label: IPMusk Plans API
  slug: ipmusk-com-plans-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ipmusk-com/openapi/ipmusk-com-plans-api-openapi.yml
- filename: ipmusk-com-products-api-openapi.yml
  format: yaml
  label: IPMusk Products API
  slug: ipmusk-com-products-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ipmusk-com/openapi/ipmusk-com-products-api-openapi.yml
- filename: ipmusk-com-quotes-api-openapi.yml
  format: yaml
  label: IPMusk Quotes API
  slug: ipmusk-com-quotes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ipmusk-com/openapi/ipmusk-com-quotes-api-openapi.yml
- filename: ipmusk-com-residential-api-openapi.yml
  format: yaml
  label: IPMusk Residential API
  slug: ipmusk-com-residential-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ipmusk-com/openapi/ipmusk-com-residential-api-openapi.yml
- filename: ipmusk-com-static-proxies-api-openapi.yml
  format: yaml
  label: IPMusk Static Proxies API
  slug: ipmusk-com-static-proxies-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ipmusk-com/openapi/ipmusk-com-static-proxies-api-openapi.yml
- filename: ipmusk-com-tickets-api-openapi.yml
  format: yaml
  label: IPMusk Tickets API
  slug: ipmusk-com-tickets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ipmusk-com/openapi/ipmusk-com-tickets-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
mechanism_count: 2
method: searched
name: IPMusk Authentication
name_suffix: Authentication
oauth_flows: []
overview: IPMusk declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: IPMusk
provider_slug: ipmusk-com
scheme_count: 2
schemes:
- evidence: IPMusk uses username and password authentication for proxy connections.
  how_to_obtain: Issued automatically when your first traffic package is delivered; shown read‑only in the Residential workspace.
  location: proxy URL (http://USERNAME:PASSWORD@PROXY_HOST:PORT)
  name: Proxy username/password
  type: other
- evidence: Send the key in the Authorization header as a Bearer token.
  header: Authorization
  how_to_obtain: Create a key in the dashboard under Settings → API keys, then copy the full key.
  location: header
  name: API key Bearer token
  scopes:
  - read
  - connect
  - support
  - order
  type: http-bearer
slug: ipmusk-com-authentication
source_filename: ipmusk-com-authentication.yml
source_heading: Authentication Profile
source_url: https://ipmusk.com/docs/authentication
source_yaml: "generated: '2026-11-12'\nmethod: searched\ngenerator: extract-docs-artifacts.py (local)\nsource: https://ipmusk.com/docs/authentication\nsources:\n- https://ipmusk.com/docs/authentication\n- https://ipmusk.com/docs/api\n- https://ipmusk.com/es/docs/authentication\n- https://ipmusk.com/it/docs/authentication\nschemes:\n- type: other\n  name: Proxy username/password\n  evidence: IPMusk uses username and password authentication for proxy connections.\n  location: proxy URL (http://USERNAME:PASSWORD@PROXY_HOST:PORT)\n  how_to_obtain: Issued automatically when your first traffic package is delivered; shown read‑only in the Residential workspace.\n- type: http-bearer\n  name: API key Bearer token\n  evidence: Send the key in the Authorization header as a Bearer token.\n  location: header\n  header: Authorization\n  scopes:\n  - read\n  - connect\n  - support\n  - order\n  how_to_obtain: Create a key in the dashboard under Settings → API keys, then copy the full key.\ndocs: https://ipmusk.com/docs/authentication\n"
source_yaml_url: https://artifacts.apis.io/ipmusk-com/authentication/ipmusk-com-authentication.yml
summary_line: 2 schemes
tags:
- Proxy
- Web Scraping
- Data Collection
- Developer Tools
---
