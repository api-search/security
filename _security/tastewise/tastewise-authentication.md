---
api_key_in: []
auth_types: []
description: ''
kind: authentication
layout: security
method: searched
name: Tastewise Authentication
name_suffix: Authentication
oauth_flows: []
overview: Tastewise declares 2 security scheme(s) across its OpenAPI definitions.
provider_name: Tastewise
provider_slug: tastewise
scheme_count: 2
schemes:
- description: Bearer API key issued by Tastewise to the customer.
  format: 'Authorization: Bearer <your-api-key>'
  in: header
  name: BearerApiKey
  parameter_name: Authorization
  required: true
  scheme: bearer
  type: http
- description: Tenant/customer identifier issued alongside the API key.
  in: header
  name: CustomerId
  parameter_name: X-Customer-Id
  required: true
  type: apiKey
slug: tastewise-authentication
source_filename: tastewise-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-29'\nmethod: searched\nsource: https://docs.tastewise.io/\ndocs: https://docs.tastewise.io/\nnote: >-\n  Derived by hand from the provider's published API reference, not from an OpenAPI —\n  Tastewise publishes no machine-readable specification, so derive-authentication.py had\n  no spec to read. Every field below is quoted from docs.tastewise.io.\nsummary:\n  auth_types:\n  - http-bearer\n  - apiKey\n  api_key_locations:\n  - header\n  oauth2_flows: []\n  oauth2: false\n  openid_connect: false\n  mutual_tls: false\n  multi_factor: true\n  note: >-\n    Authentication is two-factor at the credential level: a bearer API key identifies the\n    integration and a separate X-Customer-Id header identifies the tenant. Both are required\n    on every authenticated request.\nschemes:\n- name: BearerApiKey\n  type: http\n  scheme: bearer\n  in: header\n  parameter_name: Authorization\n  format: 'Authorization: Bearer <your-api-key>'\n  required: true\n  description:\
  \ Bearer API key issued by Tastewise to the customer.\n- name: CustomerId\n  type: apiKey\n  in: header\n  parameter_name: X-Customer-Id\n  required: true\n  description: Tenant/customer identifier issued alongside the API key.\nalternative_formats:\n- name: combined-header\n  format: 'Authorization: Bearer <your-api-key>^customer-id'\n  description: >-\n    Some endpoints accept the API key and customer ID combined in a single Authorization\n    header, separated by a caret.\n  source: https://docs.tastewise.io/\nauthorization_model:\n  style: route-permissions\n  description: >-\n    Authorization is not scope-based. Each API route requires a named permission to be\n    enabled on the customer's account; a key without the permission is rejected. Permissions\n    are granted commercially, per contract, not requested at runtime.\n  permissions:\n  - permission: recipes\n    routes: [/recipes]\n    description: Recipe search and discovery\n  - permission: restaurants\n    routes: [/restaurants,\
  \ /k12]\n    description: Restaurant data and menus; K12 school foodservice data\n  - permission: restaurants_by_token\n    routes: [/restaurants/bestsellers, /restaurants/pricingAnalysis]\n    description: Bestseller analysis and price analysis (US only)\n  - permission: menus\n    routes: [/menus]\n    description: Menu item details\n  - permission: content_discovery\n    routes: [/content_discovery]\n    description: Social media content\n  - permission: motivations\n    routes: [/motivations]\n    description: Consumer motivations\n  - permission: flavour_combination\n    routes: [/flavor_combination]\n    description: Flavor pairing analysis\n  - permission: trend_performance\n    routes: [/trend_performance]\n    description: Trend tracking\n  - permission: trend_validation\n    routes: [/trend_validation]\n    description: Trend validation\n  - permission: widgets\n    routes: [/widgets]\n    description: Widget queries\n  - permission: insights\n    routes: [/insights]\n    description:\
  \ Combined insights\n  - permission: operations\n    routes: [/operations]\n    description: Combined restaurant/K12 data\nunauthenticated_endpoints:\n- path: /ping\n  method: GET\n  description: Health check; explicitly documented as requiring no authentication.\n  verified: probed\n  probe:\n    url: https://api.tastewise.io/ping\n    status: 200\n    body: healthy\n    fetched: '2026-08-29'\nerrors:\n  401: Unauthorized -- Either the API key, the Customer ID is wrong or you don't have access to the API.\n  403: Forbidden -- You are not allowed to perform the request.\nx-evidence:\n  fetched: '2026-08-29'\n  docs_url: https://docs.tastewise.io/\n  docs_http_status: 200\n  live_probe: https://api.tastewise.io/ping (200, \"healthy\")\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tastewise/refs/heads/main/authentication/tastewise-authentication.yml
summary_line: 2 schemes
tags:
- Company
- Food and Beverage
- Consumer Insights
- Market Intelligence
- Restaurant
- Menus
- Recipes
- Trends
- CPG
- Artificial Intelligence
- Data
- Analytics
---
