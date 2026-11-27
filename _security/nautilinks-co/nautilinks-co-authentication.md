---
anonymous_access: false
api_key_in: []
api_specs:
- filename: nautilinks-co-ai-visibility-api-openapi.yml
  format: yaml
  label: Nautilinks AI visibility API
  slug: nautilinks-co-ai-visibility-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nautilinks-co/openapi/nautilinks-co-ai-visibility-api-openapi.yml
- filename: nautilinks-co-catalog-api-openapi.yml
  format: yaml
  label: Nautilinks Catalog API
  slug: nautilinks-co-catalog-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nautilinks-co/openapi/nautilinks-co-catalog-api-openapi.yml
- filename: nautilinks-co-commerce-api-openapi.yml
  format: yaml
  label: Nautilinks Commerce API
  slug: nautilinks-co-commerce-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nautilinks-co/openapi/nautilinks-co-commerce-api-openapi.yml
- filename: nautilinks-co-webhooks-api-openapi.yml
  format: yaml
  label: Nautilinks Webhooks API
  slug: nautilinks-co-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/nautilinks-co/openapi/nautilinks-co-webhooks-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Nautilinks Authentication
name_suffix: Authentication
oauth_flows: []
overview: Nautilinks secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Nautilinks
provider_slug: nautilinks-co
scheme_count: 1
schemes:
- bearerFormat: sn_live_<40 hex> or sn_test_<40 hex>
  description: Create a live or sandbox key in the Nautilinks member area. Send it on every request; never put it in a URL.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/nautilinks-co-openapi.json
  type: http
slug: nautilinks-co-authentication
source_filename: nautilinks-co-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-19'\nmethod: derived\nsource: openapi/nautilinks-co-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  bearerFormat: sn_live_<40 hex> or sn_test_<40 hex>\n  description: Create a live or sandbox key in the Nautilinks member area. Send it on every\n    request; never put it in a URL.\n  sources:\n  - openapi/nautilinks-co-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/nautilinks-co/authentication/nautilinks-co-authentication.yml
summary_line: http · 1 scheme
tags:
- Netlinking
- Backlinks
- SEO
- Digital-PR
- Link Building
---
