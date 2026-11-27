---
anonymous_access: false
api_key_in: []
api_specs:
- filename: getnoden-com-listings-api-openapi.yml
  format: yaml
  label: Noden Listings API
  slug: getnoden-com-listings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getnoden-com/openapi/getnoden-com-listings-api-openapi.yml
- filename: getnoden-com-operators-api-openapi.yml
  format: yaml
  label: Noden Operators API
  slug: getnoden-com-operators-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getnoden-com/openapi/getnoden-com-operators-api-openapi.yml
- filename: getnoden-com-orders-api-openapi.yml
  format: yaml
  label: Noden Orders API
  slug: getnoden-com-orders-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/getnoden-com/openapi/getnoden-com-orders-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Noden Authentication
name_suffix: Authentication
oauth_flows: []
overview: Noden secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Noden
provider_slug: getnoden-com
scheme_count: 1
schemes:
- description: Operator API key, issued at https://shop.getnoden.com/signup
  name: ApiKeyAuth
  scheme: bearer
  sources:
  - openapi/shop-getnoden-com-openapi.json
  type: http
slug: getnoden-com-authentication
source_filename: getnoden-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-10'\nmethod: derived\nsource: openapi/shop-getnoden-com-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: ApiKeyAuth\n  type: http\n  scheme: bearer\n  description: Operator API key, issued at https://shop.getnoden.com/signup\n  sources:\n  - openapi/shop-getnoden-com-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/getnoden-com/authentication/getnoden-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Artificial Intelligence
- Marketplace
- Bitcoin
- Lightning
- Agents
- Company
---
