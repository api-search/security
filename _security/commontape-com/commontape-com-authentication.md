---
anonymous_access: false
api_key_in: []
api_specs:
- filename: commontape-com-book-api-openapi.yml
  format: yaml
  label: CommonTape Book API
  slug: commontape-com-book-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/commontape-com/openapi/commontape-com-book-api-openapi.yml
- filename: commontape-com-cancel-api-openapi.yml
  format: yaml
  label: CommonTape Cancel API
  slug: commontape-com-cancel-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/commontape-com/openapi/commontape-com-cancel-api-openapi.yml
- filename: commontape-com-discover-api-openapi.yml
  format: yaml
  label: CommonTape Discover API
  slug: commontape-com-discover-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/commontape-com/openapi/commontape-com-discover-api-openapi.yml
- filename: commontape-com-hold-api-openapi.yml
  format: yaml
  label: CommonTape Hold API
  slug: commontape-com-hold-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/commontape-com/openapi/commontape-com-hold-api-openapi.yml
- filename: commontape-com-keys-api-openapi.yml
  format: yaml
  label: CommonTape Keys API
  slug: commontape-com-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/commontape-com/openapi/commontape-com-keys-api-openapi.yml
- filename: commontape-com-modify-api-openapi.yml
  format: yaml
  label: CommonTape Modify API
  slug: commontape-com-modify-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/commontape-com/openapi/commontape-com-modify-api-openapi.yml
- filename: commontape-com-quote-api-openapi.yml
  format: yaml
  label: CommonTape Quote API
  slug: commontape-com-quote-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/commontape-com/openapi/commontape-com-quote-api-openapi.yml
- filename: commontape-com-search-api-openapi.yml
  format: yaml
  label: CommonTape Search API
  slug: commontape-com-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/commontape-com/openapi/commontape-com-search-api-openapi.yml
- filename: commontape-com-status-api-openapi.yml
  format: yaml
  label: CommonTape Status API
  slug: commontape-com-status-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/commontape-com/openapi/commontape-com-status-api-openapi.yml
- filename: commontape-com-taxonomy-api-openapi.yml
  format: yaml
  label: CommonTape Taxonomy API
  slug: commontape-com-taxonomy-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/commontape-com/openapi/commontape-com-taxonomy-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: searched
name: CommonTape Authentication
name_suffix: Authentication
oauth_flows: []
overview: CommonTape secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: CommonTape
provider_slug: commontape-com
scheme_count: 1
schemes:
- description: Your agent key (ct_live_...). Get one with POST /api/v1/keys (no key needed); the demo key ct_demo_... needs no registration.
  header: 'Authorization: Bearer <key>'
  issuance: 'Self-service: "Get a key One call, no human. The key is shown once, at starter limits" (POST /api/v1/keys, the MCP register tool, or the docs form). Three keys a day per address; the key is never in the email.'
  key_prefixes:
    demo: ct_demo_
    live: ct_live_
  management: The key page linked from the registration email offers usage, the name owners see, rotate and revoke.
  name: bearerAuth
  scheme: bearer
  sources:
  - openapi/commontape-com-openapi.yml
  - https://commontape.com/docs
  type: http
slug: commontape-com-authentication
source_filename: commontape-com-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: searched\nsource: https://commontape.com/docs\ndocs: https://commontape.com/docs\nsummary:\n  types:\n  - http\nschemes:\n- name: bearerAuth\n  type: http\n  scheme: bearer\n  header: 'Authorization: Bearer <key>'\n  description: Your agent key (ct_live_...). Get one with POST /api/v1/keys (no key needed);\n    the demo key ct_demo_... needs no registration.\n  key_prefixes:\n    live: ct_live_\n    demo: ct_demo_\n  issuance: 'Self-service: \"Get a key One call, no human. The key is shown once, at starter limits\" (POST /api/v1/keys, the MCP register tool, or the docs form). Three keys a day per address; the key is never in the email.'\n  management: The key page linked from the registration email offers usage, the name owners see, rotate and revoke.\n  sources:\n  - openapi/commontape-com-openapi.yml\n  - https://commontape.com/docs\nunauthenticated_access: A search with no key shows supply, prices and reasons, without quote tokens. The word\
  \ list (GET /api/v1/taxonomy/{vertical}) is public, no key.\n"
source_yaml_url: https://artifacts.apis.io/commontape-com/authentication/commontape-com-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- AI Agents
- Booking
- Home Services
- House Cleaning
- MCP
- Marketplace
- Scheduling
---
