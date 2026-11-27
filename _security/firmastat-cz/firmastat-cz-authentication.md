---
anonymous_access: false
api_key_in: []
api_specs:
- filename: firmastat-cz-firma-api-openapi.yml
  format: yaml
  label: Firmastat Firma API
  slug: firmastat-cz-firma-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/firmastat-cz/openapi/firmastat-cz-firma-api-openapi.yml
- filename: firmastat-cz-firmy-api-openapi.yml
  format: yaml
  label: Firmastat Firmy API
  slug: firmastat-cz-firmy-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/firmastat-cz/openapi/firmastat-cz-firmy-api-openapi.yml
- filename: firmastat-cz-health-api-openapi.yml
  format: yaml
  label: Firmastat Health API
  slug: firmastat-cz-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/firmastat-cz/openapi/firmastat-cz-health-api-openapi.yml
- filename: firmastat-cz-osoba-api-openapi.yml
  format: yaml
  label: Firmastat Osoba API
  slug: firmastat-cz-osoba-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/firmastat-cz/openapi/firmastat-cz-osoba-api-openapi.yml
- filename: firmastat-cz-osoby-api-openapi.yml
  format: yaml
  label: Firmastat Osoby API
  slug: firmastat-cz-osoby-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/firmastat-cz/openapi/firmastat-cz-osoby-api-openapi.yml
- filename: firmastat-cz-suggest-api-openapi.yml
  format: yaml
  label: Firmastat Suggest API
  slug: firmastat-cz-suggest-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/firmastat-cz/openapi/firmastat-cz-suggest-api-openapi.yml
- filename: firmastat-cz-vyhledavani-api-openapi.yml
  format: yaml
  label: Firmastat Vyhledavani API
  slug: firmastat-cz-vyhledavani-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/firmastat-cz/openapi/firmastat-cz-vyhledavani-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
mechanism_count: 1
method: derived
name: Firmastat Authentication
name_suffix: Authentication
oauth_flows: []
overview: Firmastat secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: Firmastat
provider_slug: firmastat-cz
scheme_count: 1
schemes:
- bearerFormat: fs_<token>
  description: API klíč vydaný v účtu na /ucet. Platí pro REST i MCP a čerpá jednu společnou měsíční kvótu účtu. Klíč posílej jen ze serveru.
  name: apiKey
  scheme: bearer
  sources:
  - openapi/firmastat-cz-openapi.json
  type: http
slug: firmastat-cz-authentication
source_filename: firmastat-cz-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: derived\nsource: openapi/firmastat-cz-openapi.json\nsummary:\n  types:\n  - http\nschemes:\n- name: apiKey\n  type: http\n  scheme: bearer\n  bearerFormat: fs_<token>\n  description: API klíč vydaný v účtu na /ucet. Platí pro REST i MCP a čerpá jednu společnou\n    měsíční kvótu účtu. Klíč posílej jen ze serveru.\n  sources:\n  - openapi/firmastat-cz-openapi.json\n"
source_yaml_url: https://artifacts.apis.io/firmastat-cz/authentication/firmastat-cz-authentication.yml
summary_line: http · 1 scheme
tags:
- Company
- Czech
- Business
- Data
- Search
---
