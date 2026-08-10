---
api_key_in: []
api_specs:
- filename: h1-insights-cost-estimates-api-openapi.yml
  format: yaml
  label: H1 Cost Estimates API
  slug: h1-insights-cost-estimates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/h1-insights/refs/heads/main/openapi/h1-insights-cost-estimates-api-openapi.yml
- filename: h1-insights-filters-api-openapi.yml
  format: yaml
  label: H1 Filters API
  slug: h1-insights-filters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/h1-insights/refs/heads/main/openapi/h1-insights-filters-api-openapi.yml
- filename: h1-insights-focus-area-endpoints-api-openapi.yml
  format: yaml
  label: H1 Focus Area Endpoints API
  slug: h1-insights-focus-area-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/h1-insights/refs/heads/main/openapi/h1-insights-focus-area-endpoints-api-openapi.yml
- filename: h1-insights-locations-api-openapi.yml
  format: yaml
  label: H1 Locations API
  slug: h1-insights-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/h1-insights/refs/heads/main/openapi/h1-insights-locations-api-openapi.yml
- filename: h1-insights-networks-api-openapi.yml
  format: yaml
  label: H1 Networks API
  slug: h1-insights-networks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/h1-insights/refs/heads/main/openapi/h1-insights-networks-api-openapi.yml
- filename: h1-insights-organizations-api-openapi.yml
  format: yaml
  label: H1 Organizations API
  slug: h1-insights-organizations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/h1-insights/refs/heads/main/openapi/h1-insights-organizations-api-openapi.yml
- filename: h1-insights-price-transparency-api-openapi.yml
  format: yaml
  label: H1 Price Transparency API
  slug: h1-insights-price-transparency-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/h1-insights/refs/heads/main/openapi/h1-insights-price-transparency-api-openapi.yml
- filename: h1-insights-providers-api-openapi.yml
  format: yaml
  label: H1 Providers API
  slug: h1-insights-providers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/h1-insights/refs/heads/main/openapi/h1-insights-providers-api-openapi.yml
- filename: h1-insights-reference-endpoints-api-openapi.yml
  format: yaml
  label: H1 Reference Endpoints API
  slug: h1-insights-reference-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/h1-insights/refs/heads/main/openapi/h1-insights-reference-endpoints-api-openapi.yml
- filename: h1-insights-tins-api-openapi.yml
  format: yaml
  label: H1 TI Ns API
  slug: h1-insights-tins-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/h1-insights/refs/heads/main/openapi/h1-insights-tins-api-openapi.yml
- filename: h1-insights-virtual-care-platforms-api-openapi.yml
  format: yaml
  label: H1 Virtual Care Platforms API
  slug: h1-insights-virtual-care-platforms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/h1-insights/refs/heads/main/openapi/h1-insights-virtual-care-platforms-api-openapi.yml
auth_types:
- http
description: ''
kind: authentication
layout: security
method: searched
name: H1 Insights Authentication
name_suffix: Authentication
oauth_flows: []
overview: H1 secures its APIs with http across 1 declared security scheme, as derived from its OpenAPI definitions.
provider_name: H1
provider_slug: h1-insights
scheme_count: 1
schemes:
- applied: global
  credential_type: A long-lived customer API key presented as a bearer token. Despite the http-bearer scheme this is an API key, not an OAuth 2.0 access token — there is no authorization server, no token endpoint, no refresh and no documented expiry.
  docs: https://ribbon.readme.io/docs/authentication
  header: 'Authorization: Bearer {customer_token}'
  key_prefix: not documented
  name: BearerAuth
  quote: '"The H1 API uses an API Key to authenticate requests. Authentication is performed by passing the token as an HTTP header in the Bearer Authentication scheme `Authorization: Bearer {customer_token}`."'
  rotation: not documented
  scheme: bearer
  sources:
  - openapi/h1-insights-openapi-original.json
  test_vs_live: No separate test/sandbox key or mode is published. Entitlement differences are expressed as account "packages" (Base API Access, Upgraded API, Add-Ons) and a trial account tier, not as key modes.
  type: http
slug: h1-insights-authentication
source_filename: h1-insights-authentication.yml
source_heading: Authentication Profile
source_url: ''
source_yaml: "generated: '2026-08-04'\nmethod: searched\nsource: openapi/h1-insights-openapi-original.json\ndocs: https://ribbon.readme.io/docs/authentication\nsummary:\n  types:\n  - http\n  http_schemes:\n  - bearer\n  api_key_in: []\n  oauth2_flows: []\n  scopes: false\n  mtls: false\n  openid_connect: false\nschemes:\n- name: BearerAuth\n  type: http\n  scheme: bearer\n  applied: global\n  sources:\n  - openapi/h1-insights-openapi-original.json\n  docs: https://ribbon.readme.io/docs/authentication\n  header: 'Authorization: Bearer {customer_token}'\n  quote: >-\n    \"The H1 API uses an API Key to authenticate requests. Authentication is performed by passing the token\n    as an HTTP header in the Bearer Authentication scheme `Authorization: Bearer {customer_token}`.\"\n  credential_type: >-\n    A long-lived customer API key presented as a bearer token. Despite the http-bearer scheme this is an\n    API key, not an OAuth 2.0 access token — there is no authorization server, no token\
  \ endpoint, no\n    refresh and no documented expiry.\n  rotation: not documented\n  key_prefix: not documented\n  test_vs_live: >-\n    No separate test/sandbox key or mode is published. Entitlement differences are expressed as account\n    \"packages\" (Base API Access, Upgraded API, Add-Ons) and a trial account tier, not as key modes.\nauthorization_model:\n  style: account-package entitlement\n  scopes: false\n  note: >-\n    There is no scope, permission or consent surface. What an authenticated caller may do is determined by\n    the account's contracted package. Calls outside the package return 403 permission_denied with an\n    explanatory message (for example \"Trial accounts do not have access to custom provider directories\",\n    \"This resource is managed by Ribbon and cannot be modified\"). An agent cannot narrow its own\n    privileges on this API — the token is all-or-nothing within the account's entitlement.\n  add_on_gated_surfaces:\n  - Provider Cost / Quality\n  - Eligibility\
  \ Check\n  - Price Transparency\n  upgraded_only_surfaces:\n  - Custom / Boost Filters\n  - Custom Fields / Data Editing\n  source: https://ribbon.readme.io/docs/ribbon-products\nunauthenticated_behaviour:\n  probed: '2026-08-04'\n  url: https://api.ribbonhealth.com/v1/\n  http_status: 401\n  body: >-\n    {\"error\": {\"status\": 401, \"code\": \"not_authenticated\", \"message\": \"You did not provide an API Key.\n    If you need help, please feel free to contact us at team@ribbonhealth.com!\"}}\n  note: The 401 response is not declared anywhere in the published OpenAPI.\nkey_acquisition:\n  self_serve: false\n  url: https://h1.com/request-demo/\n  note: >-\n    Keys are issued through a sales/demo request, not a self-serve developer signup. The docs direct new\n    users to \"sign up here\" (the request-demo form) and to support@h1.co for package questions.\ndiscovery:\n  openid_configuration: 404\n  oauth_authorization_server: 404\n  oauth_protected_resource: 404\n  source: well-known/h1-insights-well-known.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/h1-insights/refs/heads/main/authentication/h1-insights-authentication.yml
summary_line: http · 1 scheme
tags:
- healthcare
- provider-data
- provider-directory
- health-insurance
- price-transparency
- eligibility
- care-navigation
- health-plans
- digital-health
- life-sciences
- clinical-trials
- reference-data
---
