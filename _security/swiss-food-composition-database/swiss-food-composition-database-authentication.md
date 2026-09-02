---
api_key_in: []
api_specs:
- filename: swiss-food-composition-database-data-api-openapi.yml
  format: yaml
  label: Swiss Food Composition Database Data API
  slug: swiss-food-composition-database-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/swiss-food-composition-database/refs/heads/main/openapi/swiss-food-composition-database-data-api-openapi.yml
- filename: swiss-food-composition-database-stats-api-openapi.yml
  format: yaml
  label: Swiss Food Composition Database Stats API
  slug: swiss-food-composition-database-stats-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/swiss-food-composition-database/refs/heads/main/openapi/swiss-food-composition-database-stats-api-openapi.yml
- filename: swiss-food-composition-database-system-api-openapi.yml
  format: yaml
  label: Swiss Food Composition Database System API
  slug: swiss-food-composition-database-system-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/swiss-food-composition-database/refs/heads/main/openapi/swiss-food-composition-database-system-api-openapi.yml
- filename: swiss-food-composition-database-system-configuration-api-openapi.yml
  format: yaml
  label: Swiss Food Composition Database system configuration API
  slug: swiss-food-composition-database-system-configuration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/swiss-food-composition-database/refs/heads/main/openapi/swiss-food-composition-database-system-configuration-api-openapi.yml
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Swiss Food Composition Database Authentication
name_suffix: Authentication
oauth_flows: []
overview: Swiss Food Composition Database declares 0 security scheme(s) across its OpenAPI definitions.
provider_name: Swiss Food Composition Database
provider_slug: swiss-food-composition-database
scheme_count: 0
schemes: []
slug: swiss-food-composition-database-authentication
source_filename: swiss-food-composition-database-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-27'\nmethod: searched\nsource: >-\n  The FSVO's own API description document, \"The Swiss Food Composition Database API\" (published at\n  https://naehrwertdaten.ch/en/downloads/), which states: \"API is free to use and allows unrestricted access\"\n  and \"All of the available endpoints and methods are nonrestricted, free to access\". Corroborated by the\n  served OpenAPI 3.0.1 document, which declares no components.securitySchemes and no top-level security\n  requirement, and by live anonymous calls on 2026-08-27 that returned 200 with data.\ndocs: https://naehrwertdaten.ch/en/downloads/\nsummary: >-\n  No authentication of any kind. There is no API key, no OAuth, no signup and no account. Every one of the 21\n  operations is a public read that succeeds anonymously.\nschemes: []\nauth_required: false\nsignup_required: false\ncredential_types: []\ntransport:\n  https: true\n  tls_version: TLSv1.3\n  http_to_https_redirect: true\ncors:\n  enabled: true\n\
  \  access_control_allow_origin: '*'\n  access_control_allow_credentials: true\n  access_control_allow_methods: GET, PUT, POST, OPTIONS\n  note: >-\n    Observed on live responses 2026-08-27. The API is directly callable from a browser, which is how the\n    provider's own Swagger UI and search application consume it.\nevidence:\n  - url: https://api.webapp.prod.blv.foodcase-services.com/BLV_WebApp_WS/webresources/BLV-api/versiondb\n    status: 200\n    note: Anonymous GET returned {\"idversion\":51,\"versiontext\":\"V 7.1\"} with no credential supplied.\n  - url: https://api.webapp.prod.blv.foodcase-services.com/BLV_WebApp_WS/webresources/openapi.json\n    status: 200\n    note: Served OpenAPI declares no securitySchemes.\nobservations:\n  - >-\n    An administrative operation, GET /webresources/BLV-api/reloadCache (\"Reloads the local database cache of\n    the application\"), is exposed on the same unauthenticated public surface as the read operations. It is\n    tagged \"system configuration\"\
  \ in the provider's own spec. This is recorded as an observation about the\n    published contract; API Evangelist did not invoke it.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/swiss-food-composition-database/refs/heads/main/authentication/swiss-food-composition-database-authentication.yml
summary_line: 0 schemes
tags:
- Food
- Nutrition
- food-composition
- Health
- Open Data
- Government
- Switzerland
- Reference Data
- Public Sector
- Research
---
